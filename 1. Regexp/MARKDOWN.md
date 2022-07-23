# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 📖Ejercicios de https://regexone.com/📖 

## 📚 **Exercice 1: Matching Characters:** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado1.png?raw=true  "Enunciado ejercicio 1")

👉 **Solución simple/sencilla: ``abc``** → Cuando queremos que el match sea explícitamente ``abc``  
<details>
  <summary>Ver esquema</summary>
  
</details>

👉 **Solución "más compleja" I: ``^abc.*``**  → Cuando queremos que la línea empiece explícitamente por ``abc``. Posteriormente, utilizando el ``.`` (JOKER/comodín) el cual nos permitirá tener un carácter cualquiera, es decir, no importa el carácter que sea. Finalmente, seguidamente del ``.``, añadimos el cuantificador ``*`` para hacer que contenga 0 o más caracteres. 
> 🚨Recordad que el símbolo que en este caso utilizamos como quantifier ``*`` es el conocido como la estrella de Kleene (que como ya dijimos durante el curso homenajea a uno de los padres de las expresiones regulares).🚨

👉 **Solución más compleja II: ``^abc.{0,}``** → Cuando queremos que la línea empiece explícitamente por ``abc``. Posteriormente, utilizando el ``{0,}`` hacemos que pueda venir cualquier carácter  0 o más veces. 
> 🚨Esta solución es muy similar y por tanto equivalente a la solución "más compleja" I que acabamos de ver. 🚨

👉 **Solución más compleja III: ``^abc(.?)+``** → Cuando queremos que la línea empiece explícitamente por ``abc``. Posteriormente, hemos realizado un grupo mediante a los ``()``. En el interior de dicho grupo, hemos añadido un ``.`` (JOKER/comodín) el cual nos permitirá tener un carácter cualquiera, es decir, no importa el carácter que sea. Finalmente, seguidamente del ``.``, añadimos un ``?`` el cual hará que el carácter (JOKER) sea opcional. Finalmente, añadimos un ``+`` para que el grupo anterior se pueda repetir 1 o más veces.

## 📚 **Exercice 1.½ -  Matching Characters:** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado%201.2.png?raw=true  "Enunciado ejercicio 1.½")

👉 **Solución sencilla:	``123``** → Cuando queremos que el match realizado sea explícitamente ``123``  

👉 **Solución más compleja I: ``\d+``**	 → Cuando queremos que el match sea con todos los dígitos e independientemente de la cantidad  
  
👉 **Solución más compleja II: ``\d{3}``** → Cuando queremos que coja solamente los grupos de 3 dígitos  

👉 **Solución más compleja III: ``\d{3,}``** → Cuando queremos que coja solamente los grupos de 3 dígitos o más dígitos (equivalente a solución II)  

👉 **Solución más compleja III: ``\d{3,}``** → Cuando queremos que coja solamente los grupos de 3 dígitos o más dígitos (equivalente a solución II) 

👉 **Solución más compleja IV: ``[^\D]+``** → Los corchetes ``[]`` nos permiten definir rangos. En su interior, vamos a añadir ``\D`` para seleccionar todo lo que no sea un dígito.  
>🚨``\D`` es equivalente a definir el rango ``0-9``. Por lo que podríamos utilizarlo para definir el rango ya que ambos son equivalentes🚨  

Finalmente, antes del ``\D`` pero contenido entre los ``[]`` vamos a añadir un ``^`` para invertir el rango seleccionado. Por tanto, en este caso, estaremos seleccionando todos elementos que sean un dígito. Finalmente, añadimos un ``+`` después de los ``[]`` para poder seleccionar que el rango puede ser repetido una o más veces.

## 📚 **Exercise 2: Matching With Wildcards** 📚

![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado2.png?raw=true "Enunciado 2")  

👉 **Solución sencilla: ``^...\.$``**	→  Cuando queremos hacer match sobre una línea que contenga un texto que empiece ``^`` con tres caracteres sin importar los que sean una manera de hacer es utilizar el comodín/joker tres veces ``...``. Posteriormente, queremos que haya un punto explícitamente. Por lo que escribimos un ``\.`` para hacer referencia a dicho carácter en concreto. Finalmente, seguido del ``\.`` escribimos un ``$`` para indicar que queremos que este sea el fin del texto y de la línea.

👉 **Solución sencilla II: ``^.{3}\.$``**	→ Cuando queremos hacer match sobre una línea que contenga un texto que empiece ``^`` con un carácter sin importar el que sea utilizamos el comodín/joker. Y, posteriormente, añadimos un ``{3}`` para que el comodín se repita 3 veces en concreto. Finalmente, añadimos un ``\.`` ya que en esta ocasiones no queremos utilizar el comodín/joker sino explícitamente un punto. Finalmente, seguido del ``\.`` escribimos un ``$`` para indicar que queremos que este sea el fin del texto y de la línea.

👉 **Solución más compleja I: ``^(cat|896|\?\=\+)\.$``** → Cuando queremos hacer match sobre una línea que contenga un texto que empiece ``^`` explícitamente sobre uno de los siguientes textos: ``cat`` o ``896`` o ``?=+``. Para seleccionar los tres hacemos un grupo ``()`` y separamos dichos valores por un ``|``. En caso del último bloque como son caracteres que nuevamente tienen una cierta funcionalidad dentro del regexp, cuando queremos utilizarlos deben de ir definidos junto a un ``\`` quedando dicho bloque de la siguiente manera ``\?\=\?``. Finalmente, queremos que en los 3 casos, el texto acabe en un . por lo que volver a utilizar el ``\`` seguido del ``.``. Y, añadimos un ``$`` para indicar que queremos que este sea el final del texto y de la línea.

👉 **Solución más completa II: ``.*\.$``** → Cuando queremos hacer match sobre una línea que contenga un texto sin importar el que sea podemos utilizar el comodín/joker ``.`` junto al quantifier ``*``. Con ello, hacemos que venga 0 o más veces un carácter sin importar el que sea. Finalmente, seguido de lo anterior, escribimos un ``\.`` para seleccionar un carácter punto en específico. Posteriormente, añadimos un ``$`` seguido de este ``\.`` para indicar que queremos que este sea el fin del texto y de la línea.   
>🚨 Esta solución es la menos específica de todas las que hemos visto 🚨  

👉 **Solución más completa III: ``(\w+|\W+)\.``** → Cuando queremos hacer match sobre una palabra o bien caracteres especiales una más veces seguido de un .   

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
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado5.png?raw=true "Enunciado 5")  

👉 **Solución sencilla:** ``[A-C][anobpc]+``  

👉 **Solución más compleja I:** ``[A-C][n-p][a-c]``  

👉 **Solución más compleja II:** ``^[A-Z]..$``  

👉 **Solución más compleja III:** ``^[A-Z][n-p][a-c]$`` 

## 📚 **Exercise 6: Matching Repeated Characters** 📚
![Error, la imagen no se ha podido cargar](https://github.com/DavidBernalGonzalez/SolucionesEjerciciosBootcampJava/blob/main/1.%20Regexp/regexpone/Enunciado6.png?raw=true "Enunciado 6") 

