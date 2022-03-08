------

Hi 2\! \- index
===

{% assign doclist = site.pages | sort: 'url' %}

{% for doc in doclist %}
    {% if doc.name contains '.md' or doc.name contains '.html' or doc.name contains '/' %}
* [{{ doc.url }}]({{ site.baseurl }}{{ doc.url }})
    {% endif %}
{% endfor %}
