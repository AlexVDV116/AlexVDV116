```Kotlin
class Person(
    private val firstName: String,
    private var age: Int,
    private val code: MutableList<String>,
) {
    override fun toString(): String {
        return "Hello, my name is $firstName, I am $age years of age.\n " +
                "I like to code in: $code"
    }
}

fun main() {
    val alex = Person("Alex", 31, mutableListOf("HTML", "CSS", "JavaScript", "PHP", "Python", "Kotlin"))
    println(alex.toString())
}
```
