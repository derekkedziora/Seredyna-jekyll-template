# Seredyna, a Jekyll Template 

This has everything you need to get started using my personal site, [derekkedziora.com](https://derekkedziora.com), as a template for your own Jekyll site. 

I’ve removed all of my information and content, included some examples and added a bit of documentation. It’s not a true theme, so will require some basic coding knowledge to adapt it to your needs. 

## Getting started 

1. Add your own info in the `_config` file 
2. Read the posts to understand how it works 
3. Add your own pictures in `_includes/about-picture-script.html`

## Structure 

This is an RSS first blog and microblog. 

Posts with the category `rss-club` will **only** be published via the RSS feed. 

By default only 10 notes are displayed on the site at a time, although the permalinks to older notes don’t expire. This allows the site to stay fresh and not overwhelming without breaking links and allows you to still have easy access to older notes. 

`/now` will display the most recent post with the category `now`. 


## Blocked from Google by default 

The main page, about, portfolio page and blog posts under the category `essay` are all visible to search engines by default. My assumption is this is the sort of evergreen content that you want to display to world and be found by.

Notes and rss-club posts are blocked from search engines by default. These are more experimental posts that are meant to be more private and fleeting. Not everything needs to be remembered until the end of the internet. 

If you don’t want to use these defaults, move pages from the `_no-index` folder to the `_pages` folder and adjust the conditional `no-index` in the `_config` file and in `_includes/head-matter.html`


## To do 

- [ ] I’m still not happy with the internal navigation, want to clean it up a bit 
- [ ] Add a bit more clear documentation about social images 
- [ ] More detailed documentation about the now posts 