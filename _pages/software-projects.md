---
layout: page
---

## software-projects 

Here's a somewhat representative sample of what I spend my time thinking about. While the timestamp format might come across as pretentious, I found that it constantly reminds me of two things. First, that I should use my time here wisely. Second, that we each have our own unique timeline -- comparing my work to that of seasoned PhDs and industry veterans is counterproductive, if anything. Hope you enjoy these, and feel free to share your comments.

<div class="posts" id="Blog">
    <ul>
        {% assign software-projects = site.software-projects | sort | reverse %}
        {% for software-project in software-projects %}
        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ software-project.url }}">{{ software-project.title | downcase }}</a>: {{ software-project.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>

</div>

