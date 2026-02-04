# Kotlin Interfaces

```kotlin
interface Drivable {
    fun drive()
}

class Car : Drivable {
    override fun drive() {
        println("Driving")
    }
}
```

Notes:
- Supports multiple interfaces
- Can include default methods
