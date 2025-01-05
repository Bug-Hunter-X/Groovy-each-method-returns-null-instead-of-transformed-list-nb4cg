# Groovy 'each' Method Unexpected Null Return

This example demonstrates a common pitfall when using the `each` method in Groovy.  The `each` method iterates over a collection and applies a closure to each element, but it doesn't return a modified collection.  This often leads to unexpected `null` return values.

The provided `bug.groovy` file shows the problem. The `each` method is used to double each element in a list, but the result printed is `null`.

The solution, `bugSolution.groovy`, uses the `collect` method which returns a new list containing the transformed elements.  This is the more idiomatic Groovy way to achieve the desired transformation.