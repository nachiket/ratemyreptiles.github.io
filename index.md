---
layout: default
title: Rating Waterloo Reptiles.... since 2025
---

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}


<form action="https://formsubmit.co/nachiket@gmail.com" method="POST">
  <textarea name="usercode" rows="10" style="width:100%;" placeholder="Write your code here..."></textarea><br>
  <input type="hidden" name="_subject" value="New Code Submission!">
  <input type="hidden" name="_captcha" value="false">
  <button type="submit">Submit Code</button>
</form>
