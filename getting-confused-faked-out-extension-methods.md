```
  public decimal SumAccounts(IEnumerable<Account> myAccounts) {
      return myAccounts.Sum(a => a.Balance);
  }
```