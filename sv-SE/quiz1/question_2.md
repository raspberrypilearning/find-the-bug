--- question ---
---
legend: Fråga 2 av 3
---

Du använde en `för alltid`{:class="block3control"}-loop för att få **papegoja**sprajten att flyga runt på ett irriterande sätt.

Vi har försökt lägga till ytterligare en distraktionssprajt men den rör sig bara en gång när vi klickar på den gröna flaggan. Hur kan vi fixa detta?

![Raketsprajten.](images/rocket-sprite.png)

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

- ( ) Ändra talet i `gå`{:class="block3motion"}blocket

  --- feedback ---

Om du ändrar talet i `gå`{:class="block3motion"}blocket kommer du att ändra hur långt sprajten rör sig när den gröna flaggan klickas men du kommer inte få raketen att fortsätta röra sig.

  --- /feedback ---

- ( ) Ta bort `om på kanten, studsa`{:class="block3motion"}-blocket

  --- feedback ---

`om på kanten, studsa`{:class="block3motion"}-blocket får sprajten att studsa på scenens kant. Om du tog bort den skulle raketen fastna vid scenens kant.

  --- /feedback ---

- ( ) Lägg till ett till `för alltid`{:class="block3control"}block

--- feedback ---

Din kod kan bara ha ett `för alltid`{:class="block3control"}-block. Har du märkt att du inte kan lägga till ett block under ett `för alltid`{:class="block3control"}-block?

--- /feedback ---

- (x) Dra `gå`{:class="block3motion"}blocket in i `för alltid`{:class="block3control"}-loopen

  --- feedback ---

  Ja! Sprajten rör sig bara en gång. Om du flyttar `gå`{:class="block3motion"}blocket inuti `för alltid`{:class="block3control"}-loopen, kommer sprajten att fortsätta röra sig tills du stoppar ditt projekt.

  --- /feedback ---

--- /choices ---

--- /question ---
