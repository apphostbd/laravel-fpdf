# laravel-fpdf

<p align="center">
     <a href="https://github.com/apphostbd/laravel-fpdf/tags" alt="tag">
        <img src="https://img.shields.io/github/v/tag/apphostbd/laravel-fpdf" alt="tag"/>
      </a> 
     <a href="https://packagist.org/packages/apphostbd/laravel-fpdf" alt="Total Downloads">
        <img src="https://img.shields.io/packagist/dt/apphostbd/laravel-fpdf" alt="Total Downloads"/>
      </a> 
     <a href="https://github.com/apphostbd/laravel-fpdf/issues" alt="Issues">
        <img src="https://img.shields.io/github/issues/apphostbd/laravel-fpdf" alt="Issues"/>
      </a>  
     <a href="https://github.com/apphostbd/laravel-fpdf/fork" alt="Forks">
        <img src="https://img.shields.io/github/forks/apphostbd/laravel-fpdf"  alt="Forks"/>
      </a>  
     <a href="https://github.com/apphostbd/laravel-fpdf/stargazers" alt="Stars">
        <img src="https://img.shields.io/github/stars/apphostbd/laravel-fpdf"  alt="Stars"/>
      </a>  
     <a href="https://github.com/apphostbd/laravel-fpdf/blob/master/LICENSE" alt="License">
        <img src="https://img.shields.io/github/license/apphostbd/laravel-fpdf" />
      </a>       
</p>


FPDF is a PHP class which allows to generate PDF files with pure PHP, that is to say without using the PDFlib library. F from FPDF stands for Free: you may use it for any kind of usage and modify it to suit your needs.

## Installation Composer
```sh
  composer require apphostbd/laravel-fpdf
```
### Laravel >= 5.5
Enjoy the auto discovery feature. 

### Laravel <5.5
`config/app.php`

```php

// config/app.php

return [
    'aliases' => [
        'Fpdf' => AppHostBD\Fpdf\Facades\FpdfFacade::class,
     ]

```

## Basic example
     ## Route Page example
          ```php
               Route::get('/', function () {
                   Fpdf::AddPage();
                   Fpdf::SetFont('Courier', 'B', 18);
                   Fpdf::Cell(50, 25, 'Hello World!');
                   Fpdf::Output();
                   exit();
               });

          ```




