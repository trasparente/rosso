---
---

- <a href="{{ site.github.repository_url }}">GitHub repository</a>
- Rouge version {{ site.github.versions.rouge }}
- Jekyll version {{ site.github.versions.jekyll }}
<aside class="right">
* toc
{:toc}
</aside>

# Rouge

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
```coffee
{% include coffee.html %}
```
{%- highlight coffee -%}
{% include coffee.html %}
{%- endhighlight -%}
~~~ coffee
{% include coffee.html %}
~~~
</div>
{% endfor %}

# Pygments

{% for t in site.data.pygments %}
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
```coffee
{% include coffee.html %}
```
{%- highlight coffee -%}
{% include coffee.html %}
{%- endhighlight -%}
~~~ coffee
{% include coffee.html %}
~~~
</div>
{% endfor %}