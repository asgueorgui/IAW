## Una empresa tiene el problema que quiere monitorizar sus servidores web de cara a las aplicaciones internas que usan, el problema es que sólo el administrador de sistemas tiene acceso a la máquina y nos piden que cualquier técnico pueda realizar un chequeo de los logs del sistema. Para ello nos piden una aplicación que detecte problemas en los logs típicos, que puedan visualizar logs del sistema y lanzar scripts de mantenimiento dentro del servidor.
### Fichero log de apache en un textarea.
``` php
<?php
    $fichero = fopen("C:\\xampp\\apache\\logs\\error.log","r");
    echo "<textarea>";
    while (!feof($fichero))
    {
        $linea = fgets($fichero);
        echo $linea;
        echo "<br>";
    }
    fclose ($fichero);
    echo "</textarea>";
?>
```
### Encontrar una palabra o letra en una cadena de texto como es un string.
``` php
<?php
    $mystring = "Me encantan las abichuelas, si nena";
    $findeme = "si";
$pos = strpos($mystring, $findeme);

    if($pos === false) 
    {
        echo "La cadena '$findeme' no fue encontrada en la cadena '$mystring'";
    }
    else 
    {
        echo "La cadena '$findeme' fue encontrada en la cadena '$mystring'";
        echo " y existe en la posición $pos";
    }
?>
```
