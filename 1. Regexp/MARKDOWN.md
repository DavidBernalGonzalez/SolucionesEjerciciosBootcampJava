# Soluciones de ejercicios de expresiones regulares (REGEXP)
## 1. Ejercicios de https://regexone.com/  

 **1.1 -  Matching Characters:**

- **Solución simple/sencilla: `` regex abc ``** → cuando queremos que sea literalmente abc  
- **Solución "más compleja" I: ``^abc.*``**  → cuando queremos que empiece por abc y luego lo que sea utilizando la estrella de kleene
-  **Solución más compleja II: ``^abc.{0,}``** → cuando queremos que empiece por abc y luego tenga 0 o más (por tanto, equivalente a la anterior solución)  

 **1.½ -  Matching Characters:**
- **Solución sencilla:	`` 123 ``** → cuando queremos que sea literalmente 123  
- **Solución más compleja I: `` \d+``**	 → cuando queremos que coja todos los dígitos independientemente de la cantidadç
- **Solución más compleja II: ``\d{3}	``** → cuando queremos que coja solamente los grupos de 3 dígitos
- **Solución más compleja III: ``\d{3,} ``** → cuando queremos que coja solamente los grupos de 3 dígitos o más dígitos (equivalente a solución II)