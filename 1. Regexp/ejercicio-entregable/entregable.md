# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 📖Ejercicios del documento de Word📖 

## 📚 **Ejercicio 1:** 📚
Basándote en el fichero original, añade un “)” inmediatamente después del primer número del resultado debe ser el siguiente:   

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Exercice01.png "Enunciado ejercicio 1")

### **Solución ejercicio 1:**  
Con esto estamos seleccionando únicamente todos los dígitos del principio de la línea que tengan tanto uno o varios dígitos.  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion1.png "Solución ejercicio 1")
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion1-3.png "Solución ejercicio 1")
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion1-2.png "Solución ejercicio 1")

## 📚 **Ejercicio 2:** 📚
Basándote en el fichero original, haz que todos los elementos tengan un solo espacio entre palabra y palabra. Por tanto, es necesario quitar tabulaciones y doble espaciados. Además, también debes de seleccionar los espacios del final independientemente de si son tabulaciones o espacios.  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Exercice02.png "Enunciado ejercicio 2")

### **Solución ejercicio 2:**  
Primeramente, seleccionamos las casuisticas que tengan dos o más espacios (aparecen con puntitos cuando los subrayamos) o bien una o varias tabulaciones (aparecen como una flecha cuando las subrayamos). Y los reemplazamos por un solo espacio poniendo un espacio en el campo de replace.  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2.png "Solución ejercicio 2")  

Aquí vemos la explicación de la expresión regular:  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-2.png "Solución ejercicio 2")  

Ahora, solamente tenemos el problema con los espacios del final  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-3.png "Solución ejercicio 2")  

Nos bastará con realizar lo siguiente:  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-4.png "Solución ejercicio 2")  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-6.png "Solución ejercicio 2")    

Y ahora si, que tenemos este apartado finalizado:  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-5.png "Solución ejercicio 2")  

## 📚 **Ejercicio 3:** 📚
Basándote en el fichero original, sustituye todos los subdominios de los correos que acaben en cl o ch por gmail (incluidos los que ya tengan dicha casuística):  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Exercice03.png "Enunciado ejercicio 3")  

### **Solución ejercicio 3:**  

Si nos metemos en la web de https://regex101.com/ al salir en distintos colores los grupos, esto, puede ayudar a entender mejor el trabajo de grupo que queremos hacer:  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion3-1.png "Solución ejercicio 3")  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion3-2.png "Solución ejercicio 3")  

Si nos fijamos, vemos que ha una parte que no capturamos en nuestro patrón dentro de un grupo, la que vamos a substituir. Por lo que solamente necesitamos realizar la llamada a los grupos que si que capturamos y meter la palabra gmail en medio:  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion3-3.png "Solución ejercicio 3")  

El resultado será el siguiente:  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion3-4.png "Solución ejercicio 3")  

## 📚 **Ejercicio 4:** 📚
Elimina todo lo que no sea un email de cada una de las líneas:

### **Solución ejercicio 4. Manera I (en 2 pasos):**  

Vamos a arreglar la cosa a hachazos🪓, para ello, vamos a realizar unas pequeñas marcas en el documento, en este caso puntos comas con los que será más fácil cortar el contenido que no nos interesa de las líneas.

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion4.png "Solución ejercicio 4")  

Una vez reemplazado, tenemos dos ; uno en cada lado de email para cortar el documento.Por lo que aplicando la siguiente formula:

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion4-2.png "Solución ejercicio 4")  

Obtendremos el siguiente resultado:  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion4-3.png "Solución ejercicio 4") 

### **Solución ejercicio 4. Manera II (en 1 solo paso):**  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion4-B.png "Solución ejercicio 4")  

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion4-3.png "Solución ejercicio 4")

