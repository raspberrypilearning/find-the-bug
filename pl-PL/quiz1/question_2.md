--- question ---
---
legend: Pytanie 2 z 3
---

Użyłaś/użyłeś pętli `zawsze`{:class="block3control"}, aby duszek **Parrot** latał w irytujący sposób.

Próbowaliśmy dodać kolejnego rozpraszającego duszka, ale porusza się on tylko raz, gdy klikniemy zieloną flagę, a potem się zatrzymuje. Jak możemy to naprawić?

![Duszek Rocket.](images/rocket-sprite.png)

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

- ( ) Zmienić liczbę w bloku `przesuń o`{:class="block3motion"}

  --- feedback ---

Jeśli zmienisz liczbę w bloku `przesuń o`{:class="block3motion"} to zmienisz długość ruchu duszka po kliknięciu zielonej flagi, ale ta zmiana nie sprawi, że rakieta poruszy się więcej niż raz.

  --- /feedback ---

- ( ) Usuń blok `jeżeli na brzegu, odbij się`{:class="block3motion"}

  --- feedback ---

Blok `jeżeli na brzegu, odbij się`{:class="block3motion"} powoduje, że duszek odbija się od krawędzi sceny. Jeśli go usuniesz, rakieta utknie na brzegu sceny.

  --- /feedback ---

- ( ) Dodaj kolejny blok `zawsze`{:class="block3control"}

--- feedback ---

Skrypt może mieć tylko jeden blok `zawsze`{:class="block3control"}. Czy zauważyłaś/zauważyłeś, że nie możesz dodać bloku pod blokiem `zawsze`{:class="block3control"}?

--- /feedback ---

- (x) Przeciągnij blok `przesuń o`{:class="block3motion"} wewnątrz pętli `zawsze`{:class="block3control"}

  --- feedback ---

  Tak! Duszek porusza się tylko raz. Jeśli umieścisz blok `przesuń o`{:class="block3motion"} wewnątrz pętli `zawsze`{:class="block3control"}, duszek będzie się poruszał, dopóki nie zatrzymasz skryptu.

  --- /feedback ---

--- /choices ---

--- /question ---
