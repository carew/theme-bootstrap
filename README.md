Twitter bootstrap Theme for [Carew](http://github.com/lyrixx/Carew)
===================================================================

Installation
------------

Install it with composer:

```
composer require lyrixx/carew-theme-bootstrap:dev-master
```

Then configure `config.yml`

```
engine:
    theme_path: %dir%/vendor/carew/theme-bootstrap
```

Customisation
-------------

You can customize all templates.

Create a new template in your `layouts` directory with the same
name as the original one.

You can also inherit original template with `extends`:

```
# my_project/layouts/default.html.twig
{% extends 'vendor/lyrixx/carew-theme-bootstrap/layouts/default.html.twig'%}

{% block nav_right %}
    <ul class="nav pull-right">
        <li class="dropdown">
            ...
        </li>
    </ul>
{% endblock %}
```
