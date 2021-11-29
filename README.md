# PHP Programming Notes

## Table of Contents

- [PHP in 100 Seconds](#php-in-100-seconds)

---

## PHP in 100 Seconds

| [![PHP in 100 Seconds](https://img.youtube.com/vi/a7_WFUlFS94/0.jpg)](https://www.youtube.com/watch?v=a7_WFUlFS94) |  
| - |

- PHP, a dynamic interpreted scripting language for building interactive websites on the server despite the haters  pronouncing it dead it remains one of the most popular languages for back-end web development 
- It powers content management systems like wordpress, top-tier websites like wikipedia and countless others via frameworks like laravel and symphony
- hell man even facebook uses it although they built a custom compiler to convert it to machine code on their servers 
- It was created in 1994 by rasmus lyrdorf to manage his personal home page 
- clever acronym but it sounds lame for a language that powers multi-billion dollar enterprises 
- So today we practice cognitive dissonance to tell ourselves php stands for hypertext preprocessor 
- It has a special place in history because it predates javascript and was one of the first languages to be embedded directly in html allowing websites to be built dynamically on a server 
- It's open source and was one of the technologies that revolutionized the web by making application development accessible to the average person 
- Its interpreter is implemented in c and has a syntax inspired by perl 


### Get started with PHP

- To get started create a php file "[hello.php](PHP-in-100-Seconds\hello.php)"
- Add some basic html to it
```
<html>

</html>
```
- Within this file you can go into php mode by opening a question mark php tag
```
<html>

    <?php ?>

</html>
```
- The code within these tags will be rendered on the server
- Use echo to output a value and the location of the tag 
```
<html>

    <?php echo '🐘 Cool!' ?>

</html>
```
- To declare a variable give it a name that starts with a dollar sign followed by a value
```
<html>

    <?php

        $hello = 'Hi Mom!';
        echo $hello;

    ?>

</html>
```
- It's a weekly typed language so no type annotations are necessary
- It also comes with a large number of predefined variables geared towards web development like **get**, **post** and **cookie** which contain information about the incoming http request 
```
<html>

    <?php

        $_GET['video']
        $_POST
        $_COOKIE

    ?>

</html>
```
- Now when this code 👇 is rendered on your server it will output an html string with the php tags being replaced by whatever you echoed
```
<html>

    <?php

        $hello = 'Hi Mom!';
        echo $hello;

    ?>

</html>
```
- Output:
```
$ php hello.php

<html>
    Hi Mom!
</html>
```
- The language also supports multiple programming paradigms
- You have first class functions which can be assigned to variables
```
<html>

    <?php

        $add = function ($a, $b) {
            return $a * $b;
        };

    ?>

</html>
```
- Or used anonymously as arguments
```
<html>

    <?php

        array_map(function ($a, $b) {
            return $a * $b;
        }, $arr);

    ?>

</html>
```
- And it has tons and tons of built-in functions to do pretty much anything a web developer could ever imagine doing 
- It also has a complete object model where you can define classes with inheritance to implement object-oriented patterns
```
<html>

    <?php

        class Animal {
            public $name;
            private $weight;

            public function walk() {}
        }

        $dumbo = new Animal();

    ?>

</html>
```
- We're currently on php version 8 which has all the features you would expect from a modern pragmatic language 
- Every web developer should be familiar with it because statistically there's a 78.5 chance that your client's website is running the personal homepage language.

---
