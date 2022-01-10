## First level

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
You will add a new backdrop as the first level in your game, and hide the bug.
</div>
<div>

![The Spotlight backdrop with a bug.](images/first-level.png){:width="300px"}

</div>
</div>

--- task ---

**Spotlight** (スポットライト) の背景を **音楽** カテゴリから追加します。

![The 'Choose a Backdrop' icon.](images/backdrop-button.png)

--- /task ---

--- task ---

スプライトリストにある **バグ** スプライトをクリックします。 `背景がSpotlightに切り替わった時`{:class="block3eventsを"}、バグの`大きさ`{:class="block3looks"}を変えるスクリプトを追加します:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
```

--- /task ---

--- task ---

Click on the code to change the size, then drag your tiny bug to a hiding place.

Add code to position your bug:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**Choose:** You can choose a different size and location, if you prefer.

--- /task ---

When you play the game and you successfully find the bug, the game will switch to the next backdrop. Also, to start the game, you will click on the bug on the 'start' screen.

The `next backdrop`{:class="block3looks"} block switches to the next backdrop in the order in which the backdrops are listed when you click on the **Backdrops** tab for the **Stage**.

--- task ---

`このスプライトが押されたとき`{:class="block3events"}に`Popの音を鳴らして`{:class="block3sound"}`次の背景にする`{:class="block3looks"}スクリプトを**バグ** スプライトに追加します:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

Your project needs to start on the 'start' screen.

--- task ---

Click on the Stage pane and add this code to the **Stage**:

![The Spotlight backdrop.](images/stage-image.png)

```blocks3
when flag clicked
switch backdrop to [start v] // 'start' screen
```

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project.

You will notice that on the 'start' screen, the bug will still have the settings to hide in its hiding place from the first level (in this example, on the disco ball).

**ヒント:** リストの最後の背景の後、 `次の背景`{:class="block3looks"}で最初の背景に戻ります。

--- /task ---

--- task ---

Click on the **bug** sprite in the Sprite list. Add a script to `set the size`{:class="block3looks"} of the bug when your `backdrop switches to`{:class="block3events"} the `start`{:class="block3events"} screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
```

--- /task ---

--- task ---

Try to position the bug on the 'start' screen.

Your code will make the backdrop switch when you click on the bug! バグを配置しようとしているとき、これは不便です。

--- /task ---

To fix the problem, you need to stop the code from running when you click on the bug.

--- task ---

Click on the green flag to return to the 'start' screen.

Click on the **bug** sprite in the Sprite list and drag the blocks away from the `when this sprite clicked`{:class="block3events"} block:

![スクリプトを壊す。](images/breaking-script.png)

--- /task ---

--- task ---

Try to position the bug again. Drag the bug onto the chalkboard, below the text:

![](images/bug-chalkboard.png)

`背景が`{:class="block3events"} `スタート`{:class="block3events"}画面<0>になるたびに</0>{:class="block3events"}、バグが必ず黒板に配置されるコードを追加します。

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
+ go to x: [0] y: [30] // on the board
```

--- /task ---

--- task ---

コードブロックがもう一度`このスプライトが押されたとき`{:class="block3events"}ブロックの下にになるように、引き離したブロックをくっつけます。

![The 'when this sprite clicked' block joined to the 'play sound' and 'next backdrop' blocks.](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project. Click on the bug to move to the next backdrop. The bug should be big on the 'start' screen and small on the 'Spotlight' level.

--- collapse ---
---
title: バグをクリックしても何も起こりません
---

`このスプライトが押されたとき`{:class="block3events"}ブロックにコードブロックをつなぎ戻すのを忘れてしまいましたか？

--- /collapse ---

--- /task ---

--- save ---
