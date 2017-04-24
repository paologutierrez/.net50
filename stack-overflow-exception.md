```
class Program
{
    private static int hitCount;

    static void Main(string[] args)
    {
        hitCount = 0;
        MyRecursiveExample(null);
    }

    static void MyRecursiveExample(string value)
    {
        hitCount++;

        if (value == null)
        {
            MyRecursiveExample(value);
        }
        else
        {
            System.Console.WriteLine(value);
        }
    }
}

```