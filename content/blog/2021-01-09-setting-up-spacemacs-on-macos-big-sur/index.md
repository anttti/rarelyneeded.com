---
title: "Setting up Spacemacs on macOS Big Sur"
date: "2021-01-09"
tags:
  - "macos"
---

## 1\. Install Emacs

Spacemacs is actually just a premade set of configurations for Emacs, thus the first step on installing Spacemacs is to install Emacs. An easy way to install Emacs on a Mac is to use Homebrew:

```
brew install --cask emacs
```

## 2\. Install Source Code Pro font

Source Code Pro is the suggested font for Spacemacs. You can of course change the font later on, but to make things simple, install the free & open source font from [GitHub](https://github.com/adobe-fonts/source-code-pro).

## 3\. Clone Spacemacs configuration

To install the actual Spac part of Spacemacs, `git clone` the repository either directly to `~/.emacs.d` if you don't have an existing Emacs installation, or to some other place and then copy/merge things over:

```
git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d
```

## 4\. Run the wizard

Start Emacs and the Spacemacs wizard should pop up, prompting you for your preferences regarding some of the most common options.

## 5\. Bump up the font size

The default font size of Spacemacs is painfully small 10. To bump it up, hit `SPC f e d`, search for `dotspacemacs-default-font` and increase the `:size` prop to a more comfortable one. It should be possible to reload the config by hitting `SPC f e R`, but for me setting the font side required restarting Emacs.

## 6\. Draw the rest of the owl

Navigate to your preferred [search engine and search for Spacemacs tutorials](https://duckduckgo.com/?q=spacemacs+tutorial&ia=web) to continue your journey!
