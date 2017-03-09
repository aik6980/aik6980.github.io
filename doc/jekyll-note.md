# Github pages tips
## Emoji on GitHub Pages
https://help.github.com/articles/emoji-on-github-pages/

for example, using `:smiley:` for :smiley:
http://www.webpagefx.com/tools/emoji-cheat-sheet/

# Project: Incorperate Jekyll Theme Gem
updated 08/02/17

- **[x]** Learn to customize the theme, and maybe packed it for later use
- **[x]** Make github theme work locally  
https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll  
Have to add Github authourization so we can access `site.github.xxx` variables  
Git metadata fixed  
http://knightcodes.com/miscellaneous/2016/09/13/fix-github-metadata-error.html
SSL Cert fix
http://stackoverflow.com/questions/37219213/ssl-certificate-verification-failure-in-jekyll-github-metadata

- GHPages should be default to `minima` theme. This can be tested by simply removed `/_include`, `/_sass` and `/_layout` folders from your website (These folders overriding the theme, more of this later)
- Jykell 3.2+ supported a neat way to incorperate theme, by packing it into a gem  
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