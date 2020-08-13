# rosso
Rouge synatx highlight previews

1. Get rouge themes `rougify help style`
2. Put in `_data/rouge.csv`
3. Generate css files with scss extension and `<theme slug>` as scope  
  `rougify style <theme> --scope=.<theme slug> > _sass/rouge/<theme>.scss`
4. Include css files in `assets/master.sass`  
  ```sass
  {% for t in site.data.rouge %}
  @import rouge/{{ t.theme }}
  {% endfor %}
  ```

Pygments synatx highlight previews

1. Get rouge themes from [/pygments/styles/__init__.py](https://github.com/pygments/pygments/blob/master/pygments/styles/__init__.py)
2. Put in `_data/pygments.csv`
3. Generate css files with scss extension and `<theme slug>` as scope  
  `pygmentize -f html -S <theme> -a .<theme slug> > _sass/pygments/<theme>.scss`
4. Include css files in `assets/master.sass`  
  ```sass
  {% for t in site.data.pygments %}
  @import pygments/{{ t.theme }}
  {% endfor %}
  ```