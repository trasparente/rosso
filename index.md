---
---

# Rouge version {{ site.github.versions |inspect }}
{:.no_toc}
<aside class="right">
* toc
{:toc}
</aside>

{% for t in site.data.rouge %}
#### {{ t.theme }}
<div class="{{ t.theme | slugify }}">
```html
{% include html.html %}
```
{%- highlight html -%}
{% include html.html %}
{%- endhighlight -%}
~~~ html
{% include html.html %}
~~~
```sass
{% include sass.html %}
```
{%- highlight sass -%}
{% include sass.html %}
{%- endhighlight -%}
~~~ sass
{% include sass.html %}
~~~
```yml
{% include yml.html %}
```
{%- highlight yml -%}
{% include yml.html %}
{%- endhighlight -%}
~~~ yml
{% include yml.html %}
~~~
</div>
{% endfor %}