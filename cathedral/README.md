# Cathedral of introduction to functional programming

## First one to fall

image::https://d1u5p3l4wpay3k.cloudfront.net/diablo_gamepedia/2/2f/Fallen_%28Diablo_I%29.gif?version=2197831347a1e9e1ee94fc04b4805dca[]

First exercises come in the form of Fibonacci numbers. Wiki says:
The Fibonacci numbers are the numbers in the following integer sequence, called the Fibonacci sequence, and characterized by the fact that every number after the first two is the sum of the two preceding ones.

Our task is to write a function to compute the nth fibonacci number [1]

```
  def fib(n: Int): Int
```

For this, we will reach out to just learned recursion. 

We mentioned:
 - tailrecursion
 - higer order funciton
 - polymorphic functions

Dig through the book to understand why we use tailrecursion and how to define higer order funciton.

Solutions for Cathedral can be found here https://github.com/fpinscala/fpinscala/blob/master/answers/src/main/scala/fpinscala/gettingstarted/GettingStarted.scala 

## Scavenge that array

image::https://diablo.gamepedia.com/File:Scavenger_(Diablo_I).gif[]

We got some exp, we can add a bit of points to intelegence and try next task.
We are expected to write a a polymorphic function to check whether an `Array[A]` is sorted [2]

```  
def isSorted[A](as: Array[A], gt: (A,A) => Boolean): Boolean = ???
```


[1]https://github.com/fpinscala/fpinscala/blob/master/answers/src/main/scala/fpinscala/gettingstarted/GettingStarted.scala - Examples are taken from repo that comes with the book.
