---
title: "From WordPress to Jekyll"
date: "2015-04-04"
---

As a geek I like to fiddle. This Saturday I wondered how difficult it’d be to transition this blog from WordPress over to Jekyll, the transition containing both the old posts and the theme.

So I jumped in, installed Jekyll and fiddled with rbenv et al. for a while until I got the environment working well enough[1](#fn:1). [Jekyll’s documentation](http://jekyllrb.com/docs/home/) is really good and the whole thing is pretty well thought out; especially the post meta information handling is nice and flexible, allowing for example easily [adding support for link posts](http://brandonbohling.com/2012/04/Link-Posts-With-Jekyll/).

The whole conversion process (including exporting data from WP, importing them to Jekyll, theming Jekyll, publishing the blog with GitHub Pages and finally making rarelyneeded.com point to here) took around 3-4 hours. I’m extremely pleased at the moment.

The only thing I’m just a tad worried about is how this is going to affect my actual blogging… as you might have noticed, I’m not that frequent writer and since a static site generator just adds complexity to the process… we’ll see.

Anyway. If anything’s broken please let me know, otherwise have a nice day!

1. I have an impedance mismatch with Ruby, but I decided to lay it aside for now. I still have to mention I’m getting these `/Users/antti/.rbenv/versions/2.2.0/lib/ruby/gems/2.2.0/gems/liquid-2.6.1/lib/liquid/htmltags.rb:43: warning: duplicated key at line 46 ignored: "index0"` errors every time I run `jekyll`… [↩](#fnref:1)
