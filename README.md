# laravel-html-dom-parser
Laravel wrapper for the PHP Simple HTML DOM Parser package

## Instalation
Require this package with composer:
> composer require hungnm1518/laravel-html-dom-parser

You need to add the service provider in app.php
> HungNM\LaravelHtmlDomParser\ServiceProvider::class,

If you want to use the facade, add this to your facades in app.php
> 'HTMLDomParser' => HungNM\LaravelHtmlDomParser\Facade::class

## Usage
```php
$name = HTMLDomParser::str_get_html($html)->find('div.profile > span.name > span')[0]->plaintext;
```
## Documents
> https://simplehtmldom.sourceforge.io/docs/1.9/requirements/
