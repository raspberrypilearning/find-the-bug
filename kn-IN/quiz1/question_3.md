--- question ---
---
legend: ಪ್ರಶ್ನೆ 3 ರಲ್ಲಿ 3
---

ನೀವು ಈ ಸ್ಕ್ರಿಪ್ಟ್ ಅನ್ನು **bug** ಸ್ಪ್ರೈಟ್‌ಗೆ ಸೇರಿಸಿದ್ದೀರಿ:

![ಬಗ್ ಸ್ಪ್ರೈಟ್.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % 
go to x: [0] y: [30] 
+ say (timer) 
```

ಬ್ಯಾಕ್‌ಡ್ರಾಪ್ **end** ಬದಲಾದಾಗ, `say`{:class="block3looks"} `timer`{:class="block3sensing"} ಬ್ಲಾಕ್‌ ಸ್ಟೇಜ್‌ ಹೇಗೆ ಕಾಣಿಸುವಂತೆ ಮಾಡುತ್ತದೆ?

--- choices ---

- ( ) ![ಟೈಮರ್ ಮೌಲ್ಯವನ್ನು ಹೇಳುವ ಗಿಣಿ "4.52".](images/quiz_parrot_number.png)

  --- feedback ---

ಬರಹವನ್ನು ಮತ್ತೊಮ್ಮೆ ನೋಡಿ, ಮತ್ತು ಯಾವ ಸ್ಪ್ರೈಟ್ ಆಟದ ಮುಖ್ಯ ಪಾತ್ರವಾಗಿದೆ ಎಂದು ಯೋಚಿಸಿ (ಗಿಳಿ ಕೇವಲ ಕಿರಿಕಿರಿಗೊಳಿಸುವ ಗಮನಭಂಗವಷ್ಟೆ).

  --- /feedback ---

- ( ) ![ಗಿಣಿ "timer" ಪದವನ್ನು ಹೇಳುತ್ತಿದೆ.](images/quiz_parrot_timer.png)

  --- feedback ---

`timer`{:class="block3sensing"} ಬ್ಲಾಕ್ `Sensing`{:class="block3sensing"} ಬ್ಲಾಕ್ಸ್‌ ಮೆನುವಿನಿಂದ ಬರುತ್ತದೆ. ಸ್ಪ್ರೈಟ್ "ಟೈಮರ್" ಪದವನ್ನು ಹೇಳುವುದಿಲ್ಲ. ಅಲ್ಲದೆ, ಈ ಕೋಡ್ ಅನ್ನು ಯಾವ ಸ್ಪ್ರೈಟ್ ಬಳಸುತ್ತದೆ ಎಂದು ಯೋಚಿಸಿ.

  --- /feedback ---

- (x) ![ಟೈಮರ್ ಮೌಲ್ಯ "4.52" ವನ್ನು ಹೇಳುವ ಹುಳ.](images/quiz_bug_number.png)

  --- feedback ---

ಹೌದು. `timer`{:class="block3sensing"} ಪ್ರಾಜೆಕ್ಟ್ ಪ್ರಾರಂಭವಾದ ಸಮಯದಿಂದ ಅಥವಾ ಟೈಮರ್ ಮರುಹೊಂದಿಸಿದ ನಂತರ ಸಮಯ ವರದಿ ಮಾಡುತ್ತದೆ. The `say`{:class="block3looks"} block creates a speech bubble next to bug.

  --- /feedback ---

- ( ) !["timer" ಪದವನ್ನು ಹೇಳುವ ಹುಳ.](images/quiz_bug_timer.png)

  --- feedback ---

`timer`{:class="block3sensing"} ಬ್ಲಾಕ್ `Sensing`{:class="block3sensing"} ಬ್ಲಾಕ್ಸ್ ಮೆನುವಿನಿಂದ ಬರುತ್ತದೆ. ಸ್ಪ್ರೈಟ್ "ಟೈಮರ್" ಪದವನ್ನು ಹೇಳುವುದಿಲ್ಲ.

  --- /feedback ---

--- /choices ---

--- /question ---





