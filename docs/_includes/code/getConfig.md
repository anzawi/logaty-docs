```php
<?php
    logaty()->config->get('file-name.option-you-need');

    // get default language
    echo logaty()->config->get('options.default_lang');

    // get direction for arabic language
    echo logaty()->config->get('direction.ar');

```

<br>


All options in (options.php) file you can retrieve value using options helper function
```php
<?php
    logaty()->option('option-you-need');

    // get default language
    echo logaty()->option('default_lang');

    // check if detecting browser language is enabled
    if( logaty()->option('detect_browser_lang')
    {
        echo "Yes";
    }
    else
    {
        echo "NO";
    }

```

<br>

You can get configuration using [Helpers](/helpers/)
```php
<?php
     // return -Array- All enabled languages
    logaty()->enabled();
     // check if english language is enabled return -Bool-
     logaty()->isEnabled('en');

     // get english language direction return -string (rtl, ltr)-
      logaty()->direction('en');

```