---
icon: fas fa-bolt
order: 5
---


<p> Team Optix 3749 Electrical Blog Posts </p>

{% if site.categories.electrical.size > 0 %}

  {% for post in site.posts %}

    {% if post.categories contains "electrical" and post.hide != true %}

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

  var data = ["Alex Z", "Varalu N", "Chinmay N", "Collin M", "Alex G", "Ace C", "Parmis J", "Matthew W"];

  var list = document.getElementById("table");

  data.forEach((item) => {
    let li = document.createElement("td");
    li.innerText = item;
    list.appendChild(li);
  });

</script>