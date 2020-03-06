---
title: Secondary colors (Status)
styles: base/variables.scss
maturity: draft
control: exclude
colors:
  - name: $redsec
    hex: '#ee3557'
    rgb: rgb(238,53,87)
  - name: $greensec4
    hex: '#38b55e'
    rgb: rgb(56,181,94)
  - name: $yellowsec
    hex: '#fdc164'
    rgb: rgb(253,193,100)
  - name: $orangesec4
    hex: '#f7931d'
    rgb: rgb(112,203,224)
  - name: $bluesec5
    hex: '#27a9e1'
    rgb: rgb(37,169,225)
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
  margin: 1rem;
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
