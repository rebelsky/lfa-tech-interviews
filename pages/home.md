---
title: Thinking Beyond Grinnell---Learning from CS Alumni
permalink: /home/
---
# {{ page.title }}

**_This site is under development!_**

<dl class="dl-horizontal">
  <dt>Instructor</dt>
  <dd>
    <p><a href="{{ site.instructor_homepage }}">{{ site.instructor }}</a>
      [<a href="mailto:{{ site.instructor_email }}">{{ site.instructor_email | remove: "@grinnell.edu" }}</a>]</p>
  </dd>

  <dt>Meeting Times</dt>
  <dd>
    <ul class="list-unstyled">
      {% for item in site.meeting_times %}
        <li>{{ item | markdownify | remove: "<p>" | remove: "</p>" }}</li>
      {% endfor %}
    </ul>
  </dd>

  <dt>Office Hours</dt>
  <dd>
    <ul class="list-unstyled">
      {% for item in site.office_hours %}
        <li>{{ item | markdownify | remove: "<p>" | remove: "</p>" }}</li>
      {% endfor %}
    </ul>
  </dd>
</dl>

## About this course

Welcome to the Fall 2020 session of Grinnell College's CSC 281, a course entitled _Thinking Beyond Grinnell---Learning from CS Alumni_. In this course, we will meet virtually with alumni with careers related to computer science who will talk about their life and career paths, and will provide advice for students on things to learn and things to do. 

The focus of the class is the visits by alumni. While in some years some of these visits will involve alumni coming directly to campus, this year, all of our visits will be online via Webex.

The Web site for the course is <http://www.cs.grinnell.edu/~rebelsky/Courses/CSC281/2020F/> You find find some interesting things on the course web, and I'd encourage you to look there.

This is an evolving course. Among other things, this means that I expect to be updating the syllabus as the semester goes on.


