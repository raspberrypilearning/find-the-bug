## ಮೊದಲ ಹಂತ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ನಿಮ್ಮ ಆಟದ ಮೊದಲ ಹಂತವಾಗಿ ನೀವು ಹೊಸ ಹಿನ್ನೆಲೆಯನ್ನು ಸೇರಿಸುತ್ತೀರಿ ಮತ್ತು ದೋಷವನ್ನು ಅಡಗಿಸುತೀರೀ.
</div>
<div>

![The Spotlight backdrop with a bug.](images/first-level.png){:width="300px"}

</div>
</div>

--- task ---

**Music** ವರ್ಗದಿಂದ **Spotlight** ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ ಸೇರಿಸಿ.

![ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ ಐಕಾನ್ ಆಯ್ಕೆಮಾಡಿ.](images/backdrop-button.png)

--- /task ---

--- task ---

ಸ್ಪ್ರೈಟ್ ಪಟ್ಟಿಯಲ್ಲಿರುವ **bug** ಸ್ಪ್ರೈಟ್ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ. `ಹಿನ್ನೆಲೆಯು "Spotlight" ಗೆ ಬದಲಾವಣೆಗೊಂಡಾಗ `{:class="block3events"} ನಿಮ್ಮ ದೋಷದ `size`{:class="block3looks"} (ಗಾತ್ರ) ಬದಲಾಯಿಸಲು ಸ್ಕ್ರಿಪ್ಟ್ ಸೇರಿಸಿ:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
```

--- /task ---

--- task ---

ಗಾತ್ರವನ್ನು ಬದಲಾಯಿಸಲು ಕೋಡ್ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ, ನಂತರ ನಿಮ್ಮ ಸಣ್ಣ ದೋಷವನ್ನು ಅಡಗಿರುವ ಸ್ಥಳಕ್ಕೆ ಎಳೆಯಿರಿ.

ನಿಮ್ಮ ದೋಷವನ್ನು ಇರಿಸಲು ಕೋಡ್ ಸೇರಿಸಿ:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // tiny
+ go to x: [13] y: [132] // on the disco ball
```

**Choose:** ನೀವು ಬಯಸಿದಲ್ಲಿ ಬೇರೆ ಗಾತ್ರ ಮತ್ತು ಸ್ಥಳವನ್ನು ಆಯ್ಕೆ ಮಾಡಬಹುದು.

--- /task ---

ನೀವು ಆಟವನ್ನು ಆಡುವಾಗ ಮತ್ತು ದೋಷವನ್ನು ಯಶಸ್ವಿಯಾಗಿ ಕಂಡುಕೊಂಡಾಗ, ಆಟವು ಮುಂದಿನ ಹಿನ್ನೆಲೆಗೆ ಬದಲಾಗುತ್ತದೆ. ಅಲ್ಲದೆ, ಆಟವನ್ನು ಪ್ರಾರಂಭಿಸಲು, ನೀವು 'ಪ್ರಾರಂಭ' ಪರದೆಯ ಮೇಲೆ ದೋಷದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡುತ್ತೀರಿ.

`next backdrop`{:class="block3looks"} ಬ್ಲಾಕ್ **Stage**ನ **Backdrops** ಟ್ಯಾಬ್ ನಲ್ಲಿ ಬರುವ ಬ್ಯಾಕ್ಡ್ರಾಪ್ಸ್ ಪಟ್ಟಿಗಳಿಂದ ನಂತರ ಬರುವ ಬಕ್ಗ್ಡ್ರಾಪ್ ಗೆ ಬದಲಾಗುವುದು.

--- task ---

ನಿಮ್ಮ ಒಂದು ಸ್ಕ್ರಿಪ್ಟ್ **bug** ಸ್ಪ್ರೈಟ್ ಗೆ ಸೇರಿಸಿ. ಅದು `play a Pop sound`{:class="block3sound"} (ಪಾಪ್ ಧ್ವನಿಯನ್ನು ಕೇಳಲು) ಮತ್ತು `next backdrop`{:class="block3looks"} (ಮುಂದಿನ ಬ್ಯಾಕ್ಡ್ರಾಪ್ ಗೆ) `when this sprite is clicked`{:class="block3events"} ಸ್ಪ್ರೈಟ್ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಬದಲಾಯಿಸುವುದು:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್ 'ಸ್ಟಾರ್ಟ್' ಸ್ಕ್ರೀನ್ ನಲ್ಲಿ ಆರಂಭವಾಗಬೇಕು.

--- task ---

ಹಂತ ಫಲಕದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ಈ ಕೋಡ್ ಅನ್ನು **Stage**ಗೆ ಹಾಕಿ:

![ಸ್ಪಾಟ್‌ಲೈಟ್ ಹಿನ್ನೆಲೆ.](images/stage-image.png)

```blocks3
when flag clicked
switch backdrop to [start v] // 'start' screen
```

--- /task ---

--- task ---

**Test:** ನಿಮ್ಮ ಯೋಜನೆಯನ್ನು ಪರೀಕ್ಷಿಸಲು ಹಸಿರು ಧ್ವಜದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ.

'ಸ್ಟಾರ್ಟ್' ಸ್ಕ್ರೀನ್‌ನಲ್ಲಿ, ಬಗ್ ಮೊದಲ ಹಂತದಿಂದ ತನ್ನ ಅಡಗಿರುವ ಸ್ಥಳದಲ್ಲಿ ಅಡಗಿಸಲು ಸೆಟ್ಟಿಂಗ್‌ಗಳನ್ನು ಹೊಂದಿರುವುದನ್ನು ನೀವು ಗಮನಿಸಬಹುದು (ಈ ಉದಾಹರಣೆಯಲ್ಲಿ, ಡಿಸ್ಕೋ ಬಾಲ್‌ನಲ್ಲಿ).

