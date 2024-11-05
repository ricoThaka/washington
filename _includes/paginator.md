
<!--
<ul>
  {% for post in site.posts %}
      <li>
      <div class="featured-post" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}>
      <h2><a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">{{ post.title }}</a></h2>
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time>
      <p>{{ post.content | strip_html | truncatewords:50 }}</p>
      </li>
  {% endfor %}
</ul>
-->

<article>
  <a href="{{ site.github.url }}{{ post.url }}">
    <div class="featured-post" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}>
      <h2><span>{{ post.title }}</span></h2>
    </div>
  </a>
</article>