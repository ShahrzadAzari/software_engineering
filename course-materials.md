---
layout: page
title: Course Materials
permalink: /course-materials/
---

<div style="width:100%; float: left">
    <div class="profile-pic-gallary ">
        <h2>Resources</h2>
        {% for resource in site.data.resources.resources %}
        <div class="image--cover-container">
            <img src="{{ resource.pic | prepend: site.baseurl }}" class="image--cover">
            <p><a href="{{resource.address}}">{{resource.name}}</a></p>
        </div>
        {% endfor %}
    </div>
</div>