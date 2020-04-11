---
layout: default
---

# Hello!

Here is a random [test page]({% link /test.md %})

My favourite post is [this]({% post_url 2017-10-28-testing-post.md %})

Here are all the blogposts so far:

<ul>
    {% for post in site.posts %}
    <li>
        <a href="{{ site.baseurl }}/{{ post.url }}">{{ post.title }}</a>
        {{ post.excerpt }}
    </li>
    {% endfor %}
</ul>