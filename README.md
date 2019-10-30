# Personal PHP Web-Development Setup

These are my minimum requirements for an elegant and easy-to-use development environment with **VS Code**.

## Editor

I am using [Visual Studio Code](https://code.visualstudio.com/) as my main editor for several months now. It's perfomance, look & feels, available plugins and features makes it the perfect every-day editor for me. The only thing I'm missing is an equivalent Symfony plugin as it exists for PHPStorm.

Coupled with the following packages it has excellent autocompletion, code-formatting and many more.

## Global **Composer** Packages

Get and install composer as described [here](https://getcomposer.org/download/).<br>
Install packages with `composer global require <package_name>`.

- [`phpstan/phpstan`](https://github.com/phpstan/phpstan) - _PHP Static Analysis Tool_
- [`deployer/deployer`](https://github.com/deployphp/deployer) - _PHP Deployment Tool_
- [`squizlabs/php_codesniffer`](https://github.com/squizlabs/PHP_CodeSniffer) - _PHP Coding Standard Analysis_
- [`phpunit/phpunit`](https://github.com/sebastianbergmann/phpunit) - _PHP Unit Testing Framework_

## Global **NPM** Packages

Get and install NodeJS as described [here](https://nodejs.org/en/). Alternatively use YARN.<br>
Install packages with `npm install -g <package_name>`.

- [`eslint`](https://github.com/eslint/eslint) - _A fully pluggable tool for identifying and reporting on patterns in JavaScript_
- [`prettier`](https://github.com/prettier/prettier) - _Opinionated Code Formatter_
- [`@prettier/plugin-php`](https://github.com/prettier/plugin-php) - _Prettier PHP Support_

## **VSCode** Extensions

Those can be found in the inbuilt extension manager.

### PHP

- [`PHP Debug`](https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-debug) - _Debug support for PHP with XDebug_
- [`PHP DocBlockr`](https://marketplace.visualstudio.com/items?itemName=neilbrayfield.php-docblocker) - _Helps Writing PHPDoc_
- [`PHP Getters & Setters`](https://marketplace.visualstudio.com/items?itemName=phproberto.vscode-php-getters-setters) - _Create PHP getters and setters from class properties_
- [`PHP Intelephense`](https://marketplace.visualstudio.com/items?itemName=bmewburn.vscode-intelephense-client) - _PHP code intelligence for Visual Studio Code_
- [`PHP Static Analysis`](https://marketplace.visualstudio.com/items?itemName=breezelin.phpstan) - _Static analysis support for PHP with PhpStan_
- [`phpcs`](https://marketplace.visualstudio.com/items?itemName=ikappas.phpcs) - _Static analysis support for PHP with PhpStan_
- [`Twig`](https://marketplace.visualstudio.com/items?itemName=whatwedo.twig) - _Syntax highlighting for PHP Twig_

### JavaScript/ECMAScript

- [`ESLint`](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - _Integrates ESLint JavaScript into VS Code_
- [`Vetur`](https://marketplace.visualstudio.com/items?itemName=octref.vetur) - _Vue tooling for VS Code_

### Appereance

- [`Nomo Dark Icon Theme`](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-icontheme-nomo-dark) - _Icon Theme_
- [`Paper-tmTheme`](https://marketplace.visualstudio.com/items?itemName=DiryoX.Paper-tmTheme) - _Color Scheme_

### Misc

- [`Beautify`](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify) - _Beautify code in place for VS Code_
- [`Bracket Pair Colorizer 2`](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2) - _A customizable extension for colorizing matching brackets_
- [`DotENV`](https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv) - _Support for dotenv file syntax_
- [`EditorConfig for VS Code`](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig) - _EditorConfig Support for Visual Studio Code_
- [`Prettier - Code formatter`](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - _VS Code plugin for prettier/prettier_
- [`Project Manager`](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager) - _Easily switch between projects_

## **Font**

There are a variety of fonts which come down to personal preference. The ones I use the most are:

- [`Hack`](https://github.com/source-foundry/Hack) - _A typeface designed for source code_
- [`Fira Code`](https://github.com/tonsky/FiraCode) - _Monospaced font with programming ligatures_

## **VSCode** Settings

```JSON
{
    "explorer.openEditors.visible": 0,
    "git.autofetch": true,

    // Editor
    "editor.fontLigatures": true, // needed if using Fira Code
    "editor.fontFamily": "'Hack', monospace",
    "editor.fontSize": 13,
    "editor.formatOnSave": true,
    "editor.wordWrapColumn": 120,

    // Workbench
    "workbench.colorTheme": "Paper Dark",
    "workbench.editor.enablePreview": false,
    "workbench.iconTheme": "vs-nomo-dark",

    // Project Manager
    "projectManager.git.baseFolders": [
        "C:\\Users\\<USERNAME>\\Development" // whatever your path is
    ],
    "projectManager.git.ignoredFolders": [
        "node_modules",
        "out",
        "build",
        "typings",
        "test",
        ".haxelib",
        "vendor"
    ],

    // PHP
    "intelephense.licenceKey": "YOUR-LICENSE-KEY", // comment if you don't have one
    "phpcs.executablePath": "C:\\Users\\<USERNAME>\\AppData\\Roaming\\Composer\\vendor\\bin\\phpcs.bat", // This is on windows

    // Formatting
    "eslint.autoFixOnSave": true,
    "beautify.language": {
        "html": [
            "html",
            "vue"
        ],
        "css": [],
        "js": []
    }
}
```
