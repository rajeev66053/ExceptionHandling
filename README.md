# Exception Handling

* Exception is an abnormal condition which occurs during the execution of a program and distrupts normal flow of the program. If not handled properly it can cause the program to terminate abruptly.


### Hierarchy of exception handling

1. Throwable
	1. Exception
		1. Checked Exception
			1. IO Exception
			2. SQL Exception
			3. ClassNotFound Exception
			4. FileNotFound Exception
		2. Unchecked Exception/Runtime Exceptions
			1. Null Pointer Exception
			2. Number Format Exception
			3. Index OutOfBound Exception
				1. ArrayIndexOutOfBound Exception
				2. StringIndexOutOfBound Exception
	2. Error
		1. StackOverflow Error
		2. OutOfMemory Error
		3. Virtual Machine Error
		

### Difference between Exception and Error

* We can recover from exception using try catch block or using throw. Recovering from error is not possible.
* In Exception, compiler will have knowledge about checked exceptions hence compiler will force to use try catch blocks. In Error, compiler will not have any knowledge about unchecked exceptions and Errors.
* Exceptions are related to application. Errors are related to environment where application is running.
* Exceptions include both checked and unchecked type. All errors in java are unchecked type.
* Exceptions in java are of type java.lang.Exception. Errors in java are of type java.lang.Error.




* We cannot write try block without catch or finally block otherwise we will get compile time error  saying " insert finally to cmplete try statement" like this.
* If main method throw an exception then java runtime terminates the program and prints the exception message and the stack trace in system console.

### Difference between Throw and Throws
* Java throw keyword is used to explictly throw an exception. Java throws keyword is used to declare an exception.
* Checked exception cannot be propagated using throw only. Checked Exception can be propagated with throws.
* Throw is used within the method. Throws is used with the method signature.
* You cannot throw multiple exceptions. you can declare multiple exceptions using throws.