---
layout: page
---

## Websites 

<div class="posts" id="Blog">
    <ul style="padding-left: 0em">
        {% assign websites = site.websites | sort | reverse %}
        {% for website in websites %}
        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ website.url }}">{{ website.title | downcase }}</a> {{ website.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>
</div>
