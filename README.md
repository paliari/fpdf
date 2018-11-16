# fpdf
FPDF is a PHP class which allows to generate PDF files with pure PHP. F from FPDF stands for Free: you may use it for any kind of usage and modify it to suit your needs. http://www.fpdf.org


## Installation

```bash
composer require paliari/fpdf

```


## Usage

```php
<?php
require __DIR__ . '/vendor/autoload.php';


$pdf = new \Fpdf\Fpdf();
$pdf->setFont('Arial');
$pdf->addPage();
$pdf->cell(190, 10, 'Batata frita', 1);

/**
* I: send the file inline to the browser.
* D: download.
* F: save to a local file with the name.
* S: return the document as a string.
*/
$pdf->output('I');


```
