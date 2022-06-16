---
layout: page
---

## writing 

<div class="posts" id="Blog">
    <ul>
        {% assign writings = site.writing | sort | reverse %}
        {% for writing in writings %}
        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ writing.url }}">{{ writing.title | downcase }}</a>: {{ writing.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>
</div>
