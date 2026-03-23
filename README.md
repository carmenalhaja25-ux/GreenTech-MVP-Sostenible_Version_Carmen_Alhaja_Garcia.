# GreenTech-MVP-Sostenible_Version_Carmen_Alhaja_Garcia.
¿Cómo he eliminado la "Grasa Digital" (Refactorización)?
1. Hemos eliminado por completo Bootstrap, jQuery, FontAwesome y Moment.js.
2. Todo el diseño se apoya en CSS nativo y hace que la web reduzca mucho su peso.
3. Reducción de peticione http. Al no cargar librerias externas ni fuentes de Google, el navegador realiza menos conexiones al servidor, ahorrando energía en los centros de datos y en la red de transmisión.
4. La imagen se carga con un ancho de 1200px y calidad optimizada en lugar de los 3000px del código anterior.
5. Bajo consumo de CPU: Al eliminar scripts pesados, el procesador no se sobrecalienta, lo que tiene un impacto positivo en la batería y la durabilidad de la vida de los dispositivos.
7. Al usar tipografías nativas del dipositivo, evitamos el renderizado de archivos de fuentes externos, lo que ahorra batería y memoria RAM.
