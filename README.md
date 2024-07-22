```kotlin
fun main() {
    // Declaración de Variables
    val velocidadLuz: Int = 299_792_458  // Variable inmutable
    println("La velocidad de la luz es: $velocidadLuz m/s")
    
    var planeta: String = "Tierra"  // Variable mutable
    println("Planeta inicial: $planeta")
    
    planeta = "Marte"  // Modificación de variable mutable
    println("Planeta modificado: $planeta")

    // Manejo de Nulos
    var mensajeNoNulo: String = "Este mensaje nunca es nulo"
    println(mensajeNoNulo)

    var mensajeOpcional: String? = "Este mensaje puede ser nulo"  // Variable que puede ser nula
    println(mensajeOpcional)

    mensajeOpcional = null  // Asignación de valor nulo
    println(mensajeOpcional)

    // Opcionales
    var ciudadOpcional: String? = null
    val longitudCiudad: Int = ciudadOpcional?.length ?: 10 
    println("Longitud del nombre de la ciudad: $longitudCiudad")

    ciudadOpcional = "Quito"
    val longitudNombreCiudad: Int? = ciudadOpcional?.length  // 
    println("Longitud del nombre de la ciudad: $longitudNombreCiudad")
    
    ciudadOpcional = null
    val longitudNombreCiudadNulo: Int? = ciudadOpcional?.length
    println("Longitud del nombre de la ciudad nulo: $longitudNombreCiudadNulo")
}
