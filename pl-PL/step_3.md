## Pierwszy poziom

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Dodasz nowe tło jako pierwszy poziom gry i ukryjesz robaka.
</div>
<div>

![Tło Spotlight z robakiem.](images/first-level.png){:width="300px"}

</div>
</div>

--- task ---

Dodaj tło **Spotlight** z kategorii **Muzyka**.

![Ikona „Wybierz tło”.](images/backdrop-button.png)

--- /task ---

--- task ---

Kliknij **robaka** na liście duszków. Dodaj skrypt, aby zmienić `rozmiar`{:class="block3looks"} swojego robaka `kiedy tło zmieni się na Spotlight`{:class="block3events"}:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // malutki
```

--- /task ---

--- task ---

Kliknij kod, by zmienić rozmiar, a następnie przeciągnij swojego malutkiego robaka do kryjówki.

Dodaj kod, aby umieścić swojego robaka:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // malutki
+ go to x: [13] y: [132] // na kuli dyskotekowej
```

**Wybierz:** Jeśli wolisz, możesz wybrać inny rozmiar i miejsce.

--- /task ---

Kiedy zagrasz w grę i z sukcesem znajdziesz robaka, gra przełączy się na następne tło. Ponadto, aby rozpocząć grę, kliknij robaka na ekranie "start".

Blok `następne tło`{:class="block3looks"} przełącza na następne tło w kolejności, w jakiej tła są wymienione po kliknięciu zakładki **Tła** dla **Sceny**.

--- task ---

Dodaj skrypt do swojego duszka **robaka** by `grał dźwięk Pop`{:class="block3sound"} i przełącz się na `następne tło`{:class="block3looks"} `kiedy ten duszek zostanie kliknięty`{:class="block3events"}:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

Twój projekt musi rozpocząć się na ekranie "start".

--- task ---

Kliknij okienko Scena i dodaj ten kod do **Scena**:

![Tło Spotlight.](images/stage-image.png)

```blocks3
when flag clicked
switch backdrop to [start v] // ekran startowy
```

--- /task ---

--- task ---

**Test:** Kliknij zieloną flagę, aby przetestować swój projekt.

Zauważysz, że na ekranie "start" robak nadal będzie miał ustawienia ukrywania się w kryjówce z pierwszego poziomu (w tym przykładzie na kuli dyskotekowej).

**Wskazówka:** Po ostatnim tle na liście, `następne tło`{:class="block3looks"} przełączy się z powrotem na pierwsze tło.

--- /task ---

--- task ---

Kliknij na duszka **robaka** na liście duszków. Dodaj skrypt na `ustaw rozmiar`{:class="block3looks"} robaka, kiedy twoje `tło zmieni się na`{:class="block3events"} ekran `start`{:class="block3events"}:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // pełnowymiarowy
```

--- /task ---

--- task ---

Spróbuj umieścić robaka na ekranie "start".

Twój kod zmieni tło po kliknięciu robaka! Nie jest to pomocne, gdy próbujesz pozycjonować robaka.

--- /task ---

Aby rozwiązać ten problem, musisz zatrzymać działanie kodu po kliknięciu robaka.

--- task ---

Kliknij zieloną flagę, aby powrócić do ekranu "start".

Kliknij na duszka **bug** na liście duszków i przeciągnij bloki z dala od bloku `kiedy ten duszek kliknięty`{:class="block3events"}:

![Psucie skryptu.](images/breaking-script.png)

--- /task ---

--- task ---

Spróbuj ponownie umieścić robaka. Przeciągnij robaka na tablicę, pod tekstem:

![](images/bug-chalkboard.png)

Dodaj kod, aby upewnić się, że robak jest umieszczany na tablicy za każdym razem, `kiedy tło zmienia się na`{:class="block3events"} ekran `start`{:class="block3events"}:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // pełnowymiarowy
+ go to x: [0] y: [30] // na tablicy
```

--- /task ---

--- task ---

Połącz bloki z powrotem, tak aby bloki kodu ponownie znajdowały się poniżej bloku `kiedy ten duszek kliknięty`{:class="block3events"} blok:

![Blok „Kiedy ten duszek kliknięty” złączony z blokami „graj dźwięk” i „następne tło”.](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Kliknij zieloną flagę, aby przetestować swój projekt. Kliknij robaka, aby przejść do następnego tła. Robak powinien być duży na ekranie "start" i mały na poziomie "Spotlight".

--- collapse ---
---
title: Nic się nie dzieje po kliknięciu robaka
---

Czy zapomniałeś dołączyć kod z powrotem do bloku `kiedy ten duszek kliknięty`{:class="block3events"}?

--- /collapse ---

--- /task ---

--- save ---
