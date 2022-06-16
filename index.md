---
layout: page
---

<center>
<br/>
<img width="30%" src="/assets/img/profile.jpg" style="border-radius: 50%;">
<h2>Johannes Hagspiel</h2>
</center>

> **Note**: Test

Test 

### software projects [(see all)](/software-projects)

<div class="posts" id="Blog">
    <ul>
        {% assign software-projects = site.software-projects | sort | reverse %}
        {% for software-project in software-projects limit:10 %}

        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ software-project.url }}">{{ software-project.title | downcase }}</a>: {{ software-project.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>

</div>

### writing [(see all)](/writing)

<div class="posts" id="Blog">
    <ul>
        {% assign writings = site.writing | sort | reverse %}
        {% for writing in writings limit:10 %}

        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ writing.url }}">{{ writing.title | downcase }}</a>: {{ writing.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>
</div>

### miscellaneous

- [**bookshelf**](/bookshelf): 📚 a collection of the books I have read
- [**playlist**](/playlist): 🎧 a playlist of the podcasts I listen to