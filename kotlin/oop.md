# Kotlin Classes & Objects

## Primary Constructor
```kotlin
class Person(var name: String, var age: Int) {
    fun sayHello() = println("Hi! I'm $name!")
}
```

---

## Init Block
```kotlin
class Person(name: String, age: Int) {
   var name = name
   var age = age

   init {
      println("Created $name")
   }
}
```

---

## Custom Getters & Setters
```kotlin
class Person {
   var age = 0
      set(value) {
         if (value >= 0) {
            field = value
         }
      }

   val hasAccess: Boolean
      get() = age >= 18
}
```
