## Ulepsz swój projekt

Jeśli masz czas, możesz dodać więcej poziomów i więcej rozpraszaczy do swojej gry. Możesz także zmienić ukrywającego się duszka i zmienić tekst na tablicy.

Oto bloki, których będziesz potrzebować, aby ukryć robaka na nowym poziomie:

```blocks3
when backdrop switches to [new level v]

set size to [20] %

go to x: [0] y: [0] // drag to position the bug first

set [color v] effect to [50]
```

--- task ---

Dla każdego poziomu musisz:
- Dodać tło
- Kliknąć na panel Sceny, potem zakładkę **Tła**, a następnie przeciągnąć nowe tło na miejsce przed tłem **koniec**
- Dodać blok `kiedy tło zmieni się na`{:class="block3events"} dla nowego tła oraz dodać kod, aby umieścić i ukryć robaka

**Wskazówka:** Aby przeciągnąć robaka do nowej kryjówki, będziesz musiał "złamać" kod, aby tło nie zmieniło się po kliknięciu robaka w celu ustawienia go na nowy poziom.

--- /task ---

--- task ---

Możesz dodać więcej papug lub wybrać innego duszka, który będzie odwracał uwagę.

Oto kod, którego użyłeś dla papugi:
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

**Wskazówka:** Możesz przeciągnąć kod duszka **Parrot** na innego duszka, aby przyspieszyć tworzenie kolejnego duszka rozpraszającego.

![Przeciągnięcie kodu z obszaru Skrypt do innego duszka na liście duszków.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Ukończony projekt
---

Tutaj możesz zobaczyć [ukończony projekt](https://scratch.mit.edu/projects/486719939/){:target="_blank"}.

--- /collapse ---

--- save ---

