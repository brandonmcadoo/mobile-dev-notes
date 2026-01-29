# Kotlin Lambdas

Lambdas are unnamed functions used for short, one-off logic.

```kotlin
val findSum = { a: Int, b: Int -> a + b }
```

Single parameter lambdas use `it`:
```kotlin
"Bookkeeper".count { it == 'e' }
```

Common usage:
```kotlin
val nums = listOf(1, 2, 3, 4)
val evens = nums.filter { it % 2 == 0 }
val doubled = nums.map { it * 2 }
```

Used heavily in:
- Collections
- Coroutines
- Android callbacks
