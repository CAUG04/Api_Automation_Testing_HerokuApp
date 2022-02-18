# Api_Automation_Testing_HerokuApp
Este proyecto es un reto técnico con Karate APi Framework usando la Api de HerokuApp

Tabla de contenido

Introducción
Probando API con Karate
requisitos previos
Ejecutar las pruebas localmente


Introducción
En este proyecto se aplican los ejemplos más comunes de pruebas con el marco de Karate. Para aplicar los casos de prueba, utilizaremos el sitio web de prueba https://reqres.in/ , que proporciona varios puntos finales en los que puede realizar solicitudes GET, PUT, POST y DELETE.

Probando API con Karate
Karate es la única herramienta de código abierto que combina automatización de pruebas de API, simulacros, pruebas de rendimiento e incluso automatización de la interfaz de usuario en un solo marco unificado. La sintaxis BDD popularizada por Cucumber es independiente del lenguaje y fácil incluso para los no programadores. Las aserciones potentes de JSON y XML están integradas, y puede ejecutar pruebas en paralelo para aumentar la velocidad.
La ejecución de pruebas y la generación de informes se sienten como cualquier proyecto Java estándar. Pero también hay un ejecutable independiente para equipos que no se sienten cómodos con Java. No tienes que compilar código. Simplemente escriba pruebas en una sintaxis simple y legible, cuidadosamente diseñada para HTTP, JSON, GraphQL y XML. Y puede combinar la automatización de pruebas de API y UI dentro del mismo script de prueba.
https://github.com/intuit/karate

requisitos previos
El proyecto está desarrollado en Java con Maven por lo que instalará el siguiente software:

SDK de Oracle Java 8
Apache experto
Su IDE favorito, que incluye:


Eclipse IDE (o IDE basado en Eclipse, se recomienda Spring ToolSuite)

Intellij IDEA : Para ejecutar pruebas de características o escenarios configurará:




[Run configuration with Cucumber Java template]
    Main class: com.intuit.karate.cli.Main    
    Glue: com.intuit.karate



Ejecutar las pruebas localmente
Para intentar ejecutar la demostración en el sistema local, ingrese a la carpeta raíz y ejecute los siguientes comandos para instalar las dependencias e iniciar los corredores de prueba uno por uno.

mvn clean install -DskipTests
mvn clean test -Dtest=ExamplesRunner
mvn clean test -Dtest=DemoTestParallel
