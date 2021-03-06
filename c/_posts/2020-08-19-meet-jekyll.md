---
layout: post
title: some jekyll basics 
description: >
  how does this thing work again?
---

This is a mini shortcut and reference guide on using Jekyll on GitHub Pages as a blogging platform. The page is a work in progress, and to be perfectly honest, is mostly here so that I remember how to update my site.

# tl;dr
[Jekyll](https://jekyllrb.com/) is a Ruby-based static website generator that can be used for publishing websites of various shapes and sizes. 

Jekyll is the engine that powers GitHub pages so based on the transitive properties of internet science Jekyll is powering this very page that you are reading. 

# Know Before You Go 
There are a few key concepts or technologies that you should be aware of as you progress through this journey.

The links are here for reference, but you do not have to detour to learn everything about everything before launching a site using Jekyll.

TODO: add link on launching a site on GitHub pages using Jekyll.

- Ruby  
- Github Pages  
- Markdown  
- Liquid Templating Language
- YAML


`to bake an apple pie, you must first invent the universe. -carl sagan`

**Useful Links**  
[Jekyll Website](https://jekyllrb.com/)  
[GitHub Pages - Getting Started](https://pages.github.com/)   
[GitHub Pages Reference](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/)  
[Great Reference Guide](https://learn.cloudcannon.com/)


# Let's Talk Tech 
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
The [GitHub Pages - Getting Started](https://pages.github.com/) guide is a good place to start if you are publishing on GitHub. It's free and if you are looking to get something online fast, there are a handful of pre-built templates that you 
launch in 5 minutes and a few clicks from the Settings page of your repository. 


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
@TODO Fix the highlight type and explain

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
