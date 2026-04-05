# GreenTech-MVP-Sostenible_Version_Carmen_Alhaja_Garcia.
¿Cómo he eliminado la "Grasa Digital" (Refactorización)?
1. Hemos pasado de 83 líneas de código a 29.
2. Todo el diseño se apoya en CSS nativo y hace que la web reduzca mucho su peso.

Dentro del código HTML:
- He eliminado totalmente la dependencia del código de Bootstrap 5.3.0, que carga miles de líneas de CSS, que no sirven o no se usan en una página tan simple como esta. Al sustituirlo por CSS nativo, estamos ahorrando mucha energía, tiempo de carga y reducimos el peso de de la página de cientos de KB a solo unos pocos.
-

Dentro del CSS:
- La imagen se carga con un ancho de 1200px y calidad optimizada en lugar de los 3000px del código anterior pesado.
- He cambiado la frase para dar a entender que el codigo es sostenible, al igual que el footer.
- He cambiado las fuentes y usado tipografias nativas del dispostivo. Por ejemplo, en el botón "Quiero ayudar" para que sea mas grande y llamativo.

1. Hemos eliminado por completo Bootstrap, jQuery, FontAwesome y Moment.js.
3. Reducción de peticione http. Al no cargar librerias externas ni fuentes de Google, el navegador realiza menos conexiones al servidor, ahorrando energía en los centros de datos y en la red de transmisión.
5. Bajo consumo de CPU: Al eliminar scripts pesados, el procesador no se sobrecalienta, lo que tiene un impacto positivo en la batería y la durabilidad de la vida de los dispositivos.
