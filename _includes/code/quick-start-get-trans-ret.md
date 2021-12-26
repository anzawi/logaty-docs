```php
<?php
    // as selected language
    /* 1 */ echo logaty()->_x('home.welcome');
    /* 2 echo directly */ logaty()->__('home.welcome');

    // as given language parameter
    /* 1 */ echo logaty()->_x('home.welcome', 'ar');
    /* 2 echo directly */ logaty()->__('home.welcome', 'en');

?>
```