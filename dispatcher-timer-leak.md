```

public byte[] myMemory = new byte[50 * 1024 * 1024];

System.Windows.Threading.DispatcherTimer _timer = new System.Windows.Threading.DispatcherTimer();
int count = 0;


private void MyLabel_Loaded(object sender, RoutedEventArgs e)
{

    _timer.Interval = TimeSpan.FromMilliseconds(1000);

    _timer.Tick += new EventHandler(delegate(object s, EventArgs ev)

    {
        count++;
        textBox1.Text = count.ToString();
    });

    _timer.Start();
}
```