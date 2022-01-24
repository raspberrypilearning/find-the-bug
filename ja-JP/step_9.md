## ゲームをアップグレードする

時間があれば、ゲームに別のレベルや気を散らすものを追加できます。 隠れるスプライトを変更したり、黒板のテキストを変更したりすることもできます。

新しいレベルでバグを隠すために必要なブロックは次のとおりです。

```blocks3
when backdrop switches to [new level v]

set size to [20] %

go to x: [0] y: [0] // drag to position the bug first

set [color v] effect to [50]
```

--- task ---

レベルごとに、次のことを行う必要があります。
- 背景を追加します
- ステージペインをクリックしてから、**背景**タブで新しい背景を、**終了**背景より前の位置にドラッグします。
- `背景が・・・になったとき`{:class="block3events"}ブロックを新しい背景用に追加し、バグを配置して隠すコードを追加します

**ヒント:** バグを新しい隠し場所にドラッグするには、コードを「分割」して、新しいレベルに配置するためにバグをクリックしても背景が切り替わらないようにします。

--- /task ---

--- task ---

オウムを追加したり、別のスプライトを選択して気を散らさせることができます。

オウムに使用したコードは次のとおりです。
```blocks3
when flag clicked
set rotation style [left-right v] // do not go upside down
point in direction [35] // number from -180 to 180
forever // keep being annoying
move [10] steps // the number controls the speed
if on edge, bounce // stay on the Stage
next costume // flap
change [color v] effect by [5] // try 11 or 50
wait [0.25] seconds // try 0.1 or 0.5
end
```

**ヒント:** **Parrot** スプライトのコードを別のスプライトにドラッグすると、別の気を散らすスプライトをすばやく作成できます。

![コード領域からスプライトリスト内の別のスプライトにコードをドラッグします。](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: 完成したプロジェクト
---

[完成したプロジェクトはこちら](https://scratch.mit.edu/projects/486719939/){:target="_blank"}で確認できます。

--- /collapse ---

--- save ---

