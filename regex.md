## REGEX
### Debe empezar con...
```
^ 
```
### Debe finalizar con...
```
$ 
```
### Inicia con b y termina con b 
```
^b$
```
### Se encuentra git en la frase?
```
Git\b
```
### Tiene muchas "a" y termina en a
```
^a*$
```
###  Por lo menos debe venir una a
```
^a+
```
### Podria venir una "e" solo una vez
```
^e? 
```

## CUANTIFICADOR
### Que venga los digitos una vez
```
^[1-9]{1} 
```
### Que venga los digitos una vez o 7 veces
```
^[1-9]{1,7}
```
## CUANTIFICADOR CODICIOSO
### Evaluar uno a uno globalmente
```
^<beer>.*?<\/beer>g 
```
## CLASES DE CARACTERES
### Debe venir uno o muchos digitos
```
^\d+$
```
### Debe venir un texto menos un numero
```
^\D+$
```
### Alfanumerico
```
^[A-Za-z0-9_]+$
```
### Detecta cadena alfanumerica
```
^\w+$
```
### Caracter espacio
```
^\s+
```
## GRUPOS Y RANGOS
### Compuerta OR
```
^cerveza|vino$
```
### Tiene alfanumerico o espacio
```
^(\w|\s)+(cerveza|vino)$
```
## ASERCIONES AVANZADAS
### Debe preceder con Vino
```
Vino(=?\s\w+)
```
### Debe preceder con Vino globalmente
```
Vino(=?\s\w+)g
```
### Usando OR
```
(Vino|Cerveza)(=?\s\w+)g
```
### Asercion negativa, [no debe ser 8 y 9]
```
Java\s(?!8|9)
```