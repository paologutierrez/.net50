```

<acmecompany:PersonalEditorControl Grid.Row="0" x:Name="personEditor"/>

private void DeleteData_OnClick(object sender, RouteEventArgs e)
{
    if (personEditor != null)
    {
        _grid.Children.Remove(personEditor);
        personEditor = null;
    }
}
```