# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 📖Ejercicios de https://regexone.com/📖 

## 📚 **Exercice 1: Matching Characters:** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado1.png?raw=true  "Enunciado ejercicio 1")

👉 **Solución simple/sencilla:** ``abc``

👉 **Solución "más compleja" I:** ``^abc.*``

👉 **Solución más compleja II:** ``^abc.{0,}``

👉 **Solución más compleja III:** ``^abc(.?)+``

## 📚 **Exercice 1.½ -  Matching Characters:** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado%201.2.png?raw=true  "Enunciado ejercicio 1.½")

👉 **Solución sencilla:**	``123``

👉 **Solución más compleja I:** ``\d+``  
  
👉 **Solución más compleja II:** ``\d{3}``

👉 **Solución más compleja III:** ``\d{3,}``

👉 **Solución más compleja III:** ``[^\D]+``

## 📚 **Exercise 2: Matching With Wildcards** 📚

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado2.png?raw=true "Enunciado 2")  

👉 **Solución sencilla:** ``^...\.$``

👉 **Solución sencilla II:** ``^.{3}\.$``

👉 **Solución más compleja I:** ``^(cat|896|\?\=\+)\.$``

👉 **Solución más completa II:** ``.*\.$``

👉 **Solución más completa III:** ``^(\w+|\W+)\.$``

## 📚 **Exercise 3: Matching Characters** 📚

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado3.png?raw=true "Enunciado 3")

👉 **Solución sencilla:** ``^[cmf]an$``  

👉 **Solución más compleja I:**	``(can|man|fan)``  

👉 **Solución más compleja II:** ``(c|m|f)an``

👉 **Solución más compleja III:** ``^(c|m|f)an$``  

👉 **Solución más completa IV:** ``^[^drp]an$``

## 📚 **Exercise 4: Excluding Characters** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado4.png?raw=true "Enunciado 4")

👉 **Solución sencilla:** ``^[hd]og`` 

👉 **Solución más complejaI:** ``[^b]og``  

👉 **Solución más compleja II:** ``^[^b]og$`` 

## 📚 **Exercise 5: Matching Character Ranges** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado5.png?raw=true "Enunciado 5")  

👉 **Solución sencilla:** ``[A-C][anobpc]+``  

👉 **Solución más compleja I:** ``[A-C][n-p][a-c]``  

👉 **Solución más compleja II:** ``^[A-Z]..$``  

👉 **Solución más compleja III:** ``^[A-Z][n-p][a-c]$`` 

## 📚 **Exercise 6: Matching Repeated Characters** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado6.png?raw=true "Enunciado 6") 

👉 **Solución sencilla:** ``waz+up``	

👉 **Solución más complejaI:** ``^wa(z{2,})up$``  

👉 **Solución más compleja II:** ``waz{3,5}up``	 

👉 **Solución más compleja III:** ``waz*up``  


## 📚 **Exercise 7: Matching Repeated Characters** 📚


