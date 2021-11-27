* {{ item.degree }} in {{ item.subject }}, {{ item.institution }}, {{ item.year_start }} {% if item.year_end %} -- {{ item.year_end }} {% else %} -- Present {% endif %}
{% if item.thesis %}
    * Thesis: {{ item.thesis.title }}
{% endif %}
{% if item.advisors %}
    {% assign advisorlist = {{item.advisors | map: "name" }} %}
    * Advisor{% if advisorlist.size > 1 %}s: {% endif %} {{ advisorlist | join: ", "}}
{% endif %}
