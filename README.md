# Factorio Blueprint Library (FBL)

このリポジトリはFactorioの個人的なBlueprintをまとめています。
構造については模索中であり、変更する可能性があります。


## Structure

```
/category/blueprint_name/
  ├── info.md       # Explanation and usage details for the blueprint
  ├── Screenshot.png   # Screenshot of the blueprint
  ├── blueprint.txt   # Blueprint string
```

## Tips

ゲーム内コマンドでスクリーンショットを撮影できます。

```bash
/c game.take_screenshot{ show_entity_info=true, zoom=0.5 }
```

スクリーンショットはfactorioディレクトリに作成されます。

```
/factorio/script-output/screenshot.png
```

### info.md Template for Blueprints

```md
# [Blueprint name]

## Description

説明

## Usage

使用方法

## Dependent Mods

このBlueprintは次のMODに依存しています。

- [Editor Extensions](https://mods.factorio.com/mod/EditorExtensions)
- [Power Combinator](https://mods.factorio.com/mod/power-combinator)
- [Pushbutton](https://mods.factorio.com/mod/pushbutton)
- [Text Plates](https://mods.factorio.com/mod/textplates)
- [UPS Friendly Nixie Tube Display](https://mods.factorio.com/mod/UPSFriendlyNixieTubeDisplay)


## Screenshot
![Screenshot.png](Screenshot.png)

## Blueprint String

[here](blueprint.txt)


```
