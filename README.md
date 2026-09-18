# DuForte

A TF2 config for performance, faster response and no hiccups

<div align="center">
![License](https://img.shields.io/github/license/MrGrappleMan/DuForte?style=for-the-badge)
![Last Commit](https://img.shields.io/github/last-commit/MrGrappleMan/DuForte?style=for-the-badge)
![Contributors](https://img.shields.io/github/contributors/MrGrappleMan/DuForte?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/MrGrappleMan/DuForte?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/MrGrappleMan/DuForte?style=for-the-badge)
</div>

## Quality of Life changes

Mastercomfig low graphics, high player visibility
Custom script aliasing
Intelligent crouchjumping
Silenced XP bar ( a patchy fix for loud XP bar issues )
Killsound - [DiRT 2](https://gamebanana.com/sounds/81623)
Launch options

## ⚙️ Installation ⬇️

WARNING, Backup and move away any conflicting configs, huds or other mod files

1. [Download](https://github.com/MrGrappleMan/DuForte/archive/refs/heads/main.zip) and extract the repo file
2. Put the "tf" folder in the repo alognside the "tf" folder on your PC to \
   merge them

Path for Linux

``` bash
~/.local/share/Steam/steamapps/common/Team Fortress 2/
```

Path for Windows

``` bash
C:\Program Files (x86)\Steam\steamapps\common\Team Fortress 2\
```

3. Put these launch options in Steam

```sh
%command% -novid -nostartupsound -nohltv -particles 1 -precachefontchars -noipx -softparticlesdefaultoff -full -noquicktime +mat_queue_mode 2 -nojoy -nosteamcontroller -vulkan +fps_max 60
```

## Considerations

1. Set +fps_max to screen refresh rate. Reduces heat and more stable frame rate.
2. Remove `-nojoy -nosteamcontroller` for Steam Remote Play or controllers as \
  removal by default on PC reduces input lag
3. Remove `-vulkan` if legacy incompatibility issues occur
4. Do not force any compatibility layer. VAC breaks, and native is well supported.
5. Avoid nested wayland compositors for reducing input lag
  remains

``` sh
  scb -f -F fsr -w 1920 -h 1080 -W 1920 -H 1080 --force-grab-cursor --
```

## Explanations for unwanted launch options

`-high` causes increase in input lag, it is mainly meant for high performance \
short lived tasks
`-threads X` Valve does not recommened using it, and the engine has no concept \
of it. Default X = 3
