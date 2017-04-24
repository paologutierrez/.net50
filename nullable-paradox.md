```
 
private static void DoTestA() {
    int? maybeInt = null;
    for (int i = 0; i < 100000; ++i) {
        DoSomething(maybeInt);
    }
}
 
private static void DoTestB() {
    int? maybeInt = 3;
    for (int i = 0; i < 100000; ++i) {
        DoSomething(maybeInt);
    }
}
 
private static void DoSomething(object o) {
    // Do something...
}

```