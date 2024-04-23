---
layout: default
title: "Home"
---

# Docker Compose Experiment Steps

{% for step in site.data.steps %}
<div class="step">
    <h2>{{ step.title }}</h2>
    <p>{{ step.description }}</p>
    {% if step.command != "" %}
    <pre><code>{{ step.command }}</code></pre>
    {% endif %}
    <img src="{{ step.image }}" alt="{{ step.title }}">
</div>
{% endfor %}