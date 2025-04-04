![Alex's GitHub stats](https://github-readme-stats.vercel.app/api?username=AlexVDV116&show_icons=true&theme=transparent&hide_rank=true)


```Kotlin
import java.time.LocalDate
import java.time.Period

/**
 * Meet Alex - Tech Enthusiast 🚀
 * -----------------------------------
 * Hey there! I'm Alex, a passionate tech aficionado on a journey through the digital universe.
 * Here's a glimpse into my world:
 */
data class Person(
    val firstName: String,
    val birthYear: Int,
    val tech: MutableList<String>,
    val hobbies: MutableList<String>,
    val school: String,
    val study: String,
    val startYear: Int
) {
    private val currentYear = LocalDate.now().year
    private val age: Int
        get() = Period.between(LocalDate.of(birthYear, 1, 1), LocalDate.now()).years
    private val schoolYear: Int
        get() = currentYear - startYear + 1

    override fun toString(): String {
        return """
            👋 Hello, my name is $firstName, a perpetual learner exploring the wonders of technology!
            🎂 I've orbited the sun $age times and counting.
            💻 My interests include: ${tech.joinToString()}.
            🌟 My hobbies include: ${hobbies.joinToString()}.
            🎓 Currently pursuing a degree in $study at $school, cruising through year $schoolYear.
            🌍 Fun fact: I'm always learning something new - the journey never stops!
        """.trimIndent()
    }
}

fun main() {
    val alex = Person(
        "Alex",
        1991,
        mutableListOf("HTML", "CSS", "JavaScript", "PHP", "Python", "Kotlin", "C#", ".NET"),
        mutableListOf("Working out in the gym", "Science", "Sci-Fi: Star Wars", "Cyber security/hacking"),
        "Avans University of Applied Sciences",
        "Information Technology",
        2021
    )
    println(alex.toString())
}

```

👋 Hello, my name is Alex, a perpetual learner exploring the wonders of technology!\
🎂 I've orbited the sun 33 times and counting.\
💻 My interests include: HTML, CSS, JavaScript, PHP, Python, Kotlin, C#, .NET.\
🌟 My hobbies include: Working out in the gym, Science, Sci-Fi: Star Wars, Cyber security/hacking.\
🎓 Currently pursuing a degree in Information Technology at Avans University of Applied Sciences, cruising through year 4.\
🌍 Fun fact: I'm always learning something new - the journey never stops!

