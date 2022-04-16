CSRF Security
==========================

<br>CSRF Security php, a standalone php library for csrf mitigation in web applications. Easy to integrate in any php web app. It is based on the original version [CSRF Protector PHP](https://github.com/mebjas/CSRF-Protector-PHP)

# Add to your project using packagist
 Add a `composer.json` file to your project directory
 ```json
 {
    "require": {
        "knut7/csrf-security-php": "dev-master"
    }
}
```
Then open terminal (or command prompt), move to project directory and run
```shell
composer install

## Or alternatively

php composer.phar install
```
This will add CSRFP (library will be downloaded at `./vendor/knut7/csrf-ecurity-php`) to your project directory. View [packagist.org](https://packagist.org/) for more help with composer!

# Configuration
For composer installations: Copy the config.sample.php file into your root folder at config/csrf_config.php
For non-composer installations: Copy the `libs/csrf/config.sample.php` file into `libs/csrf/config.php`
Edit config accordingly. See Detailed Information link below.

[Link to wiki - Editing Configurations & Mandatory requirements before using this library](https://github.com/knut7/CSRF-Security-PHP/wiki/Configurations)

# How to use
```php
<?php
include_once __DIR__ .'/vendor/knut7/csrf-protector-php/libs/csrf/csrfprotector.php';

// Initialise CSRFProtector library
csrfProtector::init();
```
simply include the library and call the `init()` function!

### More information 
 - [Project wiki on Github](https://github.com/knut7/CSRF-Security-PHP/wiki)

## Discussions

For any other queries contact me at: marciozebedeu@gmail.com

## How to contribute?
### General steps
 - Fork the repo
 - Create your branch
 - Commit your changes
 - Create a pull request

### More?
Well, there are various ways to contribute to this project. Find a few of them listed below:
 - Found a bug? Raise a bug in [the issue page](https://github.com/knut7/CSRF-Security-PHP/issues?q=is%3Aissue+is%3Aopen+label%3Abug). Please make sure it's not a duplicate of an existing issue.
 - Have a feature request? Raise one at [the issue page](https://github.com/knut7/CSRF-Security-PHP/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement). As mentioned above please do a basic check if this `enhancement` exists in the mentioned link.
 - Want to contribute code to this project?
   - The best way to start is by picking up one of the existing [issues with `Up For Grab` label](https://github.com/knut7/CSRF-Security-PHP/issues?q=is%3Aissue+is%3Aopen+label%3A%22Up+For+Grabs%22). 
   - Leave a comment, that you intend to help on this > then fork > and then send a pull request to `master branch`.

## FAQ:
1. What happens if token expires? - https://github.com/knut7/CSRF-Security-PHP/wiki/what-if-token-expires
2. Secure flag in a cookie? - https://github.com/knut7/CSRF-Security-PHP/issues/54
3. NoJS support? - https://github.com/knut7/CSRF-Security-PHP/tree/nojs-support

## Appendix

### JS not supported?
This version (in `master` branch) requires the clients to have Javascript enabled. However if your application can work without javascript & you require a nojs version of this library, check our nojs version
