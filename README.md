# Unit testing with PHPUnit

## Story

Your task will be to write unit tests for a `Number\Integer` class
with `addition` and `subtraction` capabilities using `PHPUnit` and `TDD`.

## What are you going to learn?

- write unit tests using `PHPUnit`
- the application(s) of `Test-Driven Development`

## Tasks

1. Install `PHPUnit` using `Composer`
    - A folder named `phpunit` exists in the `vendor` directory

2. Create a class in `tests/TestInteger.php` called `TestInteger`.
    - The `TestInteger` class exists in `tests/TestInteger.php`
    - The class inherits from `PHPUnit TestCase`
    - The class has a test for the instantiation of the `Integer` class
    - The class has a test for the `value` property starting with `0`
    - The class has a new centralized instance of the `Integer` class for every test
    - The class has tests for `addition`
    - There are tests for `subtraction`
    - The class has tests for `addition and subtraction combined`

3. Create a class in `src/Integer.php` called `Integer` with namespace `Number`.
    - The `Integer` class exists in `src/Integer.php`
    - The class has the namespace `Number`
    - The class has a property called `value`
    - The `value` property has `0` as its default value
    - The class has an `add(int value)` method, which increases the value
    - The class has a `subtract(int value)` method, which decreases the value

## General requirements

- The project has to use the 3 rules of `Test-Driven Development`
- After each phase (test-implement-refactor), there should be a `new commit`

## Hints

- You can check the test suite behind the `Dish drainer` project for clarification.
- Use the following command for more detailed results:
  ```shell
  ./vendor/bin/phpunit ./tests/TestInteger.php --verbose --colors
  ```
- You can do more than just asserting equality. The list of the available methods can be found in the official documentation of `PHPUnit`, under the section `Assertions`.
- If you're using `PHP version 7.3` or below (which we don't recommend), then you should avoid `typed class properties`
- On `Codewars`, every `Kata` comes with a basic `PHPUnit` test suite, but you can write your custom tests too, under the `Sample Tests` block
  ![phpunit_on_codewars.png](media/php/unit-testing/phpunit_on_codewars.png)

## Background materials

- <i class="far fa-candy-cane"></i> [A step-by-step solution guide](project/curriculum/materials/pages/guides/unit-testing-with-phpunit--php.md)
- <i class="far fa-video"></i> [Uncle Bob on TDD](https://youtu.be/GvAzrC6-spQ)
- <i class="far fa-book-open"></i> [Uncle Bob Says: TDD](https://myoungsokang-36227.medium.com/uncle-bob-says-tdd-test-driven-development-7d5acd7f6c01)
- <i class="far fa-book-open"></i> [Introduction to PHPUnit](project/curriculum/materials/pages/php/introduction-to-phpunit.md)
- <i class="far fa-book-open"></i> [PHPUnit - PhpStorm](https://www.jetbrains.com/help/phpstorm/using-phpunit-framework.html)
- <i class="far fa-book-open"></i> [PHPUnit Assertions](https://phpunit.readthedocs.io/en/9.5/assertions.html)
- <i class="far fa-video"></i> [Unit testing with PHPUnit](https://www.youtube.com/playlist?list=PLFbnPuoQkKse0IoTKG8MZmjeu98DULDCe)
