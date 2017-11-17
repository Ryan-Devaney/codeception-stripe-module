# Codeception Stripe Module

[![Latest Stable Version](https://poser.pugx.org/portrino/codeception-stripe-module/v/stable)](https://packagist.org/packages/portrino/codeception-stripe-module)
[![Total Downloads](https://poser.pugx.org/portrino/codeception-stripe-module/downloads)](https://packagist.org/packages/portrino/codeception-stripe-module)

## Installation

You need to add the repository into your composer.json file

```bash
composer require --dev portrino/codeception-stripe-module
```

## Configuration

```yml
modules:
    enabled:
        - Asserts
        - Stripe:
            depends: Asserts
            api_key: 'sk_test_IGvdODXxy1xXFviyAjWMiK5q'
            api_version: '2017-08-15'
 ```  
 
Update codeception build
   
```bash
codecept build
```

### Methods

#### seeCustomerWithStripeId($table)

```php
  $I->seeCustomerWithId($id);
```

#### grabCustomerByStripeCustomerId($table)

```php
  $customer = $I->grabCustomerById($id);
```

## Authors

![](https://avatars0.githubusercontent.com/u/726519?s=40&v=4)

* **André Wuttig** - *Initial work* - [aWuttig](https://github.com/aWuttig)

See also the list of [contributors](https://github.com/portrino/codeception-stripe-module/graphs/contributors) who participated in this project.
