# Go Lang

Efficent as C and high level as python.
Compiled language with garbage collection.

## OOPs

Class is structs in Go but it doesnt support inheritance, generics and constructors.

## Concurrency 

Supports concurrency through Goroutines (threads), channels and select

## Variables 

var x int; has Keyword name type format.
Supported declaration formats :
    var x,y int;

Types :
    can define alias for specific types
    type celcius float16
    type name string

Constant :
    Declares const immutable values
    const x  = 1.3
    const ( // Declaring multiple constats
        y = 4
        name = "Austin"
    )

Iota (enumerator) :
    Constants with random values
    const (
        Monday int = iota // all other variables would also be iota
        Tuesday
        wednesday 
    )

## Control flow 

if :

```
 if <condition> {
    <statements>
}
    if x> 5 {
        fmt.Println("> 5")
    }
```

For : 
```
    for <init>; <condition>; <update> { // these 3 are optional. without any its an infinite loop
        <statements>
    }

    for i:=0; i< 10; i++ {
        fmt.Printf("%d", i);
    }
```

Switch : 
    Switch automatically breaks on a match.
```
    switch <tag> { // tag is optional, then cases are conditions.
        case <value1> :
            <statements>
        case <Value2>:
            <statements>
        default:
            <statements>
    }

    var x int = 10;
    switch x {
        case 1 :
            fmt.Printf("Case 1")
        case 2 :
            fmt.Printf("case 2")
        default :
            fmt.Printf("case 3")
    }

```

## User input 

fmt.Scan() does the scanning

var num int
fmt.Println("Enter an int")
fmt.Scan(&num) // takes in the int and assign to num.
fmt.Println(num)

## Blocks

if, for, switch : all code inside the statement
switch or select : clauses get a block  

## Composite Data type

Arrays :
    all values initailized to zero
```
    var array [5]int
    array[1] = 2
    fmt.printf(x[0]) // prints 0
```
    Iteration 
```
    array := [...]int{1,2,3,4}
    for i,v range array {
        fmt.Printf("index %d contains %d", i, v)
    }
```

Array Literal :
    used to initailize an array
```
    var x [5] int = [5]{1,2,3,4,5} // RHS is the literal
    x := [...]int{1,2,3,4} // initializes array with 4 literals
```


Slice :
    a section of an array
```
    arr := [...] string {1,2,3,4,5}
    s1 := arr[1:3] // slice
```