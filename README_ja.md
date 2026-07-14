# Block Elevators

<table>
	<thead>
		<tr>
			<th align="center"><a href="README.md">English</a></th>
			<th align="center">日本語</th>
		</tr>
	</thead>
</table>

ブロックを縦に積むだけで作れる、Paper向けのシンプルなエレベータープラグインです。

エレベーターブロックの上でジャンプすると上へ、スニークすると下へ移動できます。

## デモ

<a href="https://youtu.be/RzJluRqwEJk">
  <img src="https://img.youtube.com/vi/RzJluRqwEJk/maxresdefault.jpg" alt="Block Elevators Demo" width="500">
</a>

## ダウンロード

- [GitHub Releases](https://github.com/ryusei-sky/Block-Elevators/releases/latest)
- [Modrinth](https://modrinth.com/plugin/block-elevators)

## 特徴

- エレベーターブロックを設定可能
- 動作を細かくカスタマイズ可能
- 液体、カーペット、ハーフブロックなどを使った隠しエレベーターも作成可能
- Paper 1.21.x に対応

## 導入方法

1. JARファイルをサーバーの `plugins` フォルダに配置します。
2. サーバーを起動または再起動します。
3. 必要に応じて `config.yml` を編集します。

## コマンド

| コマンド | 説明 |
|----------|------|
| `/block-elevators-reload` |設定をリロード |

## 権限

| 権限 | 説明 | デフォルト |
|------|------|-----------|
| `blockelevators.use` | エレベーターをつかう | `true` |
| `blockelevators.reload` | 設定をリロード | `op` |

## config.yml

```yml
# 権限:
# blockelevators.use - エレベーター使用 (デフォルト: true)
# blockelevators.reload - 設定再読み込み (デフォルト: op)

# エレベーターを有効にするワールド
# 空の場合はすべてのワールドで有効
worlds: []
#  - world

# エレベーター使用時のクールダウン（秒）
# 0で無効
cooldown: 0

# エレベーターとして使用できるブロック
materials:
  - IRON_BLOCK

# エレベーターを検索する最大距離
# 0で無制限
max-search-range: 0

# サウンド設定
sound:
  enable: true
  name: entity.iron_golem.attack
  volume: 1.0
  jump-pitch: 1.2
  sneak-pitch: 0.8
```

## ライセンス

[MIT License](https://files.ryusei.space/docs/mit.txt)
