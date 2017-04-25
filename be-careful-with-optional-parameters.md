```

public class Base
{
    public virtual void Foo(Int32 x = 1) 
    {}   
}

public class Derived
{
    public override void Foo(Int32 x = 2)
    {}
}

...

Base f0 = new Base();
f0.Foo();                // Invokes Foo(1)

Base f1 = new Derived();
f1.Foo();               // Also invokes Foo(1)

Derived f2 = new Derived();
f2.Foo();               // Invokes Foo(2)
```