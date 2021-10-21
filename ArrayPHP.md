## Crear un array con un foreach en PHP

``` php
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
<h1>Array tabla</h1>
    <?php
    $nombres = array ("Alfonso","Jesus","Gueorgui");
    echo "<table border='2px'>";
    echo  "<tr><th>Nombres</th></tr>";
        foreach ($nombres as $value) {
            echo "<tr><td>". $value ."</td></tr>";
        }

        echo "</table>";
    ?>
    </table>
</body>
</html>
```
![arrayphp](https://user-images.githubusercontent.com/90854800/138329282-e28b0801-7f84-4b3f-b9bc-b1359d6acdae.JPG)
