# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 📖Ejercicios de https://regexone.com/📖 

## 📚 **Exercice 1: Matching Characters:** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/ejer1/Enunciado1.png?raw=true  "Enunciado ejercicio 1")

👉 **Solución simple/sencilla: ``abc ``** → Cuando queremos que el match sea explicitamente abc  

👉 **Solución "más compleja" I: ``^abc.*``**  → Cuando queremos que el match empiece explicitamente por abc y, posteriormente contenga 0 o más caracteres utilizando la estrella de kleene.  

👉 **Solución más compleja II: ``^abc.{0,}``** → Cuando queremos que el match empiece explicitamente por abc y posteriormente utilizando el caracter . (JOKER/comodín) tenga 0 o más caracteres. Esta solución es equivalente a la anterior solución.  

## 📚 **Exercice 1.½ -  Matching Characters:** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado%201.2.png?raw=true  "Enunciado ejercicio 1.½")

👉 **Solución sencilla:	`` 123 ``** → Cuando queremos que el match sea explicitamente 123  

👉 **Solución más compleja I: `` \d+``**	 → Cuando queremos que coja todos los dígitos independientemente de la cantidad  
  
👉 **Solución más compleja II: ``\d{3}	``** → Cuando queremos que coja solamente los grupos de 3 dígitos  

👉 **Solución más compleja III: ``\d{3,} ``** → Cuando queremos que coja solamente los grupos de 3 dígitos o más dígitos (equivalente a solución II)  

## 📚 **Exercise 2: Matching With Wildcards** 📚

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado2.png?raw=true "Enunciado 2")  

👉 **Solución sencilla:** ``...\.``	→ Cuando queremos seleccionar tres caracteres (los que sean) utilizando el comodín/Joker y después queremos que haya un punto explicitamente .

👉 **Solución sencilla II:** ``.{3}\.``	→ Cuando queremos seleccionar tres caracteres (los que sean) utilizando el comodín/Joker junto al {3} y después queremos que haya un punto explicitamente .

👉 **Solución más compleja I:** ``(cat\.|896.|\?\=\+\.)`` → Cuando queremos que literalmente literalmente cat. 896. o ?=+. podemos hacerlo mediante a grupos

👉 **Solución más completa II:** ``.*\.$`` → Cuando queremos que venga lo que sea (si es que hay algo) pero que acabe en un .

👉 **Solución más completa III:** ``(\w+|\W+)\.`` → Cuando queremos que venga una palabra o bien caracteres especiales (sin importar la canatidad pero tienes que haber) y después un .	

👉 **Solución más completa IV:** ``^(\w+|\W+)\.$`` → Lo mismo que la solución (III) anterior  pero empezando y acabando, por lo que sería un poco más exacta.

## 📚 **Exercise 3: Matching Characters** 📚

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado3.png?raw=true "Enunciado 3")

👉 **Solución sencilla:** ``^[cmf]an$``  

👉 **Solución más compleja I:**	``(can|man|fan)``  

👉 **Solución más compleja II:** ``(c|m|f)an`` → equivalente a la solución anterior  

👉 **Solución más compleja III:** ``^(c|m|f)an$``  

👉 **Solución más completa IV:** ``^[^drp]an$`` → Cuando queremos que no empiece por drp y que la línea acabe por an  

## 📚 **Exercise 4: Excluding Characters** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado4.png?raw=true "Enunciado 4")

👉 **Solución sencilla:** ``^[hg]og`` → todo lo que tenga una h (minuscula) o una g (minuscula) seguido de una o y una g  

👉 **Solución más complejaI:** ``[^b]og`` → todo lo que tenga una b (minuscula) como primer caracter y vaya seguido de una o y una g  

👉 **Solución más compleja II:** ``^[^b]og$`` → todo lo que no empiece con una b (minuscula) como primer caracter y acabe en og  

## 📚 **Exercise 5: Matching Character Ranges** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado5.png?raw=true "Enunciado 4")  

👉 **Solución sencilla:** ``[A-C][anobpc]+``
👉 **Solución más complejaI:** ``[A-C][n-p][a-c]``				
👉 **Solución más compleja II:** ``^[A-Z]..$``
👉 **Solución más compleja III:** ``^[A-Z][n-p][a-c]$``
