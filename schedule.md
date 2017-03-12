---
layout: page
title: Results
permalink: /results/
---

The two days of Science Together were distributed as:

| **Time** | **2nd March**                                     | **3rd March**                             |
|     :--- | :---                                              | :---                                      |
|    10:30 | Intro/Keynote                                     | [1st session](/blog/categories/#1Session) |
|    13:20 | [Workflow of tools](/blog/)                       | [2nd session](/blog/categories/#2Session) |
|    15:30 | [speed blogging](/blog/categories/#speedblogging) | [3rd session](/blog/categories/#3session) |
{:.mbtablestyle .whiteboard }

<br>
Check the [summary](/blog/2017-03-11-Summary.html) for the full overview of what
happened during these two days.

## List of posts

{% for post in site.posts %}
 - [{{post.title}}]({{post.url}})
{% endfor %}

### Categories

{% for category in site.categories %} [{{category | first }}](/blog/categories/#{{ category | first | slugize }}){% endfor %}

