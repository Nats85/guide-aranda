---
title: Secondary colors (Information, graphics)
styles: base/variables.scss
maturity: draft
control: exclude
colors:
  - name: $bluesec
    hex: '#2bbee0'
    rgb: rgb(43,190,224)
  - name: $purplesec
    hex: '#657d9e'
    rgb: rgb(101,125,158)
  - name: $greensec
    hex: '#42d69c'
    rgb: rgb(66,214,156)
  - name: $purplesec1
    hex: '#b3869c'
    rgb: rgb(179,134,156)
  - name: $orangesec
    hex: '#f5846f'
    rgb: rgb(245,132,111)
  - name: $orangesec1
    hex: '#e0684a'
    rgb: rgb(224,104,74)
  - name: $purplesec2
    hex: '#4e6e9c'
    rgb: rgb(78,110,156)
  - name: $greensec1
    hex: '#00a89b'
    rgb: rgb(0,168,155)
  - name: $purplesec3
    hex: '#b191bd'
    rgb: rgb(177,145,189)
  - name: $bluesec1
    hex: '#00a1c6'
    rgb: rgb(0,161,198)
  - name: $bluesec2
    hex: '#0089a8'
    rgb: rgb(0,137,168)
  - name: $purplesec4
    hex: '#7f5c8c'
    rgb: rgb(127,92,140)
  - name: $greensec2
    hex: '#077c83'
    rgb: rgb(7,124,131)
  - name: $bluesec3
    hex: '#35527a'
    rgb: rgb(53,82,122)
  - name: $orangesec2
    hex: '#f97352'
    rgb: rgb(249,115,82)
  - name: $orangesec3
    hex: '#f9957d'
    rgb: rgb(249,149,125)
  - name: $purplesec5
    hex: '#aabbdd'
    rgb: rgb(170,187,221)
  - name: $greensec3
    hex: '#8fd0b4'
    rgb: rgb(143,208,180)
  - name: $greysec
    hex: '#8899aa'
    rgb: rgb(136,153,170)
  - name: $bluesec4
    hex: '#70cbe0'
    rgb: rgb(112,203,224)


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
