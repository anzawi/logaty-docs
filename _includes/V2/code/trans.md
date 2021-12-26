to return to our example
```php
<?php
    // as selected language
    /* 1 */ echo logaty('home.welcome');
    /* 2 */ echo logaty()->_x('home.welcome');
    /* 3 echo directly */ logaty()->__('home.welcome');

    // as given language parameter
    /* 1 */ echo logaty('home.welcome', 'en');
    /* 2 */ echo logaty()->_x('home.welcome', 'ar');
    /* 3 echo directly */ logaty()->__('home.welcome', 'en');

```
<br>
output well be as selected language if second parameter not set.

```php
<?php
    echo logaty('home.welcome');
    /** Output :
        * if selected language is (arabic) : مرحبا بك في الصفحة الرئيسية للغاتي.
        * if selected language is English  : Welcome to Logaty Home Page.
    */

    /** --------------- Force Translation Language ---------------- */
     echo logaty('home.welcome', 'en');
    /** Output :
        * if selected language is (arabic) :  Welcome to Logaty Home Page.
        * if selected language is English  : Welcome to Logaty Home Page.
    */

            
```