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
    private val school: String,
    private val study: String,
    private var schoolYear: Int
) {
    override fun toString(): String {
        return "👋 Hello, I'm $firstName, a perpetual learner exploring the wonders of technology!\n" +
                "🎂 I've orbited the sun $age times and counting.\n" +
                "💻 My cosmic interests include: ${tech.joinToString()}\n" +
                "🎓 Currently pursuing a degree in $study at $school, cruising through year $schoolYear.\n"
    }
}

fun main() {
    // Initializing profile
    val alex = Person(
        "Alex",
        32,
        mutableListOf("HTML", "CSS", "JavaScript", "PHP", "Python", "Kotlin", "C#", ".NET"),
        "Avans University of Applied Sciences",
        "Information Technology",
        2
    )
    println(alex.toString())
}
```

👋 Hello, I'm Alex, a perpetual learner exploring the wonders of technology!\
🎂 I've orbited the sun 31 times and counting.\
💻 My cosmic interests include: HTML, CSS, JavaScript, PHP, Python, Kotlin, C#, .NET\
🎓 Currently pursuing a degree in Information Technology at Avans University of Applied Sciences, cruising through year 2.
