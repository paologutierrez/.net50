```

public class Parent
{
  public Parent()
  {
    Console.WriteLine("Parent Ctor");
    Method();
  }

  public virtual void Method()
  {
    Console.WriteLine("Parent method");
  }
}

public class Child : Parent
{
  public Child()
  {
    Console.WriteLine("Child Ctor");
  }

  public override void Method()
  {
    Console.WriteLine("Child method");
  }
}

```