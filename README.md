# Personal PHP Web-Development Setup

These are my minimum requirements for an elegant and easy-to-use development environment with **VS Code**.

## Editor

I am using [Visual Studio Code](https://code.visualstudio.com/) as my main editor for several months now. It's perfomance, look & feels, available plugins and features makes it the perfect every-day editor for me. The only thing I'm missing is an equivalent Symfony plugin as it exists for PHPStorm.

Coupled with the following packages it has excellent autocompletion, code-formatting and many more.

## Global **Composer** Packages

Get and install composer as described [here](https://getcomposer.org/download/).<br>
Install packages with `composer global require <package_name>`.

- `phpstan/phpstan` - _PHP Static Analysis Tool_
- `deployer/deployer` - _PHP Deployment Tool_
- `squizlabs/php_codesniffer` - _PHP Coding Standard Analysis_
- `friendsofphp/php-cs-fixer`- _PHP Coding Standard Fixer_
- `escapestudios/symfony2-coding-standard` - _Symfony PHP Coding Standard_
- `phpunit/phpunit` - _PHP Unit Testing Framework_

## Global **NPM** Packages

Get and install NodeJS as described [here](https://nodejs.org/en/). Alternatively use YARN.<br>
Install packages with `npm install -g <package_name>`.

- `prettier` - _Opinionated Code Formatter_
- `@prettier/plugin-php` (experimental) - _Prettier PHP Support_

## **VSCode** Extensions

Those can be found in the inbuilt extension manager.

### PHP

- `PHP Intelephense` - _PHP code intelligence for Visual Studio Code_
- `PHP Getters & Setters` - _Create PHP getters and setters from class properties_
- `PHP Debug` - _Debug support for PHP with XDebug_
- `phpcs` - _Use PHPCS Within Editor (eg. on-save)_
- `php cs fixer` - _Use PHPCS Fixer Within Editor_
- `PHP DocBlockr` - _Helps Writing PHPDoc_
- `vscode-phpstan` - _Use PHPStan Within Editor_
- `Twig Language 2` - _Snippets, Syntax Highlighting, Hover, and Formatting for Twig_

### Appereance

- `Nomo Dark Icon Theme` - _Icon Theme_

### Misc

- `File Utils` - _A convenient way of creating, duplicating, moving, renaming and deleting files and directories_
- `EditorConfig for VS Code` - _EditorConfig Support for Visual Studio Code_
- `DotENV` - _Support for dotenv file syntax_

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
    "workbench.colorTheme": "Atom One Dark",
    "workbench.iconTheme": "vs-nomo-dark"
}
```
