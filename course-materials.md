---
layout: page
title: Course Materials
permalink: /course-materials/
---

<div style="width:100%; float: left">
    <div class="resource-pic-gallary">
        <h2>Main resources</h2>
        {% for resource in site.data.resources.main_resources %}
        <div class="resource--image-cover-container">
            <img src="{{ resource.pic | prepend: site.baseurl }}" class="resource--image-cover">
            <p><a href="{{resource.address}}">{{resource.name}}</a></p>
        </div>
        {% endfor %}
        <br><br><br><br>
        <br><br><br><br>
        <br><br>
        <h2>Good resources</h2>
        {% for resource in site.data.resources.good_resources %}
        <div class="resource--image-cover-container">
            <img src="{{ resource.pic | prepend: site.baseurl }}" class="resource--image-cover">
            <p><a href="{{resource.address}}">{{resource.name}}</a></p>
        </div>
        {% endfor %}
        <br><br><br><br>
        <br><br><br><br>
        <br><br>
        <h2>Classic resources</h2>
        {% for resource in site.data.resources.classic_resources %}
        <div class="resource--image-cover-container">
            <img src="{{ resource.pic | prepend: site.baseurl }}" class="resource--image-cover">
            <p><a href="{{resource.address}}">{{resource.name}}</a></p>
        </div>
        {% endfor %}
    </div>
</div>