**How to Use :**

```php
<?php
    echo logaty()->detect('country');
    // return browser language code-2-digits

```

for example if country language is arabic the method will be return (ar),
and if country language is english the method will be return (en).
if detected language is not enabled in your website the method will be return (website default language). 

<br>

```php
<?php
    $browserLanguage = logaty()->detect('country');

    if($browserLanguage != logaty()->current())
    {
        showModal([
            'type'     => 'country',
            'language' => $browserLanguage,
        ]);
    }

    // showModal function
    function showModal($options = [])
    {
        if(!isset($_SESSION['detect']))
        {
            $_SESSION['detect'] = true;
            // show modal or message box or do what you want
        }
    }

        
```