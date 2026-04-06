# GreenTech-MVP-Sostenible_Version_Carmen_Alhaja_Garcia.
Este es mi codigo refactorizado.
El codigo anterior que teniamos que refactorizar era un codigo pesado, dificil de leer e incoherente, que icluye tanto html como css y Java Script. Lo que he echo, principalmente, ha sido reducir el peso de este codigo.

1. Lo primero que he cambiado y se ha notado en su peso, es cambiar el html con css interno, separandolos en dos archivos distintos que van enlazados. He pasado de tener un codigo de 83 líneas a 28 líneas.

2. Tambien, dentro del html, he modificado algunas adiciones eran innecesarias y que consumen mucha energia, como el uso de Bootstrap, que carga muchisimas lineas de CSS que muchas veces en codigos tan sencillos como este no se utilizan. Haciendo el CSS externo ajustandose a lo que necesita la pagina se ahorra mucho espacio.

3. También, en el codigo original, se usan tipografias externas del dispositivo como las de Google y las he modificado por tipografias nativas. Por ejemplo, he sustituido el icono de la hoja, que esta dentro del boton, que es una fuente externa y la he cambiado por un emoticono y no hace que se tengan que hacer peticiones adicionales que relentizan el codigo, cuando podemos usar emoticono.

También, he cambiado varias cosas en el CSS y he implementado algunas practicas sostenibles:
En primer lugar, he cambiado el tamaño de la imagen principal de la pagina que anteriormente estaba en 3000px y la he cambiado a 1200px, que se ajustan perfectamente al tamaño de la pagina, sin necesidad de que la imagen se salga de los margenes, no encajen y de un visto feo a la pagina.

También, he añadido un bloque :root en el que he definido los colores principales de la pagina y en lugar de ponerlo repetidas veces y tener que modificar uno x uno cuando quieras cambiar un color, lo modificas en el :root y se cambia en esos varios lugares que tu quieras a la vez.

Por ultimo, he usado clamp() en el css que tambien es una buena practica (para reducir lineas de codigo), cuando queremos definir el tamaño rem que se debe usar en distintos dispositivos. Por ejemplo si queremos hacer que la pagina sea visible tanto como para portatiles, moviles o tables, sin usar clamp nos puede ocupar 10 lineas de codigo definir todo eso mientras que usandolo lo podemos hacer en una. Usando clamp, dentro del parentesis ponemos primero un valor minimo, en el medio el valor preferido y luego el valor maximo que queramos usar.

Todas estas practicas hacen que el HTML sea mas facil de leer, aparte de mas sostenible y que el CSS sea reutilizable.
