# Cathedral or introduction to functional programming

## First one to fall

![first one](https://d1u5p3l4wpay3k.cloudfront.net/diablo_gamepedia/2/2f/Fallen_%28Diablo_I%29.gif?version=2197831347a1e9e1ee94fc04b4805dca)

First exercises come in the form of Fibonacci numbers. Wiki says:
*The Fibonacci numbers are the numbers in the following integer sequence, called the Fibonacci sequence, and characterized by the fact that every number after the first two is the sum of the two preceding ones.*

Our task is to write a function to compute the nth fibonacci number

```
  def fib(n: Int): Int
```

For this, we will reach out to just learned recursion. 

We should end this task with next loot:

 - tailrecursion
 - function inside a function

Dig through the book to understand why we use tailrecursion and how to define higer order funciton.



## Scavenge that array

![Scavanger](https://d1u5p3l4wpay3k.cloudfront.net/diablo_gamepedia/8/8d/Scavenger_%28Diablo_I%29.gif?version=f93598aa94853bc368ececf5d1c37d64)

We got some exp, we can add a bit of points to intelegence and try next task.
We are expected to write a a polymorphic function to check whether an `Array[A]` is sorted

```  
def isSorted[A](as: Array[A], gt: (A,A) => Boolean): Boolean = ???
```

This monster is not a difficult one but it drops some unique items:

 - higer order funciton
 - polymorphic functions
 - anonymous functions

## Curry me further

![Skeleton](https://d1u5p3l4wpay3k.cloudfront.net/diablo_gamepedia/0/04/Skeleton_%28Diablo_I%29.gif?version=5f70421d890b68881bc6ea037978b998)

Oops we are atacked by the pack, and it is a curry pack. 

Lets try to solve:

```
def curry[A,B,C](f: (A, B) => C): A => (B => C) = ???
```

and
```
  def uncurry[A,B,C](f: A => B => C): (A, B) => C = ???
```

What we have in the loot:

- Function.uncurried

## How is zombie composed?

![zombie](https://d1u5p3l4wpay3k.cloudfront.net/diablo_gamepedia/1/14/Zombie_%28Diablo_I%29.gif?version=24113720a76014d2a03582a9ebc69dd2)

Lets find out by doing:

```
def compose[A,B,C](f: B => C, g: A => B): A => C = ???
```

He stumbels and fall and behind him we find

- f `compose` g
- f `andThen` g

## Don't forget

Solutions for Cathedral can be found [here](https://github.com/fpinscala/fpinscala/blob/master/answers/src/main/scala/fpinscala/gettingstarted/GettingStarted.scala)

All examples are taken from repo that comes with the book: https://github.com/fpinscala/fpinscala/blob/master/answers/src/main/scala/fpinscala/gettingstarted/GettingStarted.scala - now go and buy this awesome book
