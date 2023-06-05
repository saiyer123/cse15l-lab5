# Part 1

What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?
Hello, I am using a MacBook Pro and have Google Chrome open, VS Studios, and the terminal.

Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.
I am running the tests for this scenario, but I am getting an error when I run it, even though I expected it to pass. 
Here is the screenshot.
![Image](cse15l-lab5-error.png)


Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.

The commands I am running are `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java.`
and `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ArrayTests.java`
These are the only 2 commands I ran, and there was nothing before. The main things I noticed by the error message were these two lines
`java.lang.IllegalArgumentException: Could not find class [ArrayTests.java]` and `Caused by: java.lang.ClassNotFoundException: ArrayTests.java`.
Here is a screenshot of my code ![Image](cse15l-lab5-code.png)
