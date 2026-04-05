# GreenTech-MVP-Sostenible_Version_Carmen_Alhaja_Garcia.
¿Cómo he eliminado la "Grasa Digital" (Refactorización)?
1. Hemos pasado de 83 líneas de código a 28.
2. Todo el diseño se apoya en CSS nativo y hace que la web reduzca mucho su peso.

Dentro del código HTML:
- He eliminado totalmente la dependencia del código de Bootstrap 5.3.0, que carga miles de líneas de CSS, que no sirven o no se usan en una página tan simple como esta. Al sustituirlo por CSS nativo, estamos ahorrando mucha energía, tiempo de carga y reducimos el peso de de la página de cientos de KB a solo unos pocos.
- He eliminado totalmente las tipografias externas al dispostivo (como Google Fonts o Font Awesome). He sustituido el icono de la hoja que es una fuente externa que requiere peticiones HTTP adicionales que ralentizan el enderizado, por un emoji de hoja, que es texto nativo y no pesa nada.

Dentro del CSS:
- He ajustado los parametros de la URL de Unsplash para reducir el tamaño de la imagen, que antes estaba en 3000px, que es excesivo para la mayoria de pantallas y lo he ajustado a 1200px.
  antes = (&w=3000&auto)
  ahora = (&w=1200&q=75)
- He cambiado la frase para dar a entender que el codigo es sostenible, al igual que el footer.
- He definido un bloque :root en el css para definir los colores principlaes. Esto mejora la mantenibilidad y la escalabilidad y si quieres cambiar un tono, lo cambias ahi y se cambia en todo el documento.
- He implementado el uso de clamp() para reducir las lineas de codigo al definir el tamaño rem que se debe usar en distintos dispositivos. Como tendriamos que escribir 3 o 4 reglas distintas, en lugar de escribir 10 o mas lineas, lo podemos hacer en una.
  clamp(mínimo, preferido, máximo)
