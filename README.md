# Personal PHP Web-Development Setup

These are my minimum requirements for an elegant and easy-to-use development environment with **VS Code**.

## Editor

I am using [Visual Studio Code](https://code.visualstudio.com/) as my main editor for several months now. It's perfomance, look & feels, available plugins and features makes it the perfect every-day editor for me. The only thing I'm missing is an equivalent Symfony plugin as it exists for PHPStorm.

Coupled with the following packages it has excellent autocompletion, code-formatting and many more.

## Global **Composer** Packages

Get and install composer as described [here](https://getcomposer.org/download/).<br>
Install packages with `composer global require <package_name>`.

* `phpstan/phpstan` - *PHP Static Analysis Tool*
* `deployer/deployer` - *PHP Deployment Tool*
* `squizlabs/php_codesniffer` - *PHP Coding Standard Analysis*
* `friendsofphp/php-cs-fixer`- *PHP Coding Standard Fixer*
* `escapestudios/symfony2-coding-standard` - *Symfony PHP Coding Standard*
* `phpunit/phpunit` - *PHP Unit Testing Framework*


## Global **NPM** Packages

Get and install NodeJS as described [here](https://nodejs.org/en/). Alternatively use YARN.<br>
Install packages with `npm install -g <package_name>`.

* `prettier` - *Opinionated Code Formatter*
* `@prettier/plugin-php` (experimental) - *Prettier PHP Support*

## **VSCode** Extensions

Those can be found in the inbuilt extension manager.

### PHP
* `PHP IntelliSense` - *Advanced PHP Autocompletion, Go-To-Definition, ...*
* `PHP Debug` - *Debug support for PHP with XDebug*
* `phpcs` - *Use PHPCS Within Editor (eg. on-save)*
* `php cs fixer` - *Use PHPCS Fixer Within Editor*
* `PHP DocBlockr` - *Helps Writing PHPDoc*
* `vscode-phpstan` - *Use PHPStan Within Editor*

### Appereance
* `Nomo Dark Icon Theme` - *Icon Theme*

## **VSCode** Settings

```JSON
{
    // PHP
    "php.suggest.basic": false,

    // PHPCS
    "phpcs.standard": "Symfony",
    "php-cs-fixer.executablePath": "php-cs-fixer",
    "php-cs-fixer.executablePathWindows": "php-cs-fixer.bat",
    "php-cs-fixer.rules": "@Symfony",

    // Code
    "files.trimTrailingWhitespace": true,
    "files.insertFinalNewline": true,

    // Appereance
    "workbench.colorTheme": "Visual Studio Dark",
    "workbench.iconTheme": "vs-nomo-dark",
}
```

