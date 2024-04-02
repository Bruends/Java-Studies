- a way to use *anonymous functions* in Java 
- can be passed to other methods or stored in a variable
- Lambdas are often used along with Collections an Streams 


Syntax:
```java
(parameters) -> expression
// or
(parameters) ->  {
	statements
	...
	...
}
```

Example: 
```java
public class Main {  
    public static void main(String[] args) {  
        ArrayList<String> games = new ArrayList<>(Arrays.asList(  
                "Street Fighter 6",  
                "Sekiro",  
                "Counter Strike 2"  
        )); 
  
        games.forEach((game) -> System.out.println(game));  
    }  
}
```
