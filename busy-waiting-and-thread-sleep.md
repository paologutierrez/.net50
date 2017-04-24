```
 
private static string userInput;

private static void Example() {
	userInput = null;
	GetUserInput(); // tells the UI to request user input on the UI thread
	
	while (userInput == null) ; // wait for user input
	
	ProcessUserInput(userInput); // now use that input
}

```