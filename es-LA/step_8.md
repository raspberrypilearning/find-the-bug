## Mejora tu juego

If you have time, you can add more levels and more distractions to your game. You could also change the sprite that is hiding and change the text on the chalkboard.

--- task ---

Juega tu juego y mira qué tan rápido puedes encontrar los insectos.

Is there someone else who can try your game? ¿Qué tan rápido pueden encontrar los insectos? They will not know where you have hidden them, so it might take them a bit longer!

Is there anything that you want to change?

You could:
- Make the parrot even more annoying
- Hacer los insectos más pequeños
- Cambiar el `efecto color`{:class="block3looks"} para camuflar el insecto en cada nivel
- Change the font or colour of the text

--- /task ---

### Add more levels

--- task ---

Estos son los bloques que necesitarás para ocultar el insecto en un nuevo nivel:

```blocks3
when backdrop switches to [new level v]

set size to [20] %

go to x: [0] y: [0] // drag to position the bug first

set [color v] effect to [50]
```

For each level, you will need to:
- Add a backdrop
- Click on the Stage pane, then on the **Backdrops** tab, then drag the new backdrop into position before the **end** backdrop
- Agregar un bloque `cuando el fondo cambie a`{:class="block3events"} para el nuevo fondo y añadir código para posicionar y ocultar el insecto

**Consejo:** Para arrastrar el insecto a un nuevo escondite, tendrás que "romper" el código para que el fondo no cambie cuando hagas clic en el insecto para posicionarlo en un nuevo nivel.

--- /task ---

### Add more distractions

--- task ---

Puedes agregar más loros o elegir otro objeto para que actúe como distracción.

Here is the code that you used for the parrot:

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

**Consejo:** Puedes arrastrar el código del objeto **Parrot** a otro objeto para que sea más rápido crear otro objeto de distracción.

![Dragging code from the Code area to another sprite in the Sprite list.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Proyecto terminado
---

Puedes ver el [proyecto terminado aquí](https://scratch.mit.edu/projects/486719939/){:target="_blank"}.

--- /collapse ---