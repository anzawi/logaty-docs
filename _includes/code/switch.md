```php
// <ul> element
echo logaty()->switch->ul();
```
```php
// <select> element
echo logaty()->switch->select();
```
<br>
examples with output!

```php
<?php
    echo logaty()->switch->ul(); #output 1
    echo logaty()->switch->select(); #output 2
```
```html
<!-- output 1 -->
<ul class='logaty-switcher'>
    <li class='logaty-switcher__li' data-value='ar'>
         <img src='https://example.test/flags/ar.png' />
         <a href='http://example.test?lang=ar'> عربي </a>
    </li>
    <li class='logaty-switcher__li' data-value='en'>
         <img src='https://example.test/flags/en.png' />
         <a href='http://example.test?lang=en'> English </a>
    </li>
</ul>
```

```html
<!-- output 2 -->
<select id='auto-generated' class='logaty-switcher'>
    <option class='logaty-switcher__option' value='http://example.test?lang=ar'> عربي</option>
    <option class='logaty-switcher__option' value='http://example.test?lang=en'>English</option>
</select>
<script>
var select_element = document.getElementById('auto-generated');
select_element.onchange = function() {
    var elem = (typeof this.selectedIndex === "undefined" ? window.event.srcElement : this);
    var value = elem.value || elem.options[elem.selectedIndex].value;
    window.location.href = value;
}
</script>
```