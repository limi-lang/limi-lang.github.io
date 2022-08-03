# Type System

### Data Constructors
Sum type declarations are distributed over several lines.
```
true  : Bool
false : Bool
```
Translated as:
```
data Bool = true | false
```

Constructor Declarations can contain variables. We assume that T and Tree<T> are already defined and in scope
```
    t: T
=> Leaf(t) : Tree<T>

    left : Tree<T>
    right : Tree<T>
=> Node(left, right) : Tree<T>
```
Is roughly equivalent to:

```
data Tree<T> = Leaf(T) | Node(Tree<T>, Tree<T>)
```

The left hand side after the implication can be a mix fix operator
```
    A : Set
    B : Set
=> A -> B : Set
```
is translated as
```
data Set = _ -> _ (Set, Set)
```


### Mixfix operators
Data Type Declarations automatically declare mixfix operators. The two examples in the previous section also declare the
following mixfix operators.

```
Leaf ( _ ) : T -> Tree<T>
Node ( _ , _ ) : (Tree<T>, Tree<T>) -> Tree<T>
_ -> _ : (Set, Set) -> Set
```
The free mixfix operators pay for the slightly more verbose syntax. Actually the declared variables can be reused many times.


### Function Declarations.
The syntax for function declarations is exactly the same as that for Type Declarations.
```
   x : Nat
=> fact(x) : Int
```
In the same way the syntax defines a mixfix operator.
```
fact ( _ ) : Nat -> Int
```
