---
layout: home_page
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

### scripts & exercises [(see all)](/scripts-exercises)

<div class="posts" id="Blog">
    <ul>
        {% assign scripts-exercises = site.scripts-exercises | sort | reverse %}
        {% for script-exercise in scripts-exercises limit:10 %}

        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ script-exercise.url }}">{{ script-exercise.title | downcase }}</a>: {{ script-exercise.description | downcase }}</div>
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

### websites [(see all)](/websites)

<div class="posts" id="Blog">
    <ul>
        {% assign websites = site.websites | sort | reverse %}
        {% for website in websites limit:10 %}

        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ website.url }}">{{ website.title | downcase }}</a>: {{ website.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>
</div>


### miscellaneous

[**bookshelf**](/bookshelf): 📚 a collection of the books I have read<br>
[**playlist**](/playlist): 🎧 a playlist of the podcasts I listen to