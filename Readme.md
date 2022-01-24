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


## Blocks

if, for, switch : all code inside the statement
switch or select : clauses get a block  


