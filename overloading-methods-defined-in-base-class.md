```
public class B
{
    public void Foo2(IEnumerable<D2> parm)
    {
        Console.WriteLine("In B.Foo2");
    }
}

public class D : B
{
    public void Foo2(IEnumerable<B2> parm)
    {
        Console.WriteLine("In D.Foo2");
    }
}

var sequence = new List<D2> { new D2(), new D2() };
var obj2 = new D();

obj2.Foo2(sequence);
```
