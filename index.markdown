---
layout: default
title: Brendan Lee
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
<body>
    <div>
        <p> 
        Full Stack Engineer working on the high-scale Marketplace platform at Walmart in the Bay Area. I build robust, modern systems, drawing on my previous experience in aerospace embedded engineering.
        </p>
    </div>
    <div>
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
    </div></body>
