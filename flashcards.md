## Give an example for local variable type inference
```java
var list = new ArrayList<String>();  // infers ArrayList<String>
var stream = list.stream();          // infers Stream<String>
```
----

## Additional local-variable syntax for lambda parameters
```java
list.stream()
      .map((@Notnull var s) -> s.toLowerCase())
      .collect(Collectors.toList());
```
