```
Point point1 = new Point(20, 30);
Point point2 = point1;
point2.X = 50;
Console.WriteLine(point1.X);       // 20 (does this surprise you?)
Console.WriteLine(point2.X);       // 50
  
Pen pen1 = new Pen(Color.Black);
Pen pen2 = pen1;
pen2.Color = Color.Blue;
Console.WriteLine(pen1.Color);     // Blue (or does this surprise you?)
Console.WriteLine(pen2.Color);     // Blue
```
