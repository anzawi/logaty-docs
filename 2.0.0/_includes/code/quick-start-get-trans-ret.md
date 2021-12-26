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

?>
```