# nuclear-power-test-setup-01

## Description

原子力発電所の核燃料棒を入れるインサータを回路で制御することで、どれだけ燃料消費を節約できるのかを調査する実験装置です。
マップエディタでの使用を想定していますが、無限パイプの部分を消去して汲み上げポンプに繋ぐとゲーム内で利用できます。

## Usage

1. マップエディタにてBPをインポートします。
2. マップエディタの時間タブよりゲーム時間を停止します
3. ロボットポートに物流ロボットを入れます
4. Zキーを使い、10台の原子炉に核燃料棒を1個ずつ（合計10個）入れます
5. リセットスイッチ上でFキーを押します
6. 時間タブよりゲームを再開します

![リセットスイッチの画像](/images/info/2024-08-21-21-42-39.png)

以上で発電が開始して、SEC部分に経過時間が表示されます。核燃料棒を100本消費するとカウンターが止まります。これにより核燃料棒を100本消費するまでの時間をシミュレートできます。

注意点として、最初の起動時には原子炉は0度から徐々に温度が上がっていきます。ここから原子炉の温度は最高で1000度まで上がりますが、核燃料棒の投入を制御しているので500度あたりまで下がります。517度くらいまで下がると熱交換器に伝わる温度は500度以下になり、熱交換器は稼働を停止します。原子炉はそれ以上温度が下がることはありません。

再び燃料を投下すると**0度ではなく517度から温度が上がることになります**
つまり最初の稼働時と、原子炉が温まった状態からの稼働時ではパフォーマンスが変わってきます。一定の実験結果を得るためには**原子炉が温まった状態においてロボットポートからロボットを撤去して蒸気がなくなるのを待ち、使用済核燃料棒を撤去してから実験を開始してください**

## Dependent Mods

このBlueprintは次のMODに依存しています。

- [Editor Extensions](https://mods.factorio.com/mod/EditorExtensions)
- [Power Combinator](https://mods.factorio.com/mod/power-combinator)
- [Pushbutton](https://mods.factorio.com/mod/pushbutton)
- [Text Plates](https://mods.factorio.com/mod/textplates)
- [UPS Friendly Nixie Tube Display](https://mods.factorio.com/mod/UPSFriendlyNixieTubeDisplay)


## Screenshot
![Screenshot.png](./Screenshot.png)

## Blueprint String

[here](blueprint.txt)

