
### Dealing with Exceptions

```Java
public static void main(String[] args) {  
    // -> deal with exceptions with try catch blocks
    try {  
       // planned code  
       canThrowException();
    } catch (Exception ex) {  
        // in case of exception  
    } finally {  
        // after try or catch  
    }  
}  

// -> Or throws the exception to be dealt with later 
public static void canThrowException() throws Exception {  
    // code ...  
    
    // you can also throw an Exception manually
    if(conditionToException()) {  
        throw new Exception("Exception message");  
    }
}
```

### Checked Exceptions 

- Have to be dealt with at compile time
- Exceptions and their subclasses that **are not RuntimeException or its subclasses**
- Ex: IOException, SQLException etc..
- The program doesn't compile without dealing with it
### Unchecked Exceptions
- Are not checked in compile time,  only in run time
- RuntimeException and it subclasses
- Ex: NullPointerException, NumberFormatException etc..
- The program will compile without dealing with it 