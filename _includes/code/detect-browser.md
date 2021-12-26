**How to Use :**

```php
<?php
    echo logaty()->detect->browser();
    // return browser language code-2-digits
   
```
<br>
for example if browser language is arabic the method will be return (ar),
and if browser language is english the method will be return (en). 

```php
<?php
    $browserLanguage = logaty()->detect->browser;

    if($browserLanguage != logaty()->current())
    {
        showModal([
            'type'     => 'browser',
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