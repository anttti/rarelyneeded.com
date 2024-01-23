---
title: Testing webhooks
date: 2024-01-23
tags:
  - development
  - til
---

Testing webhooks can be a bit of a tricky thing. For example Contentful, a headless CMS, provides extensive webhook functionality for implementing all kinds of functionality (in our case whenever a piece of content in Contentful changes, a webhook calls our cloud function which updates our search index). Developing these hooks can be a bit tricky, as in order to actually see what's coming out the other end an online endpoint needs to be connected to the webhook (obviously Contentful cannot call something that's running in `localhost`).

One great service for quickly checking what webhooks actually do is [Webhook.site](https://webhook.site/). Instantly upon landing on the site you get your own personal webhook URL, something like `https://webhook.site/10934d37-41be-40d4-ac2c-2b830f6ce2fa`. Now just plop that into your webhook calling configuration, trigger the webhook and see the requests logged on the page!
