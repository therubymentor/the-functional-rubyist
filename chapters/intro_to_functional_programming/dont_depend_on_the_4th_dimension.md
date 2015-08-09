## Don't Depend on the 4th Dimension

Pure code (code without side-effects) is beautiful code because it is not polluted by the reality of Time. I know, I know, "What the hell does _polluted by time_ even mean man?". Imagine a ledger program. It has a value that is your balance and that number can be positive or negative.

For the moment pretend that value is just a variable:

```ruby
balance = 0.0
```

Now as you update the balance you change the balance variable:

```ruby
balance = 0.0

balance += 1.5
```

So the balance started at 0.0 and then was changed when the 1.5 was added to it. At the end of this code sample the value is now at 1.5. This is the model proposed by Turing. And when coders talk of 'moving parts' they are talking about global variables that change. The `operation` here is an `addition`.

Since we have no idea what the balance was 5 minutes ago, once we change it we have _introduced time_ into our application. The result of balance is an every changing value. There is no way to go back if we add a bad value. There is no way of knowing what the value was 6 edits ago.

### Using a transaction log

Now let's look at the Church model for doing the same thing:

```ruby
transactions = []

def balance
  transactions.reduce(:+)
end

transactions << 1.5
```

The balance is now a calculation. It is no longer dependent on time. We don't ever _overwrite_ the balance. We now have a list of values that can be positive or negative and when you sum them all together (the call to reduce) you get the balance as it is _now_.

You could add another transaction, and then do another calculation minus the recently added transaction and you can get the balance from before you added that new transaction.

That is the big difference between the two models of computing. In the Turing model there is 'no going back', and in the Church model you can essentially have your Delorean and drive it too.
