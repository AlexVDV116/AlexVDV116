```Kotlin
class Person(
    private val firstName: String,
    private var age: Int,
    private val tech: MutableList<String>,
    private val school: String,
    private val study: String,
    private var schoolYear: Int
) {
    override fun toString(): String {
        return "Hello, my name is $firstName, I am $age years of age.\n" +
                "Some web technologies I am interested in are ${tech.joinToString()}\n" +
                "I am studying $study at the $school, currently in year $schoolYear.\n"
    }
}

fun main() {
    val alex = Person(
        "Alex",
        31,
        mutableListOf("HTML", "CSS", "JavaScript", "PHP", "Python", "Kotlin"),
        "Avans University of Applied Sciences",
        "Information Technology",
        2
    )
    println(alex.toString())
}
```

Hello, my name is Alex, I am 31 years of age.

I like to code in: [HTML, CSS, JavaScript, PHP, Python, Kotlin]

Process finished with exit code 0
