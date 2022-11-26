# Installation

## Requirements

The Laravel framework has a few system requirements. You should ensure that your web server has the following minimum PHP version and extensions:

- PHP >= 8.0
- BCMath PHP Extension
- Ctype PHP Extension
- cURL PHP Extension
- DOM PHP Extension
- Fileinfo PHP Extension
- JSON PHP Extension
- Mbstring PHP Extension
- OpenSSL PHP Extension
- PCRE PHP Extension
- PDO PHP Extension
- Tokenizer PHP Extension
- XML PHP Extension


## Setup

Setup the project
```php
composer create-project iceburgcrm/iceburgcrm
```

Edit your .env to point to your database
```php
vim .env 
```

Set permissions if needs

```php
chmod -R 775 /path/to/your/project
```

Setup the dabase
```php
php artisan migrate:fresh 
php artisan db:seed
php artisan serve
```
Visit localhost
