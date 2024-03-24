```Kotlin
/**
 * Meet Alex - Tech Enthusiast 🚀
 * -----------------------------------
 * Hey there! I'm Alex, a passionate tech aficionado on a journey through the digital universe.
 * Here's a glimpse into my world:
 */
class Person(
    private val firstName: String,
    private var age: Int,
    private val tech: MutableList<String>,
    private val hobbies: MutableList<String>,
    private val school: String,
    private val study: String,
    private var schoolYear: Int
) {
    override fun toString(): String {
        return "👋 Hello, my name is $firstName, a perpetual learner exploring the wonders of technology!\n" +
                "🎂 I've orbited the sun $age times and counting." +
                "💻 My cosmic interests include: ${tech.joinToString()}\n" +
                "🌟 My hobbies include: ${hobbies.joinToString()}\n" +
                "🎓 Currently pursuing a degree in Information Technology at $school, cruising through year $schoolYear.\n"
    }
}

fun main() {
    val alex = Person(
        "Alex",
        31,
        mutableListOf("HTML", "CSS", "JavaScript", "PHP", "Python", "Kotlin", "C#", ".NET"),
        mutableListOf("Working out in the gym", "Star Wars", "Cyber security/hacking"),
        "Avans University of Applied Sciences",
        "Information Technology",
        2
    )
    println(alex.toString())
}

```

👋 Hello, my name is Alex, a perpetual learner exploring the wonders of technology! \
🎂 I've orbited the sun 32 times and counting. \
💻 My cosmic interests include: HTML, CSS, JavaScript, PHP, Python, Kotlin, C#, .NET \
🌟 My hobbies include: Working out in the gym, Star Wars, Cyber security/hacking \
🎓 Currently pursuing a degree in Information Technology at Avans University of Applied Sciences, cruising through year 2.
