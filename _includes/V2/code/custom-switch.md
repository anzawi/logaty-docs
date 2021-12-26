```php
foreach ( logaty()->enabled() as $lang )
{
    // Natural Language Name
    echo  "Name: " . logaty()->nameN($lang) . "  - link: " . logaty()->link('', $lang);
    echo "<br>";
    // English Language Name
    echo  "Name: " . logaty()->name($lang) . "  - link: " . logaty()->link('', $lang);

    echo "<hr>";
}
```