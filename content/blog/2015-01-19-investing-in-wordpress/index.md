---
title: "Investing in WordPress"
date: "2015-01-19"
---

Yes, thank you. I know [WordPress](http://wordpress.org) is [11 years old](https://wordpress.org/news/2003/05/wordpress-now-available/). I know it’s not that rare that someone finds a gaping hole in WordPress[1]("#fn:security"). I know PHP isn’t exactly the new hotness (especially 5.2.4, which WP still uses). To be totally honest, I used to be a big believer in custom-built software, that is, building admin-UIs and APIs from scratch using Grails or Node or what have you.

While that still remains the case in some projects, the pragmatic in me has raised it’s head and I decided to take a look in these pre-built CMS systems, such as WordPress. Of course there are others too, the big players being [Drupal]("https://www.drupal.org/") and [Joomla]("http://www.joomla.org/"). I ended up in WordPress. Why?

- **It’s simple.** I somewhat understand how WordPress works. The default database schema has eleven or so tables, each of those with clear reason for it’s existance.
- **No click-click-configuring required.** Although many WP sites are “built” by uploading WP to a server, copying a theme over and then clicking in the admin UI to install and configure plugins to create custom post types and custom fields, it’s totally possible to have all of the customization done in code. Required plugins can be installed and activated automatically with [wp-cli]("http://wp-cli.org/") or [Composer]("https://getcomposer.org/").
- **It’s easy to update.** I don’t have any real 1st-hand experience, but from what I’ve heard, updating a Drupal installation ain’t so easy as updating a WP site. Though of course one should never do that in production.

So that’s my thought process. We’ve been building a couple of WP sites with my colleagues in our little [evenings-and-weekends-sidebusiness]("http://alupark.fi"), and plan on continuing to do so. I’m also planning on bringing the good best practices from “regular software building” over to the WP world and blogging away whilst doing so. Already prototyping a little MVVM-kinda thing with WP themes…

* * *

1. To to be honest, more often than not the security problems seem to occur in shitty plugins. [↩]("#fnref:security")
