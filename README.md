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
%command% -novid -nohltv -particles 1 -precachefontchars -noipx -softparticlesdefaultoff -full -console -noquicktime +mat_queue_mode 2 -nojoy -nosteamcontroller -vulkan +fps_max 122
```

### Adjustments to make

Set the max FPS from 122 to 2 + Display's max FPS
Remove `-nojoy -nosteamcontroller` for Steam Remote Play or controllers
removalby default on PC reduces input lag
Remove `-vulkan` if you experience issues. Generally improves performance
but may cause the inverse effect on some older devices
No compatibility layer - native is usually faster, safer and efficient.
There is the performance factor in Proton but it gives most players an insecure
mode due to VAC.

### Explanations for unwanted launch options

`-nostartupsound` just removes startup sound, not very useful
`-high` causes increase in input lag, it is mainly meant for high performance \
short lived tasks
`-threads X` Valve does not recommened using it. Default X = 3

`
