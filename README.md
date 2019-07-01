# PhpStorm Live Templates for Twig

A more extensive library of PhpStorm Live Templates for Twig.

## Features

The **Twig - Extended** Live Templates add tab-trigger support for common Twig Tags; enable support for wrapping selections with multiple Twig tags; and add various other utility snippets that help close tags, debug, and use your preferred tag syntax.

## Installation

1. Go to *PhpStorm Preferences | Tools | Settings Repository*

2. Add Read-only Source https://github.com/barrelstrength/PhpStorm-Live-Templates-Twig-Extended

3. Restart PhpStorm

### Wrap Selection in Tags

PhpStorm's `Code->Surround With...` and `Code->Surround With Live Template...` options allow you to select text that is already in your template and wrap it within tags dynamically. The **Twig-Extended** Live Templates enable the following tags to be wrapped around selections:

    option+command+j  {{ ... }}
    option+command+j  {% ... %}
    option+command+j  {# ... #}
    option+command+j  {% block name %} ... {% endblock %}
    option+command+j  {{ dump(...) }}
    option+command+j  <pre>{{ dump(...) }}</pre>

### Wrap Action Tag (via tab trigger)

The `b` tab trigger provides a flexible way to create a generic Twig action tag. By default, `b` tab trigger expands to a `block` tag, however you can immediately overwrite the `block` keyword with any keyword of your choice.

    b                 {% block name %} ... {% endblock %}

### Twig Tags (via tab trigger)

The following keywords expand to their respective code constructs when used as tab-triggers.

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
    incpo             {% include 'template' with params only %}
    inckv             {% include 'template' with { key: value } %}
    inckvo            {% include 'template' with { key: value } only %}
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
    
    rl                {% requireLogin %}

_While there are not really enough keywords to make some of these conventions very meaningful, if curious: Keywords that end in the letter `b` output a block version of the tag. Keywords that end in the letter `p` output a version of the tag with parameters._

### Debugging

    d                 <pre>{{ dump() }}</pre>
    dump              {{ dump() }}

----

### Live Template group configuration files

- Twig - Extended.xml

Visit `Preferences->Editor->Live Templates` and ensure that the **Twig - Extended** Live Templates are enabled.

----

## Maintenance & Contributions

If you'd like to contribute to the **Twig - Extended** Live Templates, please consider submitting a pull request, reporting an issue, providing examples of how you would like to see the behavior of the Live Templates improved, or just sending your thoughts.

## References

- [Twig](http://www.twig-project.org/)
- [PhpStorm](https://www.jetbrains.com/phpstorm/)
- [PhpStorm Live Templates for Craft CMS](https://github.com/BarrelStrength/PhpStorm-Live-Templates-Craft-CMS) - A library of PhpStorm Live Templates for Craft CMS, including several additional snippets for Craft Twig variables.

