---
layout: page
---

<center>
<br/>
<img width="30%" src="/assets/img/profile.jpg" style="border-radius: 50%;">
<h2>Johannes Hagspiel</h2>
</center>

> **Note**: I'm moving my work to a different space. Read more [here](/reflections/near-future-plans).

I'm a Romanian-born Netherlands-based student exploring synergies between the organic and the artificial. At peak idealism, this means bringing together minds and machines into a transhumanist symbiosis. Concretely, however, it currently means putting together proof-of-concept tools based on off-the-shelf ML models or, more recently, tiny experimental investigations into aligning AI to human intentions. My work is made possible by a handful of generous [sponsors](/sponsors).

Outside thoughtware, I'm currently learning Chinese and representational drawing, with varying degrees of success. I love visiting other worlds through fiction, and I'm trying my best to combine the effectiveness of habits with the quality of agency. To share my thoughts in a more structured format, I'm writing one short article per week.

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
