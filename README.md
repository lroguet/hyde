# Hyde-14
Hyde-14 is an enhanced version of the two-column [Hugo](https://gohugo.io) theme [Hyde](https://github.com/spf13/hyde). It pairs a prominent sidebar with uncomplicated content.

## Installation
To install Hyde-14 as your default theme, first clone this repository in the `themes/` directory:

    $ cd themes/
    $ git clone https://github.com/lroguet/hyde-14.git

Second, specify `hyde-14` as your default theme in your site `config.yaml` file. Just add:

```yaml
theme: "hyde-14"
```   

## Configuration
### Hyde
For all configuration options available in Hyde, see the original [documentation](https://github.com/spf13/hyde#options).

### Enhancements

- Disqus comment count below post title
- Disqus comments can be disabled on a per post/page basis
- Google Analytics tracking id
- Gravatar image in sidebar
- Minified CSS style sheets
- Open Graph, Google News, Schema & Twitter Cards meta tags
- Reading time below post title
- Social links with [Font Awesome](http://fontawesome.io/) 5.0.9
- And a few other layout changes to my liking

### config.yaml example
Below is the site `yaml` configuration I use to generate [fourteenislands.io](https://fourteenislands.io) with the **hyde-14** theme for Hugo.

```yaml
---

baseURL: "https://fourteenislands.io"
googleAnalytics: "UA-19075933-XX"
languageCode: "en-us"
theme: "hyde-14"
title: "fourteenislands.io"

author:
  name: "Ludovic Roguet"
  ### The hashed value of the author's Gravatar email address OR a path to a
  ### local image added to the 'static' folder (static/assets/images/avatar.jpeg for example)
  avatar: "static/assets/images/avatar.jpeg"
  external: "https://lroguet.com"
  github: "lroguet"
  linkedin: "lroguet"
  twitter: "lroguet"

params:
  ### Global
  description: "Cirrus, Cirrostratus & Cirrocumulus. From Stockholm. With Love."
  disqusShortname: "fourteenislands"
  ### Available for social: 'open-graph', 'google-news', 'schema' and 'twitter-summary-card'
  social:
    - open-graph
    - twitter-summary-card
  ### Theme
  layoutReverse: true
  ### Sidebar
  cookies: >
    This website uses [cookies](https://support.mozilla.org/en-US/kb/cookies-information-websites-store-on-your-computer) 
    to ensure you get the best experience.
  powered: false
  rss: true
  ### Will display in sidebar as '© 2010-2017' for example
  since: "1980"

permalinks:
  posts: "/:year/:month/:slug/"
  pages: "/:slug/"

taxonomies:
  category: "categories"
  tag: "tags"

---
```
## On the interwebs

* [https://fourteenislands.io](https://fourteenislands.io)
* [https://lroguet.com](https://lroguet.com)
* [https://minglass.se](https://minglass.se)