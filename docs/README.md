# RFC Register

Here's all of your teams RFCs neatly formatted into a page. Edit
this to add any content you think makes this easy for managers
to understand.

### Decisions

{% for page in site.decisions %}
  * [{{page.title}}]({{page.url}})
{% endfor %}