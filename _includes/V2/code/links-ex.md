```html
<a href="<?php echo logaty()->link('', $language_code) ?>">My Link</a>

// real example
<a href="<?php echo logaty()->link('', 'en') ?>">this page in english language</a>
```

<br>

Generate Link to other Page with selected language 

```html
<a href="<?php echo logaty()->link('my_link') ?>">
    <?php logaty()->__("My Link")?>
</a>

// real example

<a href="<?php echo logaty()->link('/about_me') ?>">
    <?php logaty()->__("Go to About me Page in selected Language")?>
</a>
```

<br>

Generate Link to other Page with forced language 

```html
<a href="<?php echo logaty()->link('my_link', 'lang-code') ?>">
    <?php logaty()->__("My Link")?>
</a>

// real example

<a href="<?php echo logaty()->link('/about_me', 'ar') ?>">
    <?php logaty()->__("Go to About me Page in Arabic Language")?>
</a>
```