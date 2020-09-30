# Problems and Solutions 
1. Local build error 
```
  Dependency Error: Yikes! It looks like you don't have kramdown-parser-gfm or one of its dependencies installed. In order to use Jekyll as currently configured, you'll need to install this gem. The full error message from Ruby is: 'cannot load such file -- kramdown-parser-gfm' If you run into trouble, you can find helpful resources at https://jekyllrb.com/help/! 
             ERROR: YOUR SITE COULD NOT BE BUILT:
                    ------------------------------------
                    kramdown-parser-gfm
```
*Fix* Update Gemfile 
https://stackoverflow.com/questions/63335953/jekyll-error-building-page-related-to-kramdown-parser

2. Embedding PDFs 
*Fix* See: https://www.labnol.org/embed-pdf-200208

https://github.com/Shopify/liquid/issues/917
https://gist.github.com/Phlow/5613fb3f18946f577f071e2a258749a3
https://www.siteleaf.com/blog/advanced-liquid-sort/
https://stackoverflow.com/questions/45780291/jekyll-cant-reverse-sort-by-date
https://stackoverflow.com/questions/52344102/upgrading-jekyll-and-dependencies-for-github-pages