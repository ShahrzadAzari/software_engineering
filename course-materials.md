---
layout: page
title: Course Materials
permalink: /course-materials/
---

<div style="width:50%; float: left">
    <div class="profile-pic-gallary ">
        <h2>Resourses</h2>
        <div class="image--cover-container">
            {% for resource in site.data.resources %}
            <img src="{{ resource.pic | prepend: site.baseurl }}" class="image--cover">
            <p><a href="{{resource.address}}"></a>{{resource.name}}</p>
            {% endfor %}
        </div>
    </div>
</div>
