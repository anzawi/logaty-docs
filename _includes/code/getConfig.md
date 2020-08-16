```php
<?php
    logaty()->config('file-name.option-you-need');

    // get default language
    echo logaty()->config('options.default_lang');

    // get direction for arabic language
    echo logaty()->config('direction.ar');

```

<br>


All options in (options.php) file you can retrieve value using options helper function
```php
<?php
    logaty()->options('option-you-need');

    // get default language
    echo logaty()->options('default_lang');

    // check if detecting browser language is enabled
    if( logaty()->options('detect_browser_lang')
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
     logaty()->enabled('en');

     // get english language direction return -string (rtl, ltr)-
      logaty()->direction('en');

```