# Github pages tips
## Liquid syntax
https://github.com/Shopify/liquid/wiki/Liquid-for-Designers

## Emoji on GitHub Pages
https://help.github.com/articles/emoji-on-github-pages/

for example, using `:smiley:` for :smiley:
http://www.webpagefx.com/tools/emoji-cheat-sheet/

## Useful Chrome plugins for web development
### Markdown Reader
Markdown Reader, for quick preview of your markdown files
### Split Tabs
Split a screen into separate Tabs with ease. Resize opened tabs into layouts on separate windows with multiple displays support

# Project: Github Page as a proper website
updated 14/03/17

- **[wip]** Updated CV Page
- **[wip]** Web layout
- **[done]** Setup custom domain (aikdev.co.uk) using cloudflare
- ~~**optional** Themes~~ now using Bootstrap 4
- **optional** `post.excerpt` doesn't work as intended, need investigation

### Custom domain setup
1. Setup custom domain name inside Github project *Setting* menu  
https://help.github.com/articles/adding-or-removing-a-custom-domain-for-your-github-pages-site/
1. Setup an apex domain in Cloudflare  
https://help.github.com/articles/setting-up-an-apex-domain/

# Project: Bootstrap
updated 20/03/17

- **[wip]** Create web layout from scratch using Bootstrap
- Better learn more about HTML5 too, https://www.w3schools.com/tags/default.asp
- Bootstrap Ref, https://v4-alpha.getbootstrap.com/content/typography/

### Bootstrap container explained
http://blog.codeply.com/2016/04/06/how-the-bootstrap-grid-really-works/


## Liquid syntax
### Nav menu sorting
http://stackoverflow.com/questions/9053066/sorted-navigation-menu-with-jekyll-and-liquid

# Project: Incorporate Jekyll Theme Gem
updated 09/03/17

- **[wip]** Learn to customize the theme, and maybe packed it for later use
- **[done]** Make github theme work locally  
https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll  
Have to add Github authorization so we can access `site.github.xxx` variables  
  - Git metadata fixed  
  use `gem 'jekyll-github-metadata'` , simply put it into Bundle
~~http://knightcodes.com/miscellaneous/2016/09/13/fix-github-metadata-error.html~~
  - SSL Cert fix (working)  
  This is not Github problem but Ruby SSL problem on Windows OS, this is why it is so difficult to find the solution Orz  
  http://stackoverflow.com/questions/37219213/ssl-certificate-verification-failure-in-jekyll-github-metadata

- GHPages should be default to `minima` theme. This can be tested by simply removed `/_include`, `/_sass` and `/_layout` folders from your website (These folders overriding the theme, more of this later)
- Jykell 3.2+ supported a neat way to incorporate theme, by packing it into a gem  
https://jekyllrb.com/docs/themes/
- Github pages supported following themes
- using 'bundler' gem, created 'GemFile' on the root level of your website (if there ain't any)  
then add the following code

```
source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins
```
- github themes setup documentation  
https://help.github.com/articles/adding-a-jekyll-theme-to-your-github-pages-site/

# Project: Jekyll Pagination 
updated 09/03/17

Once I understand how to use `bundle` and `Gemfile` this is very simple. Basically following steps defined in Jekyll user guide

> https://jekyllrb.com/docs/pagination/

This is working but not without limitation, for a free web page I think this is good enough
