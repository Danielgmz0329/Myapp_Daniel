```kotlin
fun main() {
    // Declaración de Variables
    val pi: Double = 3.14159  // Variable inmutable
    println("El valor de pi es: $pi")
    
    var nombre: String = "Juan"  // Variable mutable
    println("Nombre inicial: $nombre")
    
    nombre = "Pedro"  // Modificación de variable mutable
    println("Nombre modificado: $nombre")

    // Manejo de Nulos
    var noNulo: String = "Este es un valor no nulo"
    println(noNulo)

    var puedeSerNulo: String? = "Este valor puede ser nulo"  // Variable que puede ser nula
    println(puedeSerNulo)

    puedeSerNulo = null  // Asignación de valor nulo
    println(puedeSerNulo)

    // Opcionales
    var nombreOpcional: String? = null
    val longitud: Int = nombreOpcional?.length ?: 0 
    println("Longitud del nombre: $longitud")

    nombreOpcional = "Kotlin"
    val longitudNombre: Int? = nombreOpcional?.length 
    println("Longitud del nombre: $longitudNombre")
    
    nombreOpcional = null
    val longitudNombreNulo: Int? = nombreOpcional?.length
    println("Longitud del nombre nulo: $longitudNombreNulo")
}
