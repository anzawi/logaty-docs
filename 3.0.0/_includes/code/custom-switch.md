```php
foreach ( logaty()->enabled() as $lang )
{
    // Natural Language Name
    echo  "Name: " . logaty()->naturalName($lang) . "  - link: " . logaty()->link->create('', $lang);
    echo "<br>";
    // English Language Name
    echo  "Name: " . logaty()->name($lang) . "  - link: " . logaty()->link->create('', $lang);

    echo "<hr>";
}
```