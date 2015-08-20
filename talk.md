### ¿Quien soy?

| Nombre | Puesto | Empresa | Que hago |
| :------- | :------: | :-----: |
| Javier López López   | Tech Lead México | Clickbus (rocket-internet.de)|Team management, Deploys, Code Review, Git managment

| Experiencia | Me gusta | Blog
| :------- | :------: | :-----:
| 7 años PHP| Linux, Vim, PHP, Symfony, Redis, Scrum, Cloud Computing(Amazon), Ansible, Clean Code | [http://www.devjlopez.com/](http://www.devjlopez.com/) |

|  |
| :-------: |
| !["http://www.devjlopez.com/"](http://devjlopez.s3-us-west-1.amazonaws.com/wp-content/uploads/2015/08/18042727/Screen-Shot-2015-08-17-at-11.24.35-PM-e1439872195904.png) |

[Second Slide >>](#second)
<br>
***

<a name="second"></a>

<br><br>
### PHP a traves del tiempo


## Historia de PHP

| Versión | Comentarios |
| :--- | :--- |
| 1.0 | Primera versión lanzada por Rasmus Lerdorf Personal Home Page Tools (PHP Tools) |
| 2.0 | Soporte para DBM, mSQL, y bases de datos Postgres95, Cookies, se llamó PHP/FI  |
| 3.0 | Zeev Suraski y Andi Gutmans, reescriben PHP  |
| 4.0 | PHP ahora incorpora el motor Zend  |
| 5.0 | Zend Engine 2.0 mejora notable en orientación a objetos |

## El nuevo PHP

| Versión | Comentarios |
| :--- | :--- |
| 5.3 | namespaces, funciones anonimas,  soporte para archivos PHAR, mysqlnd  |
| 5.4 | Soporte para traits, sintaxis abreviada para arrays ([]), se removieron register_globals, servidor web incorporado  |
| 5.5 | empty() ahora soporta expresiones, se agregaron generadores (yield), se agregó finally a los bloques * try-catch *, nueva Api para hash de contraseñas(ahora es mas fácil con password_hash())  |
| 5.6 | Expresiones en constantes, Funciones variádicas `function d($a, ...$arguments)`, se agregó el método mágico __debugInfo() |


[<< Second Slide](#second)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[Third Slide>>](#third)
***
<a name="third"></a>
### PHP 7.0 RC


#### Features
- Release Novimebre 2015 (ya se publico el primer RC)
- Nuevo Operador combinado `<=>`
- Podremos declarar el tipo de retorno

   ```php
   function getData(): array
  {
      return [];
  }
  ```
- Declaraciones de tipo ahora soportan tipos escalares es decir ** bool **, ** float **, ** int **, ** string **.
- Rendimiento: PHP7 esta construido sobre PHPNG(PHP Next-Gen) desarrollado por Zend logrando un aumento de rendimiento entre el 20% hasta un 70%



[<< Third Slide](#third)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[Fourth Slide>>](#third)

***
<a name="third"></a>
### Uso PHP 5.3 por que es estable


#### Estable?
- Release: 30 Junio 2009
- Soporte hasta 14 Agosto 2014
- PHP 5.3 es (muy) viejo 6 años
- PHP 5.5 tambien es viejo Release: 20 Junio 2013
- PHP 5.6 minimo
  - Rapidez
  - Features muy interesantes
  - Soporte hasta Agosto 2017
  - Es mejor estar preparado para el salto a PHP 7.0

[<< Third Slide](#third)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[Fourth Slide>>](#third)

***
<a name="third"></a>
### PHP es más que solo código

#### Comunidad
- PHP-FIG [http://www.php-fig.org/](http://www.php-fig.org/)
  - Integrantes de muchos frameworks (Symfony, Phalcon, CakePHP, Composer, Doctrine, Drupal, Guzzle, Laravel, Zend Framework, etc.)
- PHP Standard Recommendations: PSR
  - PSR-0: Autoloading Standard
  - PSR-1: Basic Coding Standard
  - PSR-2: Coding Style Guide
  - PSR-3: Logger Interface
  - PSR-4: Autoloading Standard
  - PSR-7: HTTP Message Interface
- Packagist:
  - The PHP Package Repository
- PHP la forma correcta:
  - [http://www.phptherightway.com/](http://www.phptherightway.com/)


  [<< Third Slide](#third)
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  [Fourth Slide>>](#third)

  ***
  <a name="third"></a>
  ### ¿Preguntas?


```php
<?php
namespace Jlopez\Talk;

/**
 * Class Questions
 * @package Jlopez\Talk
 */
class Questions
{

    /**
     * @var string
     */
    private $question;

    public function __construct(string $question)
    {
        $this->question = $question;
    }

    /**
     * @return array
     */
    public function __debugInfo()
    {
        return [
            'question' => $this->question,
        ];
    }

}

$talk = new Questions('...');
var_dump($talk);
/*
object(Questions)#1 (1) {
  ["question"]=>
  string('...')
}*/
```
