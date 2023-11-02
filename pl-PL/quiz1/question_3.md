--- question ---
---
legend: Pytanie 3 z 3
---

Dodałaś/dodałeś ten skrypt do duszka **robaka**:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when backdrop switches to [koniec v]
set size to [100] % 
go to x: [0] y: [30] 
+ say (timer) 
```

W jaki sposób blok `powiedz`{:class="block3looks"} `stoper`{:class="block3sensing"} zmieni wygląd sceny, kiedy tło zmieni się na **koniec**?

--- choices ---

- ( ) ![Papuga mówiąca wartość stopera "4,52".](images/quiz_parrot_number.png)

  --- feedback ---

Przyjrzyj się jeszcze raz skryptowi i zastanów się, który duszek jest głównym bohaterem gry (papuga to tylko denerwujący rozpraszacz).

  --- /feedback ---

- ( ) ![Papuga mówiąca słowo "stoper".](images/quiz_parrot_timer.png)

  --- feedback ---

Blok `stoper`{:class="block3sensing"} znajduje się w sekcji bloków `Czujniki`{:class="block3sensing"}. Duszek nie wypowiada słowa „stoper”. Zastanów się również, który duszek wykonuje ten kod.

  --- /feedback ---

- (x) ![Robak mówiący wartość stopera "4,52".](images/quiz_bug_number.png)

  --- feedback ---

Tak. Blok `stoper`{:class="block3sensing"} podaje czas od uruchomienia projektu lub od zresetowania stopera. Blok `powiedz`{:class="block3looks"} tworzy dymek obok robaka.

  --- /feedback ---

- ( ) ![Robak mówiący słowo "stoper".](images/quiz_bug_timer.png)

  --- feedback ---

Blok `stoper`{:class="block3sensing"} znajduje się w sekcji bloków `Czujniki`{:class="block3sensing"}. Duszek nie wypowiada słowa „stoper”.

  --- /feedback ---

--- /choices ---

--- /question ---





