# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 📖Ejercicios del documento de Word📖 

## 📚 **Ejercicio 1:** 📚
Basándote en el fichero original, añade un “)” inmediatamente después del primer número del resultado debe ser el siguiente:
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Exercice01.png "Enunciado ejercicio 1")

**Solución ejercicio 1:**
Con esto estamos seleccionando únicamente todos los dígitos del principio de la línea que sean tanto 
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion1.png "Solución ejercicio 1")
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion1-3.png "Solución ejercicio 1")
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion1-2.png "Solución ejercicio 1")

## 📚 **Ejercicio 2:** 📚
Basándote en el fichero original, haz que todos los elementos tengan un solo espacio entre palabra y palabra. Por tanto, es necesario quitar tabulaciones y doble espaciados. Además, también debes de seleccionar los espacios del final independientemente de si son tabulaciones o espacios.  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Exercice02.png "Enunciado ejercicio 2")

**Solución ejercicio 2:**  
Primeramente, seleccionamos las casuisticas que tengan dos o más espacios (aparecen con puntitos cuando los subrayamos) o bien una o varias tabulaciones (aparecen como una flecha cuando las subrayamos). Y los reemplazamos por un solo espacio poniendo un espacio en el campo de replace.
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2.png "Solución ejercicio 2")  
Aquí vemos la explicación de la expresión regular:  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-2.png "Solución ejercicio 2")  
Ahora, solamente tenemos el problema con los espacios finales
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-3.png "Solución ejercicio 2")  
Nos bastará con realizar lo siguiente:
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-4.png "Solución ejercicio 2")  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-6.png "Solución ejercicio 2")     
Y ahora si, que tenemos este apartado finalizado:  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion2-5.png "Solución ejercicio 2")  

## 📚 **Ejercicio 3:** 📚
Basándote en el fichero original, sustituye todos los subdominios de los correos que acaben en cl o ch por gmail (incluidos los que ya tengan dicha casuística):
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Exercice03.png "Enunciado ejercicio 3")
El resultado será el siguiente:
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion3-1.png "Solución ejercicio 3")  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion3-2.png "Solución ejercicio 3")  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion3-3.png "Solución ejercicio 3")  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/ejercicio-entregable/Solucion3-4.png "Solución ejercicio 3")  

## 📚 **Ejercicio 4:** 📚
Elimina todo lo que no sea un email de cada una de las líneas:


 


