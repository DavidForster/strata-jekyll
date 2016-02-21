# Strata for Jekyll

A simple, responsive blog theme for the [Jekyll](http://jekyllrb.com) static site generator using [HTML5 UP's Strata](http://html5up.net/strata) design.

![preview](preview.jpg)

Browse the [demo](http://davidforster.com/strata-jekyll/).

## How to use

### Quick start

If you just want to get a blog up & running at [GitHub Pages](https://pages.github.com) then simply fork this repository to your own GitHub account and name the new repository *\<yourgithubusername\>.github.io*. GitHub should then start hosting your site at *http://\<yourrgithubusername\>.github.io/*. If you'd like to use your own domain name you can follow GitHub's guide to using a [custom domain](https://help.github.com/articles/using-a-custom-domain-with-github-pages/).

Edit the `_config.yml` file and use the options available in the theme, as mentioned below in the features section, to customise your site.

I recommend Development Seed's awesome [Prose](http://prose.io) editor to write your posts.

### Local development

If you want to run and develop locally on your own computer then you'll need the Ruby programming language and Jekyll installed. The Jekyll website has a handy [installation guide](http://jekyllrb.com/docs/installation/) in their online documentation. Once installed, you can download or clone this repository and run `bundle exec jekyll serve` from the root.

## Features

### Disqus comments

[Disqus](https://disqus.com) comments appear beneath posts. Add your Disqus website's shortname to `_config.yml` as `disqus_shortname:`. Leave `disqus_shortname` blank to disable comments completely or add `disqus: disabled` to a post's front matter to disable comments just for that page.

### Open Graph (Facebook) and Twitter Card meta tags

All pages have Open Graph metadata added.

All pages have Twitter Card metadata, though this requires `twitter_username:` to be configured in `_config.yml`. Twitter Card titles are trunacted at 70 characters and descriptions at 200 characters as per Twitter requirements.

Both Open Graph and Twitter Cards can show images if you specify `image: <image url>` in a page's front matter.

### RSS and Atom feeds

The last 10 posts are available in RSS and Atom format at `rss.xml` and `atom.xml`. Both feeds are linked to from every page's metadata. The feed icon in the footer is configurable by setting `feed_icon:` in `_config.yml` to `rss` or `atom`, or the property can be left blank to remove it completely.

### Feed footer

A footer is added to every post in both the RSS and Atom feeds. This is configurable by editing `_includes/feed-footer.html`.

### Sitemap

Based on [David Ensinger's sitemap](http://davidensinger.com/2013/11/building-a-better-sitemap-xml-with-jekyll/), supported front matter is:

- `sitemap.exclude: true` for pages, `post.published: false` for posts
- `sitemap.lastmod` (defaults to the post or page date)
- `sitemap.changefreq` (defaults to monthly)
- `sitemap.priority` (defaults to 0.5)

### Footer social media links

Social media icon links in the footer are enabled by adding or removing values for the following sites in `_config.yml`.

- Facebook - `facebook_username:`
- Twitter - `twitter_username:`
- LinkedIn - `linkedin_username:`
- Instagram - `instagram_username:`
- Pinterest - `pinterest_username:`
- Flickr - `flickr_username:`
- GitHub - `github_username:`

You can change the icon order and add more options by editing `_includes/footer.html`. I recommended a maximum number of 5 icons in total (including the feed icon).

### Reading time

Reading time appears on post pages alongside the date and categories if the time is 1 minute or more, based on a reading rate of 180 words per minute (3 per second).

### Pagination

Pagination is set at 5 posts per page, this can be altered by changing the `paginate:` property in `_config.yml`

### Next/Previous posts

The Next and Previous posts are displayed underneath every post (and Disqus comments if enabled) along with their excerpt.

### Custom 404

If you host your site with [GitHub Pages](https://pages.github.com) then a custom 404 page has been added (see `404.md`)

### robots.txt and humans.txt

The theme includes a basic robots.txt file which allows all robots to crawl the entire site and directs them to the sitemap.xml file. There is also a humans.txt file giving credit to Myself ([David Forster](http://davidforster.com)) and AJ, the designer of Strata.

## Acknowledgements

- [AJ](https://twitter.com/n33co) and [HTML5UP](http://html5up.net) for the design of Strata
- [David Ensinger](http://davidensinger.com) for a bunch of tips and ideas related to Jekyll

## Contributions

Issues, Pull Requests, Tweets and Forks are all greatly appreciated!

## License

The Jekyll theme is licensed under the [MIT](http://choosealicense.com/licenses/mit/) License

The Strata design is licensed under the [Creative Commons Attribution 3.0 Unported](http://creativecommons.org/licenses/by/3.0/) license.
