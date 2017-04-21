```
  decimal total = 0;
  foreach (Account account in myAccounts) {
    if (account.Status == "active") {
      total += account.Balance;
    }
  }
```