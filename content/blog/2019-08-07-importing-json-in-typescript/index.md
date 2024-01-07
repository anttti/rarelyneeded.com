---
title: "Importing JSON in TypeScript"
date: "2019-08-07"
tags:
  - "typescript"
---

Here's a quick tip: add `resolveJsonModule: true`  to your `tsconfig.json` and then you can just:

`import { version } from "./package.json";`
