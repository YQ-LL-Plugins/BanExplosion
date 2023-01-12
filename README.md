# BanExplosion

> A LiteLoaderBDS plugin to custom and intercept explosions

## Usage

`/banexp on`:   Ban explosions in config file

`/banexp off`:  Unban explosions in config file

`/banexp reload`:  Reload config file



## Config file

At `plugins/BanExplosion/config.ini`, with comments in file

- `NoExplosion=1` means this type of explosion is banned directly
- `NoExplosion=0`, but `NoDestroyBlock=1` means that this type of explosion will still occur and hurt entities in game, but will never destroy blocks and create fires

```ini
; TNT
[minecraft:tnt]
NoExplosion = 0
NoDestroyBlock = 1

; 爬行者
[minecraft:creeper]
NoExplosion = 0
NoDestroyBlock = 1

;末地水晶
[minecraft:end_crystal]
NoExplosion = 0
NoDestroyBlock = 1

; 恶魂火球
[minecraft:fireball]
NoExplosion = 0
NoDestroyBlock = 0

; TNT矿车
[minecraft:tnt_minecart]
NoExplosion = 0
NoDestroyBlock = 1

; 凋零爆炸与吃方块
[minecraft:wither]
NoExplosion = 0
NoDestroyBlock = 0

; 黑色凋零之首
[minecraft:wither_skull]
NoExplosion = 0
NoDestroyBlock = 0

; 蓝色凋零之首
[minecraft:wither_skull_dangerous]
NoExplosion = 0
NoDestroyBlock = 0

; 重生锚
[minecraft:respawn_anchor]
NoExplosion = 1

; 床
[minecraft:bed]
NoExplosion = 0
NoDestroyBlock = 0
```

