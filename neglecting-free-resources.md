```
  using (FileStream myFile = File.OpenRead("foo.txt")) {
    myFile.Read(buffer, 0, 100);
  }
```