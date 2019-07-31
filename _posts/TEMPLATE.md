---
# Jekyll supported - https://jekyllrb.com/docs/variables/#page-variables
layout: post
title:  THIS IS A TEMPLATE 
date:   2019-07-24 21:48:30 -0700
# Category: Determines the url of this post, careful!!!
#  For example: 
#     category: work code
#               url: vca.netlify.com/work/code/2019/07/24/title-of-post.md
category: webdev
# Turn to true and post will publish next build
# published: false

# Created by VCA
# Use for internal categorizing
# separated tags by spaces
tags: html webdesign
author: YOUR_NAME_HERE
---

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/

[JEKYL GLOBAL VARIABLES][jekyll-global]

[jekyll-global]: https://jekyllrb.com/docs/variables/

<!-- Example of how to dynamically populate posts with filtering -->
<ul>
  {% for post in site.posts %}
    {% if post.tags contains  page.tags %}
      <li>
        <span>{{ page.tags }} - </span><a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
