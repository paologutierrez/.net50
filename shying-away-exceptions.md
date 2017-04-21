```
  // METHOD 1:
  // Throws an exception if account can't be cast to SavingsAccount
  SavingsAccount savingsAccount = (SavingsAccount)account;
  
  // METHOD 2:
  // Does NOT throw an exception if account can't be cast to
  // SavingsAccount; will just set savingsAccount to null instead
  SavingsAccount savingsAccount = account as SavingsAccount;
```