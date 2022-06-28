---
layout: page
---

## scripts & exercises 

<div class="posts" id="Blog">
    <ul style="padding-left: 0em">
        {% assign scripts-exercises = site.scripts-exercises | sort | reverse %}
        {% for script-exercise in scripts-exercises %}
        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ script-exercise.url }}">{{ script-exercise.title | downcase }}</a>: {{ script-exercise.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>
</div>
