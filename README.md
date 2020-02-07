# PhpStorm Live Templates for Contao CMS

A libary of PhpStorm Live Templates for Contao CMS

## Installation

1. Go to PhpStorm Preferences | Tools | Settings Repository
2. Add Read-only Source https://github.com/pdir/phpstorm-contao-live-templates
3. Restart PhpStorm

Visit Preferences->Editor->Live Templates and ensure that the Contao CMS - Twig and Contao CMS - PHP Live Templates are enabled, as desired.

- Contao CMS - Twig.xml
- Contao CMS - PHP.xml

## Contao Templates

### DCA

#### cdtext

```php
'' => [
    'label' => &$GLOBALS['TL_LANG'][$strTable][''],
    'exclude' => true,
    'sorting' => true,
    'inputType' => 'text',
    'eval' => ['maxlength'=>255, 'tl_class'=>'w50'],
    'sql' => "varchar(255) NOT NULL default ''"
],
```

#### cdpwd

```php
'' => [
    'label' => &$GLOBALS['TL_LANG'][$strTable][''],
    'exclude' => true,
    'inputType' => 'password',
    'eval' => ['tl_class'=>'w50','mandatory'=>true, 'preserveTags'=>true, 'minlength'=>\Contao\Config::get('minPasswordLength')],
    'sql' => "varchar(128) NOT NULL default ''"
],
```

#### cdtextarea

```php
'' => [
    'label' => &$GLOBALS['TL_LANG'][$strTable][''],
    'exclude' => true,
    'search' => true,
    'inputType' => 'textarea',
    'eval' => ['rte'=>'tinyMCE', 'tl_class'=>'clr'],
    'sql' => 'text NOT NULL'
],
```

## Twig Templates

#### lorem

```php
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
```

#### Debugging

    td                 <pre>{{ dump() }}</pre>
    tdump              {{ dump() }}

## Maintenance & Contributions
If you'd like to contribute to the Contao CMS Live Templates, please consider submitting a pull request, reporting an issue, providing examples of how you would like to see the behavior of the Live Templates improved, or just sending your thoughts.

## References

- [Contao CMS](contao.org)
- [Twig](http://www.twig-project.org/)
- [PhpStorm](https://www.jetbrains.com/phpstorm/)
- [DCA Fields](https://easysolutionsit.de/artikel/vorlagen-f%C3%BCr-dca-felder.html)
