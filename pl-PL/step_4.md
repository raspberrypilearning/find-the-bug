## Rozpraszająca papuga

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Aby utrudnić graczom odnalezienie robaka, dodasz irytującą papugę, aby odwrócić ich uwagę. 
</div>
<div>

![Kolorowa papuga na Scenie.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

### Dodaj duszka papugi

--- task ---

Dodaj duszka **Parrot**.

![Ikona „Wybierz duszka”.](images/sprite-button.png)

--- /task ---

### Animuj duszka papugi

W projekcie [Złap autobus](https://projects.raspberrypi.org/en/projects/catch-the-bus){:target="_blank"} korzystaliśmy z pętli `powtórz`{:class="block3control"}.

Tutaj użyjesz innej pętli. Pętla `zawsze`{:class="block3control"} uruchamia bloki kodu wewnątrz niej raz za razem. To idealna pętla dla irytującej papugi, która nie przestaje latać, przeszkadzając graczowi.

--- task ---

Dodaj kod, aby papuga trzepotała skrzydłami w rozpraszający sposób: Look at the comments on the code blocks for some different numbers to try:

![Duszek Parrot.](images/parrot-sprite.png)


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

**Test:** Kliknij zieloną flagę i ponownie przetestuj swój projekt. Czy pamiętasz, gdzie jest robak?

W Scratchu uruchomiony kod jest podświetlony żółtym konturem:

![](images/running-code.png)

**Wskazówka:** Jeśli papuga stanie się zbyt denerwująca podczas kodowania, możesz kliknąć czerwony przycisk zatrzymania nad sceną, aby zatrzymać wykonywanie kodu.

--- /task ---

