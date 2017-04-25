```
public class HomeController
{
  private readonly IExampleService _service;

  public HomeController()
  {
    _service = new ExampleService();
  }

  public ActionResult Index()
  {
    return View(_service.GetSomething());
  }
}
```






