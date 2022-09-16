--- question ---
---
legend: ಪ್ರಶ್ನೆ 3 ರಲ್ಲಿ 2
---

ನೀವು **Parrot** ಸ್ಪ್ರೈಟ್ ಅನ್ನು ಕಿರಿಕಿರಿ ಉಂಟುಮಾಡುವ ರೀತಿಯಲ್ಲಿ ಹಾರುವಂತೆ ಮಾಡಲು `forever`{:class="block3control"} ಲೂಪ್ ಉಪಯೋಗ ಮಾಡಿದ್ದೀರಿ.

ನಾವು ಇನ್ನೊಂದು ಗಮನಭಂಗ ಮಾಡುವ ಸ್ಪ್ರೈಟ್‌ ಸೇರಿಸಲು ಪ್ರಯತ್ನಿಸಿದ್ದೇವೆ, ಆದರೆ ಅದು ನಾವು ಹಸಿರು ಧ್ವಜವನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಒಮ್ಮೆ ಚಲಿಸುತ್ತದೆ ಮತ್ತು ನಂತರ ನಿಂತುಹೋಗುತ್ತದೆ. ನಾವು ಅದನ್ನು ಹೇಗೆ ಸರಿಪಡಿಸಬಹುದು?

![The Rocket sprite.](images/rocket-sprite.png)

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

- ( ) `move`{:class="block3motion"} ಬ್ಲಾಕ್ ನಲ್ಲಿರುವ ಸಂಖ್ಯೆಯನ್ನು ಬದಲಾಯಿಸಿ

  --- feedback ---

ನೀವು `move`{:class="block3motion"} ಬ್ಲಾಕ್‌ನಲ್ಲಿ ಸಂಖ್ಯೆಯನ್ನು ಬದಲಾಯಿಸಿದರೆ, ಹಸಿರು ಧ್ವಜವನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಸ್ಪ್ರೈಟ್ ಎಷ್ಟು ದೂರ ಚಲಿಸುತ್ತದೆ ಎಂಬುದನ್ನು ನೀವು ಬದಲಾಯಿಸುತ್ತೀರಿ, ಆದರೆ ಈ ಬದಲಾವಣೆಯು ರಾಕೇಟ್‌ನ್ನು ಚಲಿಸುವಂತೆ ಮಾಡುವುದಿಲ್ಲ.

  --- /feedback ---

- ( ) `if on edge, bounce`{:class="block3motion"} ಬ್ಲಾಕ್ ಅನ್ನು ತೆಗೆಯಿರಿ

  --- feedback ---

`if on edge, bounce`{:class="block3motion"} ಬ್ಲಾಕ್ ಸ್ಪ್ರೈಟ್ ಅನ್ನು ವೇದಿಕೆಯ ಅಂಚಿನಿಂದ ಪುಟಿಯುವಂತೆ ಮಾಡುತ್ತದೆ. ನೀವು ಅದನ್ನು ತೆಗೆದರೆ, ರಾಕೆಟ್ ವೇದಿಕೆಯ ಅಂಚಿನಲ್ಲಿ ಸಿಲುಕಿಕೊಳ್ಳುತ್ತದೆ.

  --- /feedback ---

- ( ) ಮತ್ತೊಂದು `forever`{:class="block3control"} ಬ್ಲಾಕ್ ಅನ್ನು ಸೇರಿಸಿ

--- feedback ---

ಒಂದು ಸ್ಕ್ರಿಪ್ಟ್ ಒಂದೇ ಒಂದು `forever`{:class="block3control"} ಬ್ಲಾಕ್ ಹೊಂದಿರಬಹುದು. ನೀವು `forever`{:class="block3control"} ಕೆಳಗೆ ಬ್ಲಾಕ್ ಅನ್ನು ಸೇರಿಸಲು ಸಾಧ್ಯವಿಲ್ಲ ಎಂದು ನೀವು ಗಮನಿಸಿದ್ದೀರಾ?

--- /feedback ---

- (x) `move`{:class="block3motion"} ಬ್ಲಾಕ್ ಅನ್ನು `forever`{:class="block3control"} ಲೂಪ್ ಒಳಗೆ ಎಳೆಯಿರಿ

  --- feedback ---

  ಹೌದು! ಸ್ಪ್ರೈಟ್ ಒಮ್ಮೆ ಮಾತ್ರ ಚಲಿಸುತ್ತದೆ. ನೀವು `move`{:class="block3motion"} ಬ್ಲಾಕ್ ಅನ್ನು `forever`{:class="block3control"} ಲೂಪ್ ಒಳಗೆ ಚಲಿಸಿದರೆ, ನೀವು ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ನ್ನು ನಿಲ್ಲಿಸುವವರೆಗೂ ಸ್ಪ್ರೈಟ್ ಚಲಿಸುತ್ತಲೇ ಇರುತ್ತದೆ.

  --- /feedback ---

--- /choices ---

--- /question ---
