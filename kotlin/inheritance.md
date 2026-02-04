# Kotlin Inheritance

```kotlin
open class Animal {
    open fun speak() {
        println("Animal sound")
    }
}

class Dog : Animal() {
    override fun speak() {
        println("Bark")
    }
}
```

Notes:
- Classes are final by default
- Use `open` to allow inheritance
- Use `override` to replace behavior
