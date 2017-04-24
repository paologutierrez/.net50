```
 
private const int NUM_ITERATIONS = 20000;
private const decimal DENOMINATOR = 200m;
private const decimal MAX_POSSIBLE_VALUE = NUM_ITERATIONS / DENOMINATOR;

private static decimal sharedState;
public static decimal SharedState {
	get {
		return sharedState;
	}
	set {
		sharedState = value;
	}
}

static void Main(string[] args) {
	Thread writerThread = new Thread(WriterThreadEntry);
	Thread readerThread = new Thread(ReaderThreadEntry);

	writerThread.Start();
	readerThread.Start();

	writerThread.Join();
	readerThread.Join();

	Console.ReadKey();
}

private static void WriterThreadEntry() {
	for (int i = 0; i < NUM_ITERATIONS; ++i) {
		SharedState = i / DENOMINATOR;
	}
}

private static void ReaderThreadEntry() {
	for (int i = 0; i < NUM_ITERATIONS; ++i) {
		var sharedStateLocal = SharedState;
		if (sharedStateLocal > MAX_POSSIBLE_VALUE) Console.WriteLine("Impossible value detected: " + sharedStateLocal);
	}
}
```