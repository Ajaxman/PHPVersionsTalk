### 1.- ¿Quien soy?

| Nombre | Puesto | Empresa | ¿Qué hago? |
| :------- | :------: | :-----: |
| Javier López López | Tech Lead México | [http://www.clickbus.com.mx/](http://www.clickbus.com.mx/) |Team management, Deploys, Code Review, Git managment

| Experiencia | Me gusta | Blog |
| :------- | :------: | :-----: |
| 7 años PHP| Linux, Vim, PHP, Symfony, Redis, Scrum, Cloud Computing(Amazon), Ansible, Clean Code | [http://www.devjlopez.com/](http://www.devjlopez.com/) |

|  |
| :-------: |
| !["http://www.devjlopez.com/"](http://devjlopez.s3-us-west-1.amazonaws.com/wp-content/uploads/2015/08/18042727/Screen-Shot-2015-08-17-at-11.24.35-PM-e1439872195904.png) |

[ Next >>](#second)
<br>
***

<a name="second"></a>

<br><br>
### 2.- PHP a través del tiempo

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
| 5.6 | Expresiones en constantes, Funciones variádicas `function d($a, ...$arguments)`, se agregó el método mágico `__debugInfo()` |


[<< Previous ](#first)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[ Next >>](#third)
<br><br><br><a name="third"></a><br><br><br><br><br>
### 3.- PHP 7.0 RC


#### Features
- Release Novimebre 2015 (ya se publico el primer RC)
- Nuevo Operador combinado `<=>`
- Podremos declarar el tipo de retorno

   ```php
   <?php
  function getData(): array
  {
      return [];
  }
  ```
- Declaraciones de tipo ahora soportan tipos escalares es decir ** bool **, ** float **, ** int **, ** string **.
- Rendimiento: PHP7 esta construido sobre PHPNG(PHP Next-Gen) desarrollado por Zend logrando un aumento de rendimiento entre el 20% hasta un 70%


!["Benchmark"](http://devjlopez.s3-us-west-1.amazonaws.com/wp-content/uploads/2015/08/20045206/i%CC%81ndice-e1440046519686.png)

[<< Previous ](#second)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[ Next >>](#fourth)
<br><br><br>
***
<br><br><br>
<br><br><br>
<br><br><br>
<br><br><br>
<a name="fourth"></a>
<br><br><br>
<br><br><br>
<br><br><br>
### 4.- Uso PHP 5.3 por que es estable


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
  <br><br><br>
  <br><br><br>
  <br><br><br>
  <br><br><br>
  <br><br><br>
  <br><br><br>
  [<< Previous ](#third)
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  [ Next >>](#fifth)

***
<a name="fifth"></a>
### 5.- PHP es más que solo código

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
  <br><br><br>
  <br><br><br>
  <br><br><br>
  <br><br><br>
  <br><br><br>

  [<< Previous ](#fifth)
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  [ Next >>](#sixth)

  ***
  <a name="sixth"></a>
  ### 6.- ¿Preguntas?

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
[<< Previous ](#fifth)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[ Next >>](#seventh)
<br><br><br><br><br><br><br>
<br><br><br><br><br><br><br>
<br><br><br><br><br><br><br>
  <a name="seventh"></a>
#¡Gracias!
##¡Gracias!
###¡Gracias!
####¡Gracias!
<br>

Javier López López | twitter: [@ajaxman](http://twitter.com/ajaxman) | [http://www.devjlopez.com/](http://www.devjlopez.com/)
