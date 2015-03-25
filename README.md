# Laravel-5-Currency-Converter
Small Api for currency converting jobs in Laravel 5

# Installation
- Going your project directory on shell and run this command: composer require "senemoglu/currency"
- Add this line in your service provider's array (config/app.php) => 'Senemoglu\Currency\CurrencyServiceProvider'
- Add this line in your aliases => 'Currency' => 'Senemoglu\Currency\Facades\Converter'

# Usage

On Business Side:
Only use Currency::convert(FROM, TO, AMOUNT = 1) example: Currency::convert(USD, TRY, 20);

On Presentation Side:
Only use @currency(FROM => TO, AMOUNT) example: @currency(USD => TRY, 20)
