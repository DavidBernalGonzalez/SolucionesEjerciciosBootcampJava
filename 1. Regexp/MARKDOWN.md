# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 1. Ejercicios de https://regexone.com/  

<mark>**1.1 -  Matching Characters:**</mark>

- **Solución simple/sencilla: `` regex abc ``** → Cuando queremos que el match sea explicitamente abc  
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejer1/1.1.png?raw=true "Cuando queremos que el match sea explicitamente abc")

- **Solución "más compleja" I: ``^abc.*``**  → Cuando queremos que el match empiece explicitamente por abc y, posteriormente contenga 0 o más caracteres utilizando la estrella de kleene.
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejer1/1.2.png?raw=true "Cuando queremos que el match empiece explicitamente por abc y, posteriormente contenga 0 o más caracteres utilizando la estrella de kleene.")

-  **Solución más compleja II: ``^abc.{0,}``** → Cuando queremos que el match empiece explicitamente por abc y posteriormente utilizando el caracter . (JOKER/comodín) tenga 0 o más caracteres. Esta solución es equivalente a la anterior solución
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejer1/1.3.png?raw=true "Cuando queremos que el match empiece explicitamente por abc y posteriormente utilizando el caracter . (JOKER/comodín) tenga 0 o más caracteres. Esta solución es equivalente a la anterior solución")

<mark>**1.½ -  Matching Characters:**</mark>
- **Solución sencilla:	`` 123 ``** → Cuando queremos que el match sea explicitamente 123 
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejer1/1.3.png?raw=true "Cuando queremos que el match sea explicitamente 123")

- **Solución más compleja I: `` \d+``**	 → Cuando queremos que coja todos los dígitos independientemente de la cantidad
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejer1.2/1.2.png?raw=true "Cuando queremos que el match sea explicitamente 123")
  
- **Solución más compleja II: ``\d{3}	``** → Cuando queremos que coja solamente los grupos de 3 dígitos
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejer1.2/1.3.png?raw=true "Cuando queremos que el match sea explicitamente 123")

- **Solución más compleja III: ``\d{3,} ``** → Cuando queremos que coja solamente los grupos de 3 dígitos o más dígitos (equivalente a solución II)
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejer1.2/1.4.png?raw=true "Cuando queremos que el match sea explicitamente 123")

<mark> **Exercise 2: Matching With Wildcards:** </mark>