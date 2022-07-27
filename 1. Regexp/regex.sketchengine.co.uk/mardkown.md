# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 📖Ejercicios de https://regex.sketchengine.co.uk/📖 

## 📚 **Exercice 1** 📚
![Error, la imagen no se ha podido cargar](https://raw.githubusercontent.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/main/1.%20Regexp/regex.sketchengine.co.uk/Ejercicio1.png?raw=true  "Enunciado ejercicio 1")

👉 **Solución:** ``^p.t$|^s.{2,}(t|e|o)$|^r.*``

## 📚 **Exercice 2** 📚
![Error, la imagen no se ha podido cargar](https://raw.githubusercontent.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/main/1.%20Regexp/regex.sketchengine.co.uk/Ejercicio2.png?raw=true  "Enunciado ejercicio 2")

👉 **Solución I:** ``rap\sthem|tapeth|apth|wrap\/try|sap\stray|87ap9th|apothecary``  


👉 **Solución II:** ``((^(r).{2}\s\w+)|(^(t).p.{2}h$)|(^(a).*[^t|s]$)|(^(w|s).*y$)|(^\d).*)``  

👉 **Solución III:** ``((^(\w{3})+\s\w+)|((\d|w).*)|((^(t).[^r]).*)|(^(a).*(y|th)))``	
