---
layout: page
---

## miscellaneous 

<div class="posts" id="Blog">
    <ul style="padding-left: 0em">
        {% assign miscellaneous = site.miscellaneous | sort | reverse %}
        {% for misc in miscellaneous %}
        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ misc.url }}">{{ misc.title | downcase }}</a>: {{ misc.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>
</div>
