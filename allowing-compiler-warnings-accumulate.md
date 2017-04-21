```
  class Account {
  
      int myId;
      int Id;   // compiler warned you about this, but you didn’t listen!
  
      // Constructor
      Account(int id) {
          this.myId = Id;     // OOPS!
      }
  
  }
```