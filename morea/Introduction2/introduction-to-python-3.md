---
title: "E02: Introduce yourself"
published: true
morea_id: experience-introduce-yourself-10
morea_type: experience
morea_summary: "Get started with the ICS 314 Discord server"
morea_sort_order: 3
morea_start_date: "2021-07-08T23:00"
morea_labels:
---

# E02: Introduce yourself

## Task

For this experience, join the ICS 314 Discord server. You will receive an invitation to this server via email.

Please read through all channels in the Welcome category.

It is your responsibility to receive information about this class promptly. I highly recommend that you install a native client for Discord on your phone and your laptop and set it to display notifications.

## Submission instructions

By the time and date indicated on the Schedule page, you must have:

  * Joined the ICS 314 Discord server
  * Performed all setup actions specified in the Welcome category channels.

```
# hello 
print('hello') #code
```

Did That work?

<div class="{% cycle 'section-background-1', 'section-background-2' %}">
  <div class="container">
    <h2><small>Module:</small> <a href="{{ site.baseurl }}{{ module.module_page.url }}">{{ module.title }}</a></h2>
    {% if module.morea_experiences.size == 0 %}
    <p>No experiences for this module.</p>
    {% endif %}

    <div class="row">
    {% for page_id in module.morea_experiences %}
      {% assign experience = site.morea_page_table[page_id] %}
      {% include entity-card.html url=experience.morea_url title=experience.title summary=experience.morea_summary labels=experience.morea_labels %}
    {% endfor %}
    </div>
  </div>
</div>
