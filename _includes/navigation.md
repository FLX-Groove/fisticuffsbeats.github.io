<nav id="primary-navigation">
  <ul>
 {% for node in site.pages %}
    {% if node.navigation == 'main' %}
      {% if page.url == node.url %}
        <li class="current"><a href="{{node.url}}">{{node.title}}</a></li>
      {% else %}
        <li><a href="{{node.url}}">{{node.title}}</a></li>
      {% endif %}
    {% endif %}
  {% endfor %}
</ul>
</nav>