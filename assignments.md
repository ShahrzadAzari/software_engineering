---
layout: page
title: Assignments
permalink: /assignments/
---
<p>
<big>
<h1>A complete commercial level project done during the term with the following conditions:</h1>
<ul>
  <li>Scrum should be used as the project management framework</li>
  <li>Teams should consist of at least 4 people</li>
  <li>Deliverables should be provided in each sprint</li>
  <li>A special focus on the followings:
    <ul>
      <li>Architecture</li>
      <li>Design decisions</li>
      <li>Project management reports</li>
      <li>Learning new things!</li>
    </ul>
  </li>
</ul>
</big>
</p>

<ul id="archive">
{% for asg in site.assignments reversed %}
      <li class="archiveposturl" style="background: transparent">
        <span><a href="{{ asg.url | prepend: site.baseurl}}">{{ asg.title }}</a></span>
<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right">
<a title="Download problems (pdf)" href="{{ asg.pdf | prepend: site.baseurl }}"><i class="fas fa-file-pdf"></i></a> 
{% if asg.attachment %}
&nbsp; <a title="Download attachments (zip)" href="{{ asg.attachment | prepend: site.baseurl }}"><i class="fas fa-file-archive"></i></a>
{% endif %}
</strong> 
      </li>
{% endfor %}
</ul>