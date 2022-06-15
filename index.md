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
