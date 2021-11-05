## Conexion en php a la base de datos MySQL
### Codigo html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="redes.css">
    <title>Document</title>
</head>
<body>
    <form action="redes.php" method="post">
        <div class="container">
        
            <div class="brand-logo"></div>
        <div class="brand-title">GAS Social Media</div>
        <div class="inputs">
            <label>Nombre</label>
            <input type="text" name="nombre" placeholder="usuario o e-mail" />
            <label>PASSWORD</label>
            <input type="password" name="password" placeholder="Escribe tu contraseña" />
            <button type="submit"  formmethod="post">LOGIN</button>
        </div>
    </form>
</body>
</html>
  ```
### Codigo php
  ```php
  <?php
    $db = new mysqli("localhost","root","","iaw");

    $sql = "SELECT * from usuarios;";
    $result = $db->query($sql);
    $encontrado = false;

    while($row = $result->fetch_assoc()){
        echo "la contraseña de <b>: {$row['Nombre']} </b> es: {$row['Password']} </br>";
        if ($usuario == $row['Nombre'] && $password == $row['Password']){
            $encontrado = true;
        }
    }
    $result->close();
    $db->close();
?>
```
