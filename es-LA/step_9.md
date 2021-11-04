## Mejora tu juego

Si tienes tiempo, puedes agregar más niveles y más distracciones a tu juego. También puedes cambiar el objeto que se esconde y cambiar el texto en la pizarra.

Estos son los bloques que necesitarás para ocultar el insecto en un nuevo nivel:

```blocks3
when backdrop switches to [nuevo nivel v]

set size to [20] %

go to x: [0] y: [0] // arrastra para colocar el insecto primero

set [color v] effect to [50]
```

--- task ---

Para cada nivel necesitarás:
- Agregar un fondo
- Hacer clic en el panel Escenario, luego en la pestaña **Fondos**, luego arrastrar el nuevo fondo a la posición antes del fondo **final**
- Agregar un bloque `cuando el fondo cambie a`{:class="block3events"} para el nuevo fondo y añadir código para posicionar y ocultar el insecto

**Consejo:** Para arrastrar el insecto a un nuevo escondite, tendrás que "romper" el código para que el fondo no cambie cuando hagas clic en el insecto para posicionarlo en un nuevo nivel.

--- /task ---

--- task ---

Puedes agregar más loros o elegir otro objeto para que actúe como distracción.

Aquí está el código que usaste para el loro:
```blocks3
when flag clicked
set rotation style [left-right v] // no va boca abajo
point in direction [35] // número de -180 a 180
forever // sigue siendo molesto
move [10] steps // el número controla la velocidad
if on edge, bounce // permanecer en el Escenario
next costume // aletear
change [color v] effect by [5] // prueba 11 o 50
wait [0.25] seconds // prueba 0.1 o 0.5
end
```

**Consejo:** Puedes arrastrar el código del objeto **Parrot** a otro objeto para que sea más rápido crear otro objeto de distracción.

![Arrastrar código desde el área de Código a otro objeto en la lista de objetos.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Proyecto terminado
---

Puedes ver el [proyecto completo aquí](https://scratch.mit.edu/projects/486719939/){:target="_blank"}.

--- /collapse ---

--- save ---

