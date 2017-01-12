# RFC Register

### Previously Closed RFCS

{% for page in site.decisions %}
  <h3><a title="{{ page.title }}" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></h3>
  <p>{{page.excerpt}}</p>
{% endfor %}