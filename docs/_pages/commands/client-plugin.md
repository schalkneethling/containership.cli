---
command-name: 'client-plugin'
permalink: '/docs/commands/client-plugin'
---

<h2> Overview </h2>

The `{{ page.command-name }}` command is responsible for listing, showing, and manipulating both core plugins on your cluster and extensible CLI plugins.

<h2> Commands </h2>

<p>
{% for item in site.data.navigation.docs %}
    {% if item.title == 'Commands' %}
        <ul>
        {% for link in item.children %}
            {% if link.title contains page.command-name and link.title != page.command-name %}
                <li><a href="{{site.baseurl}}{{link.url}}">{{link.title}}</a></li>
            {% endif %}
        {% endfor %}
        </ul>
    {% endif %}
{% endfor %}
</p>