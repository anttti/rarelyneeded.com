---
title: "My CS:GO autoexec.cfg"
date: "2019-08-08"
tags:
  - "games"
---

This here is mainly for my own purposes: The configuration I like when playing Counter-Strike: Global Offensive.

```
bind f "use weapon_flashbang"
bind c "use weapon_smokegrenade"
bind g "use weapon_hegrenade"
bind x "use weapon_incgrenade;use weapon_molotov"

bind "kp_ins" "buy vesthelm;"
bind "kp_del" "buy ak47; buy m4a1;"
bind "kp_enter" "buy flashbang;"
bind "kp_plus" "buy smokegrenade;"
bind "kp_minus" "buy sg556; buy aug;"
bind "kp_home" "buy defuser;"
bind "kp_leftarrow" "buy tec9; buy fiveseven;"
bind "kp_end" "buy deagle;"
bind "kp_5" "buy ump45;"
bind "kp_downarrow" "buy p90;"
bind "kp_rightarrow" "buy hegrenade;"
bind "kp_pgdn" "buy molotov; buy incgrenade;"

alias "+jumpthrow" "+forward;+jump;-attack"
alias "-jumpthrow" "-jump;-forward"
bind "h" "+jumpthrow"

alias +knife slot3
alias -knife lastinv
bind q +knife
bind mouse4 +knife

cl_autoweaponswitch "0"
gameinstructor_enable 0

cl_teamid_overhead_always "1"
+cl_show_team_equipment
cl_showloadout "1"

cl_radar_always_centered "0"
cl_radar_scale "0.3"
cl_hud_radar_scale "1.15"

rate 128000;
cl_interp 0;
cl_interp_ratio 1;
cl_cmdrate 128;
cl_updaterate 128;

cl_crosshairalpha "200"
cl_crosshaircolor "5"
cl_crosshaircolor_b "50"
cl_crosshaircolor_r "50"
cl_crosshaircolor_g "250"
cl_crosshairdot "0"
cl_crosshairgap "-1"
cl_crosshairsize "2"
cl_crosshairstyle "4"
cl_crosshairusealpha "1"
cl_crosshairthickness "1"
cl_fixedcrosshairgap "-1"
cl_crosshair_outlinethickness "0"
cl_crosshair_drawoutline "0"

sensitivity 0.7

host_writeconfig
echo "Loaded autoexec!"
```

Place the file to `\Program Files (x86)\Steam\userdata\{user id}\730\local\cfg\` and make it read-only.
