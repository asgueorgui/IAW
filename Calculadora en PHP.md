## Implementacion de un calculadora con codigo PHP.
#### Calculadora en PHP con metodo GET:  
Codigo HTML para la creacion del formulario donde se registran los datos.
``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form action="calculadora1.php">
        <input type="text" name="operando1">
		<select name="operador">
			<option value="+">+
			</option>
			<option value="-">-
			</option>
			<option value="*">*
			</option>
			<option value="/">/
			</option>
		</select>
		<input type="text" name="operando2">
		<input type="submit" value="enviar">
    </form>
</body>
</html>
```
##### Codigo PHP que hace la operacion de la calculadora:
``` php
<?php
	$operando1 = $_GET['operando1'];
	$operando2 = $_GET['operando2'];
	$operador = $_GET['operador'];
	
	if($operador == "+"){
		$solucion = $operando1 + $operando2;
	}else if($operador == "-"){
		$solucion = $operando1 - $operando2;
	}else if($operador == "*"){
		$solucion = $operando1 * $operando2;
	}else if($operador == "/"){
		$solucion = $operando1 / $operando2;
	}
	echo "La solución es: ".$solucion;
?>
```
#### Calculadora en PHP con metodo POST:  
Codigo HTML para la creacion del formulario donde se registran los datos.
``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <form method="POST" action="sumar.php">
        <p>Valor 1: <input type="text" name="T1" size="20"></p>
        <p>Valor 2: <input type="text" name="T2" size="20"></p>
        <p>Valor 3: <input type="text" name="T3" size="20"></p>
        <p><input type="submit" value="Sumar" name="B1"></p>
    </form>
</body>
</html>
```
##### Codigo PHP que hace la operacion de la calculadora:
``` php
<?php
$valor1 = $_POST['T1'];
$valor2 = $_POST['T2'];
$valor3 = $_POST['T3'];

$suma = $valor1 + $valor2 + $valor3;

echo "$valor1 + $valor2 + $valor3 = $suma";
?>
```
