# rosso
Rouge previews

1. Get rouge themes `rougify help style`
2. Put in `_data/rouge.csv`
3. Generate css files with scss extension and `<theme slug>` as scope  
  `rougify style <theme> --scope=.<theme slug> > _sass/<theme>.scss`
4. Include css files in `master.sass`  
  ```liquid
  {% for t in site.data.rouge %}
  @import {{ t.theme }}
  {% endfor %}
  ```