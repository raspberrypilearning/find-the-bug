## ಗಿಣಿ ವ್ಯಾಕುಲತೆ

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ದೋಷವನ್ನು ಹುಡುಕಲು ಮತ್ತು ಕ್ಲಿಕ್ ಮಾಡಲು ಆಟಗಾರರಿಗೆ ಕಷ್ಟವಾಗುವಂತೆ ಮಾಡಲು, ಕಿರಿಕಿರಿಗೊಳಿಸುವ ಗಿಳಿಯನ್ನು ನೀವು ಅವರ ಗಮನವನ್ನು ಸೆಳೆಯಲು ಸೇರಿಸುತ್ತೀರಿ. 
</div>
<div>

![ವೇದಿಕೆಯಲ್ಲಿ ವರ್ಣರಂಜಿತ ಗಿಣಿ.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

--- task ---

**Parrot** ಸ್ಪ್ರೈಟ್ ಅನ್ನು ಅಳಿಸಿ.

![ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ ಐಕಾನ್ ಆಯ್ಕೆಮಾಡಿ.](images/sprite-button.png)

--- /task ---

[Catch the bus](https://projects.raspberrypi.org/en/projects/catch-the-bus){:target="_blank"} ಯೋಜನೆಯಲ್ಲಿ, ನೀವು `repeat`{:class="block3control"} ಲೂಪ್ ಅನ್ನು ಬಳಸಿದ್ದೀರಿ.

ನೀವು ಇಲ್ಲಿ ಬೇರೆ ಲೂಪ್ ಅನ್ನು ಬಳಸುತ್ತೀರಿ. `forever`{:class="block3control"} ಲೂಪ್ ಅದರೊಳಗೆ ಕೋಡ್ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಪದೇ ಪದೇ ಚಲಿಸುತ್ತದೆ. ಇದು ಕಿರಿಕಿರಿ ಗಿಣಿಗೆ ಸೂಕ್ತವಾದ ಲೂಪ್ ಆಗಿದ್ದು ಅದು ಸುತ್ತಲೂ ಹಾರುವುದನ್ನು ಮತ್ತು ದಾರಿಯಲ್ಲಿ ಹೋಗುವುದನ್ನು ನಿಲ್ಲಿಸುವುದಿಲ್ಲ.

--- task ---

ಗಮನಹರಿಸುವ ರೀತಿಯಲ್ಲಿ ಗಿಳಿಯನ್ನು ಸುತ್ತುವಂತೆ ಮಾಡಲು ಕೋಡ್ ಸೇರಿಸಿ:

![ರಾಕೆಟ್ ಸ್ಪ್ರೈಟ್.](images/parrot-sprite.png)


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

**Test:** ನಿಮ್ಮ ಯೋಜನೆಯನ್ನು ಪರೀಕ್ಷಿಸಲು ಹಸಿರು ಧ್ವಜದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ. ನೀವು ದೋಷವನ್ನು ಎಲ್ಲಿ ಮರೆಮಾಡಿದ್ದೀರಿ ಎಂದು ನಿಮಗೆ ನೆನಪಿದೆಯೇ?

ಸ್ಕ್ರಾಚ್‌ನಲ್ಲಿ, ಚಾಲನೆಯಲ್ಲಿರುವ ಕೋಡ್ ಹಳದಿ ರೂಪರೇಖೆಯೊಂದಿಗೆ ಹೊಳೆಯುತ್ತದೆ:

![](images/running-code.png)

**Tip:** ನೀವು ಕೋಡಿಂಗ್ ಮಾಡುವಾಗ ಗಿಳಿ ತುಂಬಾ ಕಿರಿಕಿರಿ ಉಂಟುಮಾಡಿದರೆ, ಕೋಡ್ ಚಾಲನೆಯಲ್ಲಿರುವುದನ್ನು ನಿಲ್ಲಿಸಲು ನೀವು ಸ್ಟೇಜ್ ಮೇಲಿನ ಕೆಂಪು ಸ್ಟಾಪ್ ಬಟನ್ ಅನ್ನು ಕ್ಲಿಕ್ ಮಾಡಬಹುದು.

--- /task ---

--- save ---
