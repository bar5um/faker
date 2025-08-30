# Persian Faker
Persian faker package for laravel . This package is created for testing your project with fake data not for create spam. please do not use it to create spam. New options are comming soon. Enjoy it, thanks.

## PHP 8 Compatibility
This fork fixes compatibility issues with PHP 8 by removing the global `string()` helper, which caused conflicts, and replacing it with explicit `(string)` casts.

- All Faker methods (`word()`, `sentence()`, `paragraph()`, etc.) now work safely in PHP 8.
- This fork can be used directly in Laravel factories and seeders without throwing `Call to undefined function Ybazli\Faker\string()` errors.


## Installation

### Step 1

get install package with composer

```bash
composer require ybazli/faker
```

### Step 2

Next add this line in your 'config/app.php' in the providers array:

```php
Ybazli\Faker\FakerServiceProvider::class,
```
### Step 3

Next add this line in your 'config/app.php' in the aliases array:

```php
'Faker' => Ybazli\Faker\Facades\Faker::class,
```
Done :)

| Code                             | Description                                                                     |
|----------------------------------|---------------------------------------------------------------------------------|
| ``` Faker::firstName() ```       | Return a random firstname                                                       |
| ``` Faker::lastName() ```        | Return a random lastname                                                        |
| ``` Faker::fullName() ```        | Return a random fullname                                                        |
| ``` Faker::company() ```         | Return a random company name                                                    |
| ``` Faker::mobile() ```          | Return a random mobile number                                                   |
| ``` Faker::telephone() ```       | Return a random telephone number                                                |
| ``` Faker::email() ```           | Return a random email address                                                   |
| ``` Faker::domain() ```          | Return a random domain like: https://www.blablabla.ir                           |
| ``` Faker::age($min,$max) ```    | Return a random you can use $min and $max but thery are nullable                |
| ``` Faker::birthday($sign) ```   | Return a random birthday date use $sign for replace '/' between year/mounth/day |
| ``` Faker::address() ```         | Return a random postal address                                                  |
| ``` Faker::city() ```            | Return a random city of iran name                                               |
| ``` Faker::state() ```           | Return a random state of iran name                                              |
| ``` Faker::melliCode() ```       | Return a random 10 integer                                                      |
| ``` Faker::word() ```            | Return a random word                                                            |
| ``` Faker::sentence() ```        | Return a random sentence                                                        |
| ``` Faker::paragraph() ```       | Return a random paragraph                                                       |
| ``` Faker::productCategory() ``` | Return a random product category for use online shops                           |
| ``` Faker::jobTitle() ```        | return a random job title                                                       |
| ``` Faker::price() ```           | Return a random  IRR                                                            |

## License
The MIT License (MIT). Please see [License File](LICENSE) for more information.
