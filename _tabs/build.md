---
icon: fas fa-toolbox
order: 3
---

<p> Team Optix 3749 Build Blog Posts </p>

{% if site.categories.build.size > 0 %}

  {% for post in site.posts %}

    {% if post.categories contains "build" and post.hide != true %}

      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>

    {% endif %}

  {% endfor %}

{% else %}

  <blockquote>This department doesn't have any blog posts yet 😔</blockquote>

{% endif %}

<h4>Team Members:</h4>
<table style="text-align: center;">
  <tr id="table">

  </tr>
</table>

<script>

  var data = ["Adrita C", "Broden G", "Anika S", "Krish P"];

  var list = document.getElementById("table");

  data.forEach((item) => {
    let li = document.createElement("td");
    li.innerText = item;
    list.appendChild(li);
  });

</script>