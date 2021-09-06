--- question ---
---
legend: Question 3 of 3
---

You added this script to the **bug** sprite:

![The bug sprite.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % 
go to x: [0] y: [30] 
+ say (timer) 
```

How does the `say`{:class="block3looks"} `timer`{:class="block3sensing"} block make the Stage look when the backdrop switches to **end**?

--- choices ---

- ( ) ![A parrot saying the timer value "4.52".](images/quiz_parrot_number.png)

  --- feedback ---

Have a look at the script again, and think about which sprite is the main character of the game (the parrot is just an annoying distraction).

  --- /feedback ---

- ( ) ![A parrot saying the word "timer".](images/quiz_parrot_timer.png)

  --- feedback ---

The `timer`{:class="block3sensing"} block comes from the `Sensing`{:class="block3sensing"} blocks menu. The sprite does not say the word "timer". Also, think about which sprite uses this code.

  --- /feedback ---

- (x) ![A bug saying the timer value "4.52".](images/quiz_bug_number.png)

  --- feedback ---

Yes. The `timer`{:class="block3sensing"} block reports the time since the project started, or since the timer reset. 

  --- /feedback ---

- ( ) ![A bug saying the word "timer".](images/quiz_bug_timer.png)

  --- feedback ---
  
The `timer`{:class="block3sensing"} block comes from the `Sensing`{:class="block3sensing"} blocks menu. The sprite does not say the word "timer".

  --- /feedback ---

--- /choices ---

--- /question ---





