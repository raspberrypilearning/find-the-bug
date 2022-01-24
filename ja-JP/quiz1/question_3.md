--- question ---
---
legend: 質問3/3
---

このスクリプトを**バグ** スプライトに追加しました。

![バグのスプライト。](images/bug-sprite.png)

```blocks3
when backdrop switches to [終了 v]
set size to [100] % 
go to x: [0] y: [30] 
+ say (timer) 
```

`タイマー`{:class="block3sensing"}`と言う`{:class="block3looks"}ブロックで、背景が **終了**に切り替わったときに、ステージはどのようになりますか？

--- choices ---

- ( ) ![タイマーの値"4.52"をいうオウム 。](images/quiz_parrot_number.png)

  --- feedback ---

スクリプトをもう一度見て、どのスプライトがゲームの主人公であるかを考えてください(オウムは単に迷惑な邪魔者です)。

  --- /feedback ---

- ( ) !["タイマー"という言葉をしゃべるオウム。](images/quiz_parrot_timer.png)

  --- feedback ---

`タイマー`{:class="block3sensing"}ブロックは、 `調べる`{:class="block3sensing"}ブロックメニューにあります。 スプライトは「タイマー」という言葉をしゃべるのではありません。 また、どのスプライトがこのコードを使用しているかを考えてください。

  --- /feedback ---

- (x) ![タイマ値である "4.52"を言うバグ。](images/quiz_bug_number.png)

  --- feedback ---

そうです。 `タイマー`{:class="block3sensing"}ブロックは、プロジェクトが開始されてから、またはタイマーがリセットされてからの時間を報告します。

  --- /feedback ---

- ( ) !["タイマー"という言葉をしゃべるバグ。](images/quiz_bug_timer.png)

  --- feedback ---

`タイマー`{:class="block3sensing"}ブロックは、 `調べる`{:class="block3sensing"}ブロックメニューにあります。 スプライトは「タイマー」という言葉をしゃべるのではありません。

  --- /feedback ---

--- /choices ---

--- /question ---





