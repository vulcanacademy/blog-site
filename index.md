---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Home
nav_order: 1
---

# Welcome to the Vulcan Code Academy
_Live. Code. Prosper._

At Vulcan Code Academy we are focused on helping folks learn the ins and outs of becoming a developer. We remember what it was like when we first started, and want to help you _not_ make the same mistakes we made!

So, what can you expect here at Vulcan Code Academy? Two things:

1. **Series** in the form of guides and tutorials around common topics and pathways for new developers.
2. **Blog** posts by the authors of Vulcan Code Academy.

----------------------
## Series

If you look on the sidebar (or menu in top-right if on mobile) you will find **Series** such as _WebDev_ or _Data Structures_. The content you find in this area of Vulcan Code Academy is intended to be guides and/or tutorials to train and improve your craft as a developer.

Go forth and explore!

----------------------
## Blogs

The authors at Vulcan Code Academy are passionate about tech, code, and many other things! So, we have a place to write about all that. **Blog** posts will be categorized for ease of navigation and discovery.

You can expect articles more along the lines of "tips n tricks" vs "do these things to become a developer". That content is located in the **Series** described above. Check out some recent posts below!

----------------------
### Recent posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

