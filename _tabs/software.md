---
icon: fas fa-code
order: 4
---


<p><a href="https://drive.google.com/drive/folders/16X8u_ZA4LTBs8cj3nJHDY29mdALZ8hV8"> Team Optix Software Slides </a> </p>
<br>
<p> Team Optix 3749 Software Blog Posts </p>

{% if site.categories.software.size > 0 %}

  {% for post in site.posts %}

    {% if post.categories contains "software" and post.hide != true %}

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

  var data = ["Toby L", "Rohin S", "Rohan J", "Jadon L", "Dash P"];

  var list = document.getElementById("table");

  data.forEach((item) => {
    let li = document.createElement("td");
    li.innerText = item;
    list.appendChild(li);
  });

</script>