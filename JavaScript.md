### Codigo para meter numero y que nos diga dependiendo del numero si es pequeño, mediano, mayor.
```javascript
let numero = prompt ("Dame un numero");
if(numero < 10){
	alert("pequeño")
} else if(numero >= 10 && numero <100){
	alert("mediano")
} else {
	alert ("mayor")
}
```
### Poner un asterisco apartir de lo que me indica el usuario.
```javascript
let contador = prompt ("Cuantos asteriscos quieres");
let dibujo = "";
while (contador >= 1){
		dibujo = dibujo + "*";
    contador = contador - 1;
}
alert (dibujo)
```
### Codigo para crear una piramide de numeros..
```javascript
let contador = prompt ("Cuantos filas quieres");
let dibujo = "";
let linea = "";
while (contador >= 1){
		dibujo = dibujo + "9";
    linea = linea + dibujo + "\n";
    contador = contador - 1;
}
alert (linea)
```
### Codigo que nos muestra los numeros pares del 1 al 12
``` javascript
let contador = "0"
while(contador <=12){
		document.write(contador);
    contador = contador + 2;
}
```
