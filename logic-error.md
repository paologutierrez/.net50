```

private void button1_Click(object, sender, EventArgs e)
{
    int startLoop = 11;
    int endLoop = 1;
    int answer = 0;
    
    for (int i = startLoop; i < endLoop; i++)
    {
        answer = answer + i;
    }
    
    MessageBox.Show("answer =" + answer.ToString());
}

```