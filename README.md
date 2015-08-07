I18n Routing Service Provider  [![Build Status](https://secure.travis-ci.org/jenyak/I18nRoutingServiceProvider.png)](http://travis-ci.org/jenyak/I18nRoutingServiceProvider)
=============================

Silex i18n routing service provider inspired by [JMSI18nRoutingBundle](https://github.com/schmittjoh/JMSI18nRoutingBundle)

Installation
------------

Recommended installation is [through composer](http://getcomposer.org). Just add
the following to your `composer.json` file:

    {
        "require": {
            "nicl/silex-autolink": "1.0.*"
        }
    }

# Parameters

* **i18n_routing.translation_domain**: Translation message domain. The default value is `routes`.
* **i18n_routing.locales**: Routing locales. The default value is `array(en)`.
* **locale**: Uses as default routing locale. The default value is `en`.

# Usage

Registering

```php
$app->register(new Jenyak\I18nRouting\Provider\I18nRoutingServiceProvider());
```

Setup your routing locales:
```php
$app['i18n_routing.locales'] = ['en', 'ua'];
```

