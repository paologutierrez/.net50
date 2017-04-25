```
public class FooController
{
    public IActionResult Index()
    {
        var fooService = new FooService(new BarService(), new BazService());
        return View(fooService.GetFoo());
    }
}
```






