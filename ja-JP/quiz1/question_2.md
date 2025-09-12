--- question ---
---
legend: 問題2/3
---

あなたは `ずっと`{:class="block3control"}ループを使って **Parrot** (オウム)スプライトが迷惑な方法で飛び回るようにしました。

別の気を散らすスプライトを追加しようとしましたが、緑色の旗をクリックすると1回だけ動いて、その後停止します。 どうすれば修正できますか？

![Rocketのスプライト](images/rocket-sprite.png)

```blocks3
when flag clicked
set rotation style [all around v] 
move [6] steps 
forever 
if on edge, bounce 
next costume 
change [color v] effect by [25] 
wait [0.5] seconds 
end
```

--- choices ---

- () `動かす`{:class="block3motion"}ブロックの数値を変更します

  --- feedback ---

`動かす`{:class="block3motion"}ブロックの数値を変更すると、緑色の旗がクリックされたときにスプライトが移動する距離が変更されますが、この変更によってロケットが移動し続けることはありません。

  --- /feedback ---

- ( ) `もし端に着いたら、跳ね返る`{:class="block3motion"} blockを削除します

  --- feedback ---

`もし端に着いたら、跳ね返る`{:class = "block3motion"}ブロックは、スプライトをステージの端から跳ね返らせます。 削除した場合、ロケットはステージの端で動かなくなります。

  --- /feedback ---

- ( ) 別の`ずっと`{:class="block3control"} ブロックを追加する

--- feedback ---

スクリプトは、`ずっと`{:class="block3control"}ブロックを１つだけ持つことができます。 `ずっと`{:class="block3control"}ブロックの下にはブロックを追加できないことに気づきましたか？

--- /feedback ---

- (x) `動かす`{:class="block3motion"} ブロックを `ずっと`{:class="block3control"}ループの中に入れます

  --- feedback ---

  そのとおり! スプライトは1回だけ動きます。 `動く`{:class="block3motion"}ブロックを `ずっと`{:class="block3control"}ループの中に移動すると、プロジェクトを停止するまでスプライトが動き続けます。

  --- /feedback ---

--- /choices ---

--- /question ---
