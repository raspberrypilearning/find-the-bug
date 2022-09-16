## 第1レベル

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Add a new backdrop as the first level in your game, and hide the bug.
</div>
<div>

![バグがいるSpotlightの背景。](images/first-level.png){:width="300px"}

</div>
</div>

### Add another Backdrop

--- task ---

**Spotlight** (スポットライト) の背景を **音楽** カテゴリから追加します。

![[背景を選ぶ] アイコン。](images/backdrop-button.png)

--- /task ---

### Resize the bug

--- task ---

スプライトリストにある **バグ** スプライトをクリックします。 `背景がSpotlightに切り替わった時`{:class="block3eventsを"}、バグの`大きさ`{:class="block3looks"}を変えるスクリプトを追加します:

![バグのスプライト。](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
```

--- /task ---

--- task ---

コードをクリックしてサイズを変更して、小さくなったバグを隠れ場所にドラッグします。

バグを配置するコードを追加します。

![バグのスプライト。](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**選ぶ:** お望みであれば、別のサイズや場所を選ぶことができます。

--- /task ---

### Move to the next Backdrop

ゲームをプレイしてバグを見つけると、ゲームは次の背景に切り替わります。 また、ゲームを開始するには、「スタート」画面でバグをクリックします。

`次の背景にする`{:class="block3looks"} ブロックは**ステージ**の**背景**タブをクリックしたときに並んでいる順序で次の背景に切り替えます。

--- task ---

`このスプライトが押されたとき`{:class="block3events"}に`Popの音を鳴らして`{:class="block3sound"}`次の背景にする`{:class="block3looks"}スクリプトを**バグ** スプライトに追加します:

![バグのスプライト。](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

### Make the game start with the Start Screen

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

**Tip:** After the last backdrop in the list, `next backdrop`{:class="block3looks"} will switch back to the first backdrop.

--- /task ---

--- task ---

Click on the **bug** sprite in the Sprite list. Add a script to `set the size`{:class="block3looks"} of the bug when your `backdrop switches to`{:class="block3events"} the `start`{:class="block3events"} screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
```

--- /task ---

### Change the position of the bug

--- task ---

Try to position the bug on the 'start' screen.

Your code will make the backdrop switch when you click on the bug! That is not helpful when you are trying to position the bug.

To fix the problem, you need to stop the code from running when you click on the bug.

--- /task ---

--- task ---

Click on the green flag to return to the 'start' screen.

Click on the **bug** sprite in the Sprite list and drag the blocks away from the `when this sprite clicked`{:class="block3events"} block:

![Breaking the script.](images/breaking-script.png)

--- /task ---

--- task ---

Try to position the bug again. Drag the bug onto the chalkboard, below the text:

![The bug on the start screen](images/bug-chalkboard.png)

Add code to make sure that the bug is positioned on the chalkboard every time your `backdrop switches to`{:class="block3events"} the `start`{:class="block3events"} screen:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
+ go to x: [0] y: [30] // on the board
```

--- /task ---

--- task ---

Join the blocks back together so that the code blocks are under the `when this sprite clicked`{:class="block3events"} block again:

![The 'when this sprite clicked' block joined to the 'play sound' and 'next backdrop' blocks.](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Click on the green flag to test your project. Click on the bug to move to the next backdrop. The bug should be big on the 'start' screen and small on the 'Spotlight' level.

--- collapse ---
---
title: バグをクリックしても何も起こりません
---

Did you forget to join the code back to the `when this sprite clicked`{:class="block3events"} block?

--- /collapse ---

--- /task ---