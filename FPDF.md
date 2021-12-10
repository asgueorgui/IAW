### Crear un fichero pdf desde PHP, descargando la libreria de FPDF, de su pagina oficial
```php
<?php
require('fpdf.php');

$pdf = new FPDF();
$pdf->AddPage();
$pdf->SetFont('Arial','B',16);
$pdf->Cell(40,10,'Muy buenas!');
$pdf->Cell(100,40,'Gueorgui');
$pdf->Output();
?>
```
