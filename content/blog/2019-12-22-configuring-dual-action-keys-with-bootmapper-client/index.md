---
title: "Configuring Dual Action keys with BootMapper Client"
date: "2019-12-22"
tags:
  - "gear"
  - "keyboards"
---

One of the cooler features of BootMapper Client (BMC) is that it can be used to make keys work double duties - act as one key when pressed alone, and act as another when pressed in combination with another key. Unfortunately by default BMC can only do a couple of keys (for instance, it's not possible to map Caps Lock to act as both Esc and Control), but it's quite easy to extend the selection of keys that are available.

In order to do this we need to edit a JSON file from under the `json` directory whereever BMC is installed. As the functionality is called "dual action", search for a file called `dualaction.json`.

The file contanis two lists of mapping objects: `compoundKeys` and `aloneKeys`. In order to do the aforementioned Caps Lock configuration we see that while Left Control is already listed under `compoundKeys`, Esc is nowhere to be seen in the `aloneKeys`. In order to add it, we need it's BMC key code. That can be found from [this Google sheet](https://docs.google.com/spreadsheets/d/1snSczHjRXubWliuWih6y3doLTaGirQJzyhf4qk5bf1A/edit?usp=sharing).

The key code for Esc is 41, so we add the following to the JSON file:

```
{
  "label": "Escape",
  "index": 41
}
```

Now when we launch BMC the next time, Escape should be possible to be selected in the Dual Action menus.
