# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 1. Ejercicios de https://regexone.com/  

<mark>**1.1 -  Matching Characters:**</mark>

- **Solución simple/sencilla: `` regex abc ``** → Cuando queremos que el match sea explicitamente abc  
![Este contenido se mostrará cuando la imagen no se pueda cargar, como texto alternativo](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejercicio1/Screenshot_1.png?raw=true "Cuando queremos que sea literalmente abc")

- **Solución "más compleja" I: ``^abc.*``**  → Cuando queremos que el match empiece por abc y, posteriormente 0 o más caracteres utilizando la estrella de kleene.
![Este contenido se mostrará cuando la imagen no se pueda cargar, como texto alternativo](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejercicio1/Screenshot_2.png?raw=true "Cuando queremos que sea literalmente abc")

-  **Solución más compleja II: ``^abc.{0,}``** → Cuando queremos que el match empiece por abc y posteriormente utilizando el caracter . (JOKER/comodín) tenga 0 o más caracteres. Esta solución es equivalente a la anterior solución
![Este contenido se mostrará cuando la imagen no se pueda cargar, como texto alternativo](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejercicio1/Screenshot_3.png?raw=true "Cuando queremos que sea literalmente abc")

<mark>**1.½ -  Matching Characters:**</mark>
- **Solución sencilla:	`` 123 ``** → Cuando queremos que el match sea explicitamente 123  
- **Solución más compleja I: `` \d+``**	 → Cuando queremos que coja todos los dígitos independientemente de la cantidadç
- **Solución más compleja II: ``\d{3}	``** → Cuando queremos que coja solamente los grupos de 3 dígitos
- **Solución más compleja III: ``\d{3,} ``** → Cuando queremos que coja solamente los grupos de 3 dígitos o más dígitos (equivalente a solución II)