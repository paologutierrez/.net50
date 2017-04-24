```

class MyFirstClass //default protection = internal
{
    public void NameFunction() {
        MySecondClass sc = new MySecondClass();
        sc.strFirstName = "Harry";
        sc.strLastName = "Potter";
        Console.WriteLine("Name: " + sc.FirstName + " " + sc.strLastName);
    }
}

public class MySecondClass
{
    string strFirstName = "Roy";
    string strLastName = "Weasley"; //default protection = private
}
```