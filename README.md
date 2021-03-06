# Magento 2 HotRod cli    [![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/dmitrijivanenko/hotrod-cli/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/dmitrijivanenko/hotrod-cli/?branch=master) [![Build Status](https://travis-ci.org/dmitrijivanenko/hotrod-cli.svg?branch=master)](https://travis-ci.org/dmitrijivanenko/hotrod-cli) [![codecov](https://codecov.io/gh/dmitrijivanenko/hotrod-cli/branch/master/graph/badge.svg)](https://codecov.io/gh/dmitrijivanenko/hotrod-cli)

This package helps you generate Magento 2 code using a clean commandline tool. All classes, templates, layouts and etc. can be dynamically generated and put together. 

## Features

- Generates different kind of magento 2 module components
- Easy to start using
- Absolutely free
- PSR2 check code command included
- Clean and fully test covered package code
- Easy to extend for your needs

## Documentation

   You'll find full documentation [here](https://dmitrijivanenko.github.io/hotrod-cli/#/).

## Example
   
   Lets review an example
   
   ``` bash
   vendor/bin/hotrod create:controller Dmiva_Test dmiva/testing/test
   ```
   
   This line tries to create a controller for the route `dmiva/testing/test` in `Dmiva_Test` namespace. Magically it
   creates for You a module `Dmiva_Test` if it is not exists, and generates files :
   
   - `app/code/Dmiva/Test/registration.php`   
   - `app/code/Dmiva/Test/etc/module.xml`   
   - `app/code/Dmiva/Test/etc/frontend/routes.xml`   
   - `app/code/Dmiva/Test/view/frontend/layout/dmiva_testing_test.xml`   
   - `app/code/Dmiva/Test/Controller/Testing/Test.php`   
   - `app/code/Dmiva/Test/Block/Testing.php`
   - `app/code/Dmiva/Test/view/frontend/templates/test.phtml`

## Installation
   
   You can install the package via composer:
   
   ``` bash
   composer require --dev dmitrijivanenko/hotrod-cli
   ```   