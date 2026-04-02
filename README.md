# DuForte

<div align="center">

A TF2 config for more performance

![License](https://img.shields.io/github/license/MrGrappleMan/DuForte?style=for-the-badge)
![Last Commit](https://img.shields.io/github/last-commit/MrGrappleMan/DuForte?style=for-the-badge)
![Contributors](https://img.shields.io/github/contributors/MrGrappleMan/DuForte?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/MrGrappleMan/DuForte?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/MrGrappleMan/DuForte?style=for-the-badge)
</div>

<div align="center">

## Quality of Life changes

</div>

Mastercomfig - Low graphics
Custom scripting
Silenced XP bar
Killsound - [DiRT 2](https://gamebanana.com/sounds/81623)
Launch options

<div align="center">

⚙️ Installation ⬇️

</div>

WARNING, Backup and move away any unsafe configs, huds or other mod files that
may conflict

1. [Download](https://github.com/MrGrappleMan/DuForte/archive/refs/heads/main.zip) and extract the repo file
2. Put the "tf" folder alongside the "tf" folder in the game folder, which will
merge them
3. Put these launch options in Steam

```sh
mangohud scb -f -F fsr -w 1920 -h 1080 -W 1920 -H 1080 --force-grab-cursor -- %command% -novid -nohltv -particles 1 -precachefontchars -noipx -softparticlesdefaultoff -full -noquicktime +mat_queue_mode 2 -nojoy -nosteamcontroller -vulkan +fps_max 62
```

### Considerations

Set +fps_max from 2 + Display FPS
Remove `-nojoy -nosteamcontroller` for Steam Remote Play or controllers as \
removal by default on PC reduces input lag
Remove `-vulkan` if old hardwware issues occur. Vulkan is a modern graphics API.
Do not force any compatibility layer as VAC is blocked. Good on other games.
Assumes you use Bazzite and have MangoHud on your system.
Set the resolution for both W H and w h to be the same

### Explanations for unwanted launch options

`-nostartupsound` just removes startup sound, not very useful
`-high` causes increase in input lag, it is mainly meant for high performance \
short lived tasks
`-threads X` Valve does not recommened using it. Default X = 3
