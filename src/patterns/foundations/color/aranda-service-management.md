---
title: Aranda Service Management
styles: base/variables.scss
maturity: ready
colors:
  - name: $salmon
    hex: '#f4846e'
    rgb: rgb(244,132,110)
  - name: $black
    hex: '#3c3c3b'
    rgb: rgb(60,60,59)
---
<style>
.set {
  display: flex;
  flex-wrap: wrap;
  margin: 0 -1rem;
  margin-top: 0;
  padding: 0;
  list-style: none;
}
li {
    flex: 1 0 20%;
}
.color {
  width: 100%;
  min-width: 160px;
  height: 80px;
  color: white;
  border: 1px solid whitesmoke;
  margin-bottom: 1rem;
}
p {
  margin: 0;
}
</style>
<ul class="set">
{% for item in page.colors %}
  <li>
    <div class="color" style="background:{{ item.hex }}"></div>
    <p>{{ item.name }}</p>
    {% if item.hex %}<p>{{ item.hex }}</p>{% endif %}
    {% if item.rgb %}<p>{{ item.rgb }}</p>{% endif %}
  </li>
{% endfor %}
</ul>
