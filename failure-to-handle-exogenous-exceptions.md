```

try 
{   
  using ( File f = OpenFile(filename, ForReading) )   
  {
    // Blah blah blah   
  } 
} 
catch (FileNotFoundException) 
{   
  // Handle file not found 
}

```