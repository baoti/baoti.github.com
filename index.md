---
layout: page
title: Hello World!
tagline: Hello 2013.
---
{% include JB/setup %}

Welcome to baoti!

## About this blog

    class Baoti(JekyllBootstrap):
        def __init__(self):
            self.birthday = "{{ site.birthday }}"
            self.author.name = "{{ site.author.name }}"
            self.author.github = "{{ site.author.github }}"

Read [more](/pages/about.html).

## Blog Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

Learn [Racket](http://racket-lang.org/).

