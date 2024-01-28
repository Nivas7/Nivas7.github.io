---
layout: default
title: nivaz's blog
---

<h2 class="mono">hi, i am srinivas.</h2>
I  create stuff using programming.

### interests:

- deep learning
- Web development
- 3D Modeling
  {: class="mono"}

view [[online resume]][2]{: class="noline"}

while you are here you can checkout my useful programs list [WIP]\\
or [my reading list][1]{: class="noline"}

## recent posts:

<ul class="mono">
{% for post in site.posts limit:5 %}
	{% if post.url contains 'random' %}
		<li><a class="noline" href="{{ post.url }}">[r] {{ post.title | downcase }}</a></li>
	{% elsif post.url contains 'cooking' %}
		<li><a class="noline" href="{{ post.url }}">[c] {{ post.title | downcase }}</a></li>
	{% else %}
		<li><a class="noline" href="{{ post.url }}">{{ post.title | downcase }}</a></li>
	{% endif %}
	
{% endfor %}
<a class="noline" href="/blog">see more..</a>
</ul>

[1]: /books
[2]: /resume/index.html