**Tip:** ಪಟ್ಟಿಯಲ್ಲಿ ಕೊನೆಯ ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ ನಂತರ, `next backdrop`{:class="block3looks"} ಮೊದಲ ಬ್ಯಾಕ್‌ಡ್ರಾಪ್‌ಗೆ ಹಿಂತಿರುಗುತ್ತದೆ.

--- /task ---

--- task ---

ಸ್ಪ್ರೈಟ್ ಪಟ್ಟಿಯಲ್ಲಿರುವ **bug** ಸ್ಪ್ರೈಟ್ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ. ಒಂದು ಸ್ಕ್ರಿಪ್ಟ್ ಸೇರಿಸಿ `set the size`{:class="block3looks"} ದೋಷ ನಿಮ್ಮ ಮಾಡಿದಾಗ `backdrop switches to`{:class="block3events"} the `start`{:class="block3events"} ಸ್ಕ್ರೀನ್:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
```

--- /task ---

--- task ---

ಬಗ್ ಅನ್ನು 'ಸ್ಟಾರ್ಟ್' ಸ್ಕ್ರೀನ್‌ನಲ್ಲಿ ಇರಿಸಲು ಪ್ರಯತ್ನಿಸಿ.

ನೀವು ದೋಷದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ನಿಮ್ಮ ಕೋಡ್ ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ ಸ್ವಿಚ್ ಮಾಡುತ್ತದೆ! ನೀವು ದೋಷವನ್ನು ಇರಿಸಲು ಪ್ರಯತ್ನಿಸುತ್ತಿರುವಾಗ ಅದು ಸಹಾಯಕವಾಗುವುದಿಲ್ಲ.

--- /task ---

ಸಮಸ್ಯೆಯನ್ನು ಸರಿಪಡಿಸಲು, ನೀವು ದೋಷದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಕೋಡ್ ಚಾಲನೆಯಲ್ಲಿರುವುದನ್ನು ನಿಲ್ಲಿಸಬೇಕಾಗುತ್ತದೆ.

--- task ---

ಹಸಿರು ಬಾವುಟದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ 'ಸ್ಟಾರ್ಟ್' ಸ್ಕ್ರೀನ್ ಗೆ ಹಿಂತಿರುಗಿ.

**bug** ಸ್ಪ್ರೈಟ್ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ಈ ಸ್ಪ್ರೈಟ್`when this sprite clicked`{:class="block3events"}ಬ್ಲಾಕ್ ಅನ್ನು ದೂರ ಎಳೆಯಿರಿ:

![ಸ್ಕ್ರಿಪ್ಟ್ ಅನ್ನು ಮುರಿಯುವುದು.](images/breaking-script.png)

--- /task ---

--- task ---

ದೋಷವನ್ನು ಮತ್ತೆ ಇರಿಸಲು ಪ್ರಯತ್ನಿಸಿ. ಪಠ್ಯದ ಕೆಳಗೆ ಚಾಕ್‌ಬೋರ್ಡ್‌ಗೆ ದೋಷವನ್ನು ಎಳೆಯಿರಿ:

![](images/bug-chalkboard.png)

ನಿಮ್ಮ ಪ್ರತಿ ಬಾರಿ Chalkboard ಮೇಲೆ ದೋಷ ಸ್ಥಾನದಲ್ಲಿದೆ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಲು ಕೋಡ್ ಸೇರಿಸಿ `backdrop switches to`{:class="block3events"} `start`{:class="block3events"} ಸ್ಕ್ರೀನ್:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
+ go to x: [0] y: [30] // on the board
```

--- /task ---

--- task ---

ಈ ಸ್ಪ್ರೈಟ್`when this sprite clicked`{:class="block3events"}ಕ್ಕಿಂತ ಕೆಳಗಿರುವಂತೆ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಮತ್ತೆ ಜೋಡಿಸಿ:

!['ಈ ಸ್ಪ್ರೈಟ್ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ' ಬ್ಲಾಕ್ 'ಪ್ಲೇ ಸೌಂಡ್' ಮತ್ತು 'ನೆಕ್ಸ್ಟ್ ಬ್ಯಾಕ್‌ಡ್ರಾಪ್' ಬ್ಲಾಕ್‌ಗಳಿಗೆ ಸೇರಿಕೊಂಡಿತು.](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** ನಿಮ್ಮ ಯೋಜನೆಯನ್ನು ಪರೀಕ್ಷಿಸಲು ಹಸಿರು ಧ್ವಜದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ. ಮುಂದಿನ ಹಿನ್ನೆಲೆಗೆ ಹೋಗಲು ದೋಷದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ. ದೋಷವು 'ಪ್ರಾರಂಭ' ಪರದೆಯಲ್ಲಿ ದೊಡ್ಡದಾಗಿರಬೇಕು ಮತ್ತು 'ಸ್ಪಾಟ್‌ಲೈಟ್' ಮಟ್ಟದಲ್ಲಿ ಚಿಕ್ಕದಾಗಿರಬೇಕು.

--- collapse ---
---
title: ನಾನು ದೋಷದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಏನೂ ಆಗುವುದಿಲ್ಲ
---

ಈ ಸ್ಪ್ರೈಟ್`when this sprite clicked`{:class="block3events"} ಬ್ಲಾಕ್ ಅನ್ನು ಸೇರಲು ನೀವು ಮರೆತಿದ್ದೀರಾ?

--- /collapse ---

--- /task ---

--- save ---
