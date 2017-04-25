```

private ListBox SomeListBox;
private ObservableCollection<string> SomeStrings = new ObservableCollection<string>();
 
public void SomeMethod()
{
    SomeListBox.ItemsSource = null;
    ThreadPool.QueueUserWorkItem(o => AddToStrings());
}
 
private void AddToStrings()
{
    // this line will actually crash the app!
    SomeStrings.Add("blah");
 
    Dispatcher.BeginInvoke(new Action(() => SomeListBox.ItemsSource = SomeStrings);
}

```