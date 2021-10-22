### Implementacion del bucle for en PHP.
for(start, condition, incremental)  
En este caso el start es el numero 1, la condicion es donde para de contar, incremental cuenta de 1 en 1.
##### Bucle que cuenta del 0 al 9 de 2 en 2 (Solo saca 02468)
``` php
<?php
    for ($counter=0; $counter < 10; $counter = $counter+2)
    {
        echo $counter;
    }
?>
```
##### Bucle que cuenta del 0 al 9 de 1 en 1 (0123456789)
``` php
<?php
    for ($counter=0; $counter < 10; $counter++)
    {
        echo $counter;
    }
?>
```
