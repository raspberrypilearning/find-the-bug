## Drugi poziom

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Wybierzesz tło, aby stworzyć drugi poziom dla swojej gry i sprawisz, że robak będzie trudny do znalezienia. 
</div>
<div>

![Scena uliczna z ukrytym robakiem.](images/second-level.png){:width="300px"}

</div>
</div>

--- task ---

**Wybierz:** Wybierz tło dla drugiego poziomu. Wybraliśmy tło **Urban**, ale możesz wybrać to, które najbardziej Ci się podoba.

![](images/insert-urban-backdrop.png)

**Wskazówka:** Pamiętaj, że tła z dużą ilością kolorów i detali utrudnią znalezienie robaka. Jak trudną zrobisz swoją grę?

--- /task ---

Aby móc przeciągnąć robaka w nowe miejsce, musisz zatrzymać działanie skryptu `kiedy ten duszek kliknięty`{:class="block3events"}.

--- task ---

Przeciągnij bloki z dala od bloku `kiedy duszek kliknięty`{:class="block3events"}, aby zatrzymać ich działanie po kliknięciu robaka:

![](images/breaking-script.png)

--- /task ---

Twój robak musi być trudny do znalezienia, gdy zmieni się tło. Możesz zmienić rozmiar robaka, aby utrudnić jego znalezienie.

--- task ---

Dodaj kod na `ustaw rozmiar`{:class="block3looks"} robaka dla drugiego poziomu:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // wybierz swoje tło
set size to [20] % // spróbuj inny rozmiar 
```

**Test:** Kliknij swój nowy skrypt, aby go uruchomić.

--- /task ---

--- task ---

Przeciągnij swojego robaka na scenę do dobrej kryjówki dla tego poziomu.

![Duszek ukryty w witrynie sklepowej na środku tła.](images/hidden-urban-backdrop.png)

--- /task ---

Umieść swojego robaka w kryjówce.

--- task ---

Dodaj blok `idź do x: y:`{:class="block3motion"} do swojego kodu:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // spróbuj inny rozmiar 
+ go to x: [24] y: [13] // w witrynie sklepowej
```

--- /task ---

--- task ---

Dołącz bloki z powrotem do bloku `kiedy duszek kliknięty`{:class="block3events"} tak, aby po kliknięciu robaka tło zmieniło się na `następne tło`{:class="block3looks"}:

![](images/fixed-script.png)

--- /task ---

--- task ---

**Test:** Kliknij zieloną flagę, aby przetestować swój projekt.

--- /task ---

Twój robak może teraz znajdować się przed papugą.

--- task ---

Dodaj skrypt, aby upewnić się, że robak jest zawsze na `spodzie`{class="block3looks"}:

![Duszek robaka.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Teraz twój robak zawsze będzie z tyłu, nawet jeśli będziesz musiał zmienić jego pozycję.

--- /task ---

--- save ---
