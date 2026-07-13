# Elevators

<table>
	<thead>
		<tr>
			<th align="center">English</th>
			<th align="center"><a href="README_ja.md">日本語</a></th>
		</tr>
	</thead>
</table>

A simple and lightweight block-based elevator plugin for Paper.

Place elevator blocks vertically and jump to travel upward or sneak to travel downward instantly.

## Download

Download the latest version from the [Releases](https://github.com/ryusei-sky/Elevators/releases/latest) page.

## Features

- Jump to travel upward
- Sneak to travel downward
- Customizable elevator block materials
- Configurable maximum search range (`0` for unlimited)
- Configurable teleport sounds (sound, volume, and pitch)
- Cancels teleportation if the destination is blocked (Still works with liquids, carpets, slabs, and similar blocks, allowing you to camouflage the elevator's appearance.)
- Supports Paper 1.21.x

## Installation

1. Download the latest release.
2. Place the JAR file into your server's `plugins` folder.
3. Start or restart your server.
4. Edit `config.yml` if needed.
5. Enjoy!

## Commands

| Command | Description |
|---------|-------------|
| `/elevator reload` | Reloads the plugin configuration |

## Permissions

| Permission | Description | Default |
|------------|-------------|---------|
| `elevator.use` | Allows players to use elevators | `true` |
| `elevator.reload` | Allows reloading the configuration | `op` |

## Configuration

```yml
# Permissions:
# elevator.use - Allows players to use elevators (Default: true)
# elevator.reload - Allows reloading the configuration (Default: op)

# Worlds where elevators are enabled
# Empty list means all worlds
worlds: []
#  - world

# Cooldown between elevator uses (seconds)
# 0 disables cooldown
cooldown: 0

# Materials to be used as elevator blocks
materials:
  - IRON_BLOCK

# Maximum search range
# 0 means unlimited
max-search-range: 0

sound:
  enable: true
  name: entity.iron_golem.attack
  volume: 1.0
  jump-pitch: 1.2
  sneak-pitch: 0.8
```

## License

This project is licensed under the MIT License.
