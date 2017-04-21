```
  class Program {
      static Point point1;
      static Pen pen1;
      static void Main(string[] args) {
          Console.WriteLine(pen1 == null);      // True
          Console.WriteLine(point1 == null);    // False (huh?)
      }
  }
```