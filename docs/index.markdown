---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default

# Just shows the latest blog posts for now.
---

## Bienvenido!
Esta es la pagina oficial de la Jaiba Rustacea. Donde encontraras recursos sobre Rust y programacion
de sistemas y uno que otro pilon de vez en cuando.

### Ultimos Posts

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>


<p class="rss-subscribe">subscribete <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
