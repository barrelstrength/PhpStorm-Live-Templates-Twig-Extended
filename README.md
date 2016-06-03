# PhpStorm Live Templates for Twig

A more extensive library of PhpStorm Live Templates for Twig.

## Features

PhpStorm Live Templates for Twig are a **Twig - Extended** Live Template group which adds tab-trigger support for all common Twig Tags and Functions; enables support for wrapping selections with multiple Twig tags; and adds various other utility snippets that help close tags, debug, and use your preferred tag syntax.

### Wrap Selection in Tags

    option+command+j  {{ ... }}
    option+command+j  {% ... %}
    option+command+j  {# ... #}
    option+command+j  {% block name %} ... {% endblock %}
    option+command+j  {{ dump() }}
    option+command+j  <pre>{{ dump(...) }}</pre>

### Wrap Action Tag (via tab trigger)

    b                 {% block name %} ... {% endblock %}

### Twig Tags (via tab trigger)

    at                {{  }}
    ot                {%  %}
    ct                {#  #}

    do                {% do ... %}
    extends           {% extends 'template' %}
    from              {% from 'template' import 'macro' %}
    import            {% import 'template' as name %}
    importself        {% import _self as name %}
    inc, include      {% include 'template' %}
    incp              {% include 'template' with params %}
    inckv             {% include 'template' with { key: value } %}
    use               {% use 'template' %}

    autoescape        {% autoescape 'type' %}...{% endautoescape %}
    block, blockb     {% block name %} ... {% endblock %}
    blockf            {{ block('...') }}
    embed             {% embed "template" %}...{% endembed %}
    filter, filterb   {% filter name %} ... {% endfilter %}
    macro             {% macro name(params) %}...{% endmacro %}
    set, setb         {% set var = value %}
    spaceless         {% spaceless %}...{% endspaceless %}
    verbatim          {% verbatim %}...{% endverbatim %}

    if, ifb           {% if condition %} ... {% endif %}
    ife               {% if condition %} ... {% else %} ... {% endif %}
    for               {% for item in seq %} ... {% endfor %}
    fore              {% for item in seq %} ... {% else %} ... {% endfor %}
    
    else              {% else %}
    endif             {% endif %}
    endfor            {% endfor %}
    endset            {% endset %}
    endblock          {% endblock %}
    endfilter         {% endfilter %}
    endautoescape     {% endautoescape %}
    endembed          {% endembed %}
    endfilter         {% endfilter %}
    endmacro          {% endmacro %}
    endspaceless      {% endspaceless %}
    endverbatim       {% endverbatim %}

### Debugging

    d               <pre>{{ dump() }}</pre>
    dump            {{ dump() }}

----

## Installation

Copy the XML files provided in this repository to the location where PhpStorm stores Live Templates on your operating system. The PhpStorm docs provide [instructions on installing Live Templates](https://www.jetbrains.com/help/phpstorm/10.0/live-templates.html) on OSX, Windows, and Linux.

Visit `Preferences->Editor->Live Templates` and ensure that the **Twig - Extended** Live Templates are enabled.

----

## Maintenance & Contributions

If you'd like to contribute to the **Twig - Extended** Live Templates, please consider submitting a pull request, reporting an issue, providing examples of how you would like to see the behavior of the Live Templates improved, or just sending your thoughts.

## References

- [Twig](http://www.twig-project.org/)
- [PhpStorm](https://www.jetbrains.com/phpstorm/)

