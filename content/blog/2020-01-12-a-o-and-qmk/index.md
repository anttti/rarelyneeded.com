---
title: "Ä, Ö and QMK"
date: "2020-01-12"
tags:
  - "keyboards"
---

So turns out keyboards don't emit characters per se, instead they emit key codes which then in turn the operating system resolves into characters. Therefore, if one wants to use the EN-US ANSI layout but still be able to write ä or ö, things get tricky. I'm still figuring out the best way to do it, but here are my ideas:

- Use AutoHotkey or similar to bind Alt-A to ä, Alt-O to ö. Works, but it's no fun to have to rely on a utility.
- Use EN-Intl layout and get ä and ö via Alt Gr. Works great, but makes the " key behave frustratingly (if I just want to output a ", I have to first press " and then space).
- Remap all keys in a funky german layout in ANSI style, [like done here](https://github.com/qmk/qmk_firmware/blob/master/keyboards/planck/keymaps/spacebarracecar/keymap.c). More explanation in [a Reddit thread.](https://www.reddit.com/r/olkb/comments/enp1x9/intelligent_solution_for_umlauts_on_a_planck_kb/)

Still on my TODO to try out the last one.
