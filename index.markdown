---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

--- 

layout: home
title: Welcome to the Jungle  ---

# Bienvenido a mi sitio web
![Imagen de bienvenida](https://pcyti.izt.uam.mx/wp-content/uploads/2023/02/gustavo-e1676139897382.jpeg)
¡Hi! I'm Gustavo Flores, and this is my blog for my crazy stuff.

---
## Últimas Entradas del Blog

{% for post in site.posts limit:3 %} 
* [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
