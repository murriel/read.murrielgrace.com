---
layout: post
title: jekyll revisited
categories: [tech]
description: a shortcut reference guide for using Jekyll, the static site generator, on GitHub pages
---

This is a mini shortcut and reference guide on using Jekyll on GitHub Pages as a blogging platform. The page is a work in progress, and to be perfectly honest, is mostly here so that I have quick reminders about how to update my site.

**Know Before You Go**
There are a few key concepts or technologies that you should be aware of as you progress through this journey.

You do not have to detour to learn about the world before you start, but having general knowledge of these systems is helpful.
(condense)

`to bake an apple pie, you must first invent the universe. -carl sagan`

- Ruby  
- Github Pages  
- Markdown  
- Liquid Templating Language
- YAML


**Useful Links**  
[Jekyll Website](https://jekyllrb.com/)  
[GitHub Pages - Getting Started](https://pages.github.com/)   
[GitHub Pages Reference](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/)  
[Great Reference Guide](https://learn.cloudcannon.com/)


**Basic Directory Structure:**

| Directory    |  | Notes  |
|---|---|--|
| \_data |  | Location for any data that can be referenced in the site. Typically in json, yml, or csv format |
| \_drafts |  | Drafts are saved locally but not checked in to version control. |
| \_includes  | | sidebars and headers |
| \_layouts  | | page layouts |
| \_pages | | 'nonpost' pages |
| \_posts  |   | posts go here |
| \_site  | | generated website will go here. don't touch this. this should be in your .gitignore if hosting on GitHub Pages |
| assets  | | css, images, javascript, other utilities |

<br>


**What's Up GitHub?**  
GitHub Branches

**Front Matter**  
The front matter is a small section of YAML at the very start of a post, that includes meta information about the post such as the layout type, title, and categories.

Example:
```
---
layout: post | page
title: jekyll revisited | so meta | page name here
categories: [tech]
description: tell me about the page
---
```
**Note:** You can also leave the front matter blank! Just include the triple dashes so that the page will be processed by Jekyll, like so:
```
---
---
```

You can also add custom variables the the front matter that will display on the page layout. For example, if you add `author: guestauthor` to the front matter, you can then reference that variable in the layout html document using `page.author` enclosed in double curly brackets.  

<!-- @TODO - what happens without front matter? -->


**To Add a New Post**  
To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. "ext" will usually be ".md" for Markdown.  

To add tags to posts, add the following to the Jekyll Front Matter
tags: [demo, dbyll, dbtek, sample2]


**To Add Pages**  
To add new pages, simple add a file in the `_pages` directory that includes the necessary front matter. The extension will usually be ".md" for Markdown.

These pages will then be available on the site. Use the base directory and reference the page without the extension. For example,  `_pages/about.md` will be available on `www.yoursite.com/pages/about`  

**Code Snippets**  
@TODO Add the highlight type and explain

{% highlight ruby %}
def foo
  puts 'foo'
end
{% endhighlight %}

{% highlight yaml %}
title: yaml block
{% endhighlight %}


**Running Locally**

*Footnotes:* The shortcuts and details above were compiled from various Jekyll and theme reference guides.  
Here's a cool look at the evolution of GitHub pages: https://blog.github.com/2015-04-27-eight-lessons-learned-hacking-on-github-pages-for-six-months/  
