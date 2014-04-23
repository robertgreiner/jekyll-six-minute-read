#jekyll-6-minute-read

Customize your jekyll blog to display the number of minutes it will take to read your article.

    <div class="post-meta"><span>{{ page.content | number_of_words | plus: 300 | divided_by: 160 | append: " minute read" }}</span></div>