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

👉 **Solución más compleja I:** ``[^b]og``  

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

👉 **Solución más compleja I:** ``^wa(z{2,})up$``  

👉 **Solución más compleja II:** ``waz{3,5}up``	 

👉 **Solución más compleja III:** ``waz*up``  


## 📚 **Exercise 7: Matching Repeated Characters** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado7.png?raw=true "Enunciado 8") 

👉 **Solución sencilla:**	``a{2,}b{1,}c{1,}``  

👉 **Solución más compleja I:** ``a{2,4}b{0,4}c{1,2}``	 

👉 **Solución más compleja II:** ``a+b+c+``  

👉 **Solución más compleja III:**	``a+b*c+``  

👉 **Solución más compleja IV:** ``(aa)+(b+)?c+``

## 📚 **Exercise 8: Matching Repeated Characters** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado8.png?raw=true "Enunciado 8")  

👉 **Solución sencilla:** ``^\d+\sfiles?\sfound\?``  

👉 **Solución más compleja I:** ``^\d+\s\w+\s\w+\?$``  

👉 **Solución más compleja II:** ``^\d+\s\w{4,5}\s\w{5}\?$``  

👉 **Solución más compleja III:** ``^\d+\s[^\W]{4,5}\s[^\W]{5}\?$``  

## 📚 **Exercise 9: Matching Whitespaces** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado9.png?raw=true "Enunciado 9")  

👉 **Solución sencilla:** ``\d\.\s+abc``  

👉 **Solución más complejaI:** ``\d\.\s{1,}abc``  

👉 **Solución más compleja II:** ``^\d\.\s+abc$``  

👉 **Solución más compleja III:** ``^\d\.\s+[a-c]{3}$``  

## 📚 **Exercise 10: Matching Lines** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado10.png?raw=true "Enunciado 10")  

👉 **Solución sencilla:** ``^Mission: successful$``  

👉 **Solución más complejaI:** ``^M.*l$``  

👉 **Solución más compleja II:** ``^M.*:.*l$``  

👉 **Solución más compleja III:** ``^M[ison]+:\s([sucefl]+)$``  

## 📚 **Exercise 11: Matching Groups** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado11.png?raw=true "Enunciado 11")  

👉 **Solución sencilla:** ``(file_record_transcript|file_07241999)\.pdf``  

👉 **Solución más complejaI:** ``^(file_\w+)\.pdf$``  

👉 **Solución más compleja II:** ``^(f.*)\.pdf$``  

👉 **Solución más compleja IV:** ``^(f.+)\.pdf$``  

## 📚 **Exercise 12: Matching Nested Groups** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado12.png?raw=true "Enunciado 12")  

👉 **Solución sencilla:** ``(\w+\s(\d+))``	

👉 **Solución más compleja I:** ``([JMA][au][nyg]\s(\d+))``		

👉 **Solución más compleja II:** ``((Jan|May|Aug)\s(\d+))``  

👉 **Solución más compleja IV:** ``([JAManayug]+\s(\d+))``  

## 📚 **Exercise 13: Matching Nested Groups** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado13.png?raw=true "Enunciado 13")

👉 **Solución sencilla:** ``(\d+)x(\d+)``  

👉 **Solución más compleja I:** ``(\d*)x(\d*)``  

👉 **Solución más compleja II:** ``(\d{4})x(\d{3,4})``	

👉 **Solución más compleja IV:** ``^([0-9]+)x([0-9]+)$``  

## 📚 **Exercise 14: Matching Conditional Text** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado14.png?raw=true "Enunciado 14")

👉 **Solución sencilla:** ````  

👉 **Solución más compleja I:** ````  

👉 **Solución más compleja II:** ````	

👉 **Solución más compleja IV:** ````







