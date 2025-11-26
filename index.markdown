---
layout: default
title: About Me
---
<header>
    <h1>
        <a href="/">Brendan Lee</a>
    </h1>
    <nav>
        <a href="/about">About</a>
        <a href="https://drive.google.com/file/d/1w6dqI0fOXij0DeufXA1LqBpFxvzjhrmT/view?usp=sharing">Resume</a>
    </nav>
</header>
<div class="landing-page">
    <p> 
    Full Stack Engineer working on the high-scale e-commerce platform at Walmart in the Bay Area. Welcome to my page!
    </p>
</div>
<div class='main-post-container'>
    <h2 class='post-header'>Posts</h2>
    <ul>
        {% for post in site.posts %}
        <li>
            <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
            <span class="post-date">  {{ post.date | date: "%B %d, %Y" }}</span>
            <br>
            <div class="post-peek">
                {{ post.excerpt }}
                <a class="post-link" href="{{ post.url | relative_url }}">Read more...</a>
            </div>
        </li>
        {% endfor %}
    </ul>
</div>
