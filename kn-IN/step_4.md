## ಗಿಣಿ ಗಮನಭಂಗ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ದೋಷವನ್ನು ಹುಡುಕಿ ಕ್ಲಿಕ್ ಮಾಡಲು ಆಟಗಾರರಿಗೆ ಕಷ್ಟವಾಗುವಂತೆ ಮಾಡಲು, ನೀವು ಅವರ ಗಮನವನ್ನು ಸೆಳೆಯಲು ಕಿರಿಕಿರಿ ಉಂಟುಮಾಡುವ ಗಿಳಿಯನ್ನು ಸೇರಿಸುತ್ತೀರಿ. 
</div>
<div>

![ವೇದಿಕೆಯಲ್ಲಿ ವರ್ಣರಂಜಿತ ಗಿಣಿ.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

### Add the Parrot sprite

--- task ---

**Parrot** ಸ್ಪ್ರೈಟ್ ಅನ್ನು ಸೇರಿಸಿ.

!['Choose a Sprite' ಐಕಾನ್.](images/sprite-button.png)

--- /task ---

### Animate the Parrot sprite

[Catch the bus](https://projects.raspberrypi.org/en/projects/catch-the-bus){:target="_blank"} ಪ್ರಾಜೆಕ್ಟ್‌ನಲ್ಲಿ, ನೀವು `repeat`{:class="block3control"} ಲೂಪ್ ಅನ್ನು ಬಳಸಿದ್ದೀರಿ.

ನೀವು ಇಲ್ಲಿ ಬೇರೆ ಲೂಪ್ ಅನ್ನು ಬಳಸುತ್ತೀರಿ. `forever`{:class="block3control"} ಲೂಪ್ ಅದರೊಳಗೆ ಕೋಡ್ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಪದೇ ಪದೇ ರನ್‌ ಮಾಡುತ್ತದೆ. ಇದು ಸುತ್ತಲೂ ಹಾರುವುದನ್ನು ಮತ್ತು ದಾರಿಯಲ್ಲಿಗೆ ಅಡ್ಡ ಹೋಗುವುದನ್ನು ನಿಲ್ಲಿಸದ ಕಿರಿಕಿರಿ ಗಿಣಿಗೆ ಸೂಕ್ತವಾದ ಲೂಪ್ ಆಗಿದೆ.

--- task ---

Add code to make the parrot flap around in a distracting way. Look at the comments on the code blocks for some different numbers to try:

![Parrot ಸ್ಪ್ರೈಟ್.](images/parrot-sprite.png)


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

--- /task ---

--- task ---

**ಪರೀಕ್ಷೆ:** ಹಸಿರು ಬಾವುಟದ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ ಮತ್ತೆ ಪರೀಕ್ಷೆ ಮಾಡಿ. ನೀವು ದೋಷವನ್ನು ಎಲ್ಲಿ ಮರೆಮಾಡಿದ್ದೀರಿ ಎಂದು ನಿಮಗೆ ನೆನಪಿದೆಯೇ?

Scratch ನಲ್ಲಿ, ಚಾಲನೆಯಲ್ಲಿರುವ ಕೋಡ್ ಹಳದಿ ಬಾಹ್ಯರೇಖೆಯೊಂದಿಗೆ ಹೊಳೆಯುತ್ತದೆ:

![](images/running-code.png)

**ಸಲಹೆ:** ನೀವು ಕೋಡಿಂಗ್ ಮಾಡುವಾಗ ಗಿಣಿ ತುಂಬಾ ಕಿರಿಕಿರಿ ಉಂಟುಮಾಡಿದರೆ, ಕೋಡ್ ಚಾಲನೆಯಲ್ಲಿರುವುದನ್ನು ನಿಲ್ಲಿಸಲು ನೀವು ಸ್ಟೇಜ್ ಮೇಲಿನ ಕೆಂಪು ಸ್ಟಾಪ್ ಬಟನ್ ಅನ್ನು ಕ್ಲಿಕ್ ಮಾಡಬಹುದು.

--- /task ---

