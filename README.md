# mynotepaper

composer require mynotepaper/greeter

routes\web.php
use Mynotepaper\Greeter\Greet;

Route::get('/greet/{name}', function ($name) {
    $greet = new Greet();

    return $greet->greet($name);
});

http://localhost:8000/greet/{name}
