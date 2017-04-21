```
  decimal total = (from account in myAccounts
                   where account.Status == "active"
                   select account.Balance).Sum();
```