# Kotlin Basics

## Program Structure
```kotlin
fun main() {
    println("Hello, world")
}
```

Java:
```java
public static void main(String[] args) {
    System.out.println("Hello, world");
}
```

---

## Comments
```kotlin
// Single line comment

/*
   Multi
   Line
   Comment
*/
```

---

## Variables

`var` = mutable  
`val` = immutable  

```kotlin
var num = 0
var num: Int
num = 0
var num: Int = 0
```

---

## Printing & String Templates
```kotlin
val word = "World"
println("Hello $word")
println("2 + 2 = ${2 + 2}")
```

---

## Conditionals
```kotlin
if (condition) {
    body
} else if (otherCondition) {
    body
} else {
    body
}
```

---

## When Statements
```kotlin
val coinType = when (coinValue) {
   1 -> "Penny"
   5 -> "Nickel"
   10 -> "Dime"
   25 -> "Quarter"
   in 50..70 -> "Magical"
   else -> "Unknown"
}
```

---

## Loops
```kotlin
for (count in 1..4) {
   println(count)
}

for (count in 5 downTo 1 step 2) {
   println(count)
}
```

---

## Functions
```kotlin
fun findAverage(num1: Int, num2: Int): Double {
   return (num1 + num2) / 2.0
}

fun sayHello(name: String, greeting: String = "Hello") {
   println("$greeting, $name!")
}
```
