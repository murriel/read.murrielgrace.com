source "https://rubygems.org"

# Pin Jekyll 3.10 + Sass converter 1.5 for 100% parity with GitHub Pages
# and compatibility with Hydejack 8 SCSS syntax
gem "jekyll", "~> 4.4"
gem "jekyll-sass-converter", "~> 3.1"

# Ruby 3.x stdlib gems used by Jekyll local server
gem "webrick", ">= 1.9.1"

# Security floors for transitive dependencies
gem "addressable", ">= 2.9.1"
gem "concurrent-ruby", ">= 1.3.7"
gem "rexml", ">= 3.4.1"

group :jekyll_plugins do
  gem "jekyll-default-layout"
  gem "jekyll-feed"
  gem "jekyll-optional-front-matter"
  gem "jekyll-paginate"
  gem "jekyll-readme-index"
  gem "jekyll-redirect-from"
  gem "jekyll-relative-links"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
  gem "jekyll-titles-from-headings"
  gem "kramdown-parser-gfm"
end

gem "tzinfo-data", platforms: [:mingw, :mswin, :x64_mingw, :jruby]
