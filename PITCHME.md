## Error Handling

#HSLIDE

Overview of our presentation structure

#HSLIDE

### What is Error Handling?

 * The anticipation, detection, and resolution of errors in an application 
 * Helps in maintaining the normal flow of the app
 * Throwable
    - the superclass of all errors and exceptions in the Java language
    - A throwable contains a snapshot of the execution stack of its thread at the time it was created
    - It can also contain a message string that gives more information about the error
    - The recording of this causal information is referred to as the chained exception facility, as the cause can, itself, have a cause, and so on, leading to a "chain" of exceptions, each caused by another
 * Subclasses: Error and Exception
 * Checked and Unchecked  

#HSLIDE

### public class Error extends Throwable() {}

 * Serious problem has occurred that you should not try to catch
 * Why? Recovery from this error is not possible
    - StackOverflowError, OutOfMemoryError
    - Errors are usually related to the environment the app is running in
 * All unchecked types (not checked at compile time)   
     
#HSLIDE
     
### public class Exception extends Throwable() {} 

 * Checked and Unchecked types
    - Unchecked -> RuntimeException (other examples extend Runtime -> ArithmeticException)
    - Checked -> Everything else (SQLException, IOException)
    
 * Program is responsible for creating these exceptions (vs. the environment)

#HSLIDE

### Why do we have Error Handling?
 
 * As developers we are responsible for making sure our code does what it's supposed to. When things break, proper error handling can help us get back in the green as soon as possible.
 * (Show example of an uncaught stacktrace and a handled exception) 
 * something about try catch finally?

#HSLIDE

### When do we use Error Handling?

 * When we care about our future selves.
 
 (When to not use Error Handling)
 

