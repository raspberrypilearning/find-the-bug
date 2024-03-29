## Primer nivel

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Agregarás un nuevo fondo como primer nivel en tu juego y ocultarás el insecto.
</div>
<div>

![El fondo spotlight con un insecto.](images/first-level.png){:width="300px"}

</div>
</div>

### Agrega otro fondo

--- task ---

Agrega el fondo **spotlight** de la categoría **música**.

![El icono 'elige un fondo'.](images/backdrop-button.png)

--- /task ---

### Redimensiona el insecto

--- task ---

Haz clic en el objeto **insecto** en la lista de Objetos. Añade un script para cambiar el `tamaño`{:class="block3looks"} de tu insecto `cuando el fondo cambie a Spotlight`{:class="block3events"}:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // diminuto
```

--- /task ---

--- task ---

Haz clic en el código para cambiar el tamaño, luego arrastra tu pequeño insecto a un escondite.

Añade código para posicionarlo:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v]
set size to [20] % // diminuto
+ go to x: [13] y: [132] // en la bola de discoteca
```

**Elige:** Puedes elegir un tamaño y una ubicación diferentes, si lo prefieres.

--- /task ---

### Muévete al siguiente fondo

Cuando juegas y encuentras con éxito el insecto, el juego cambiará al siguiente fondo. Además, para iniciar el juego, harás clic en el error en la pantalla de "inicio".

El bloque `siguiente fondo`{:class="block3looks"} cambia al siguiente fondo en el orden en que se enumeran cuando haces clic en la pestaña **fondos** para el **escenario**.

--- task ---

Añade un script a tu objeto **insecto** para `reproducir un sonido Pop`{:class="block3sound"} y cambiar al `siguiente fondo`{:class="block3looks"} `al hacer clic en este objeto`{:class="block3events"}:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when this sprite clicked
play sound [Pop v] until done
next backdrop
```

--- /task ---

### Haz que el juego comience con la pantalla de inicio

--- task ---

Haz clic en el panel escenario y agrega este código al **escenario**:

![El fondo Spotlight.](images/stage-image.png)

```blocks3
when flag clicked
switch backdrop to [inicio v] // pantalla de 'inicio'
```

--- /task ---

--- task ---

**Prueba:** Haz clic en la bandera verde para probar tu proyecto.

Notarás que en la pantalla de 'inicio', el insecto aún tendrá la configuración para esconderse en su escondite del primer nivel (en este ejemplo, en la bola de discoteca).

**Consejo:** Después del último fondo de la lista, `siguiente fondo`{:class="block3looks"} volverá al primero.

--- /task ---

--- task ---

Haz clic en el objeto **insecto** en la lista de objetos. Añade un script para `fijar el tamaño`{:class="block3looks"} cuando tu `fondo cambia a`{:class="block3events"} la pantalla de `inicio`{:class="block3events"}:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [inicio v]
set size to [100] % // tamaño completo
```

--- /task ---

### Cambia su posición

--- task ---

Intenta colocarlo en la pantalla de 'inicio'.

¡Tu código hará que el fondo cambie cuando hagas clic en el insecto! Eso no es útil cuando intentas posicionarlo.

Para solucionar el problema, debes detener la ejecución del código cuando hagas clic en el insecto.

--- /task ---

--- task ---

Haz clic en la bandera verde para volver a la pantalla de 'inicio'.

Haz clic en el objeto **insecto** en la lista de objetos y arrastra los bloques lejos del bloque `al hacer clic en este objeto`{:class="block3events"}:

![Rompiendo el script.](images/breaking-script.png)

--- /task ---

--- task ---

Intenta posicionar el insecto nuevamente. Arrástralo a la pizarra, debajo del texto:

![El insecto en la pantalla de inicio](images/bug-chalkboard.png)

Añade código para asegurarte de que se posicione en la pizarra cada vez que tu `fondo cambia a`{:class="block3events"} la pantalla de `inicio`{:class="block3events"}:

![El objeto insecto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [inicio v]
set size to [100] % // tamaño completo
+ go to x: [0] y: [30] // en la pizarra
```

--- /task ---

--- task ---

Vuelve a unir los bloques para que los de código estén debajo del bloque `al hacer clic en este objeto`{:class="block3events"} nuevamente:

![El bloque 'al hacer clic en este objeto' unido a los bloques 'reproducir sonido' y 'siguiente fondo'.](images/fixed-script.png)

--- /task ---

--- task ---

**Prueba:** Haz clic en la bandera verde para probar tu proyecto. Haz clic en el insecto para pasar al siguiente fondo. Debería ser grande en la pantalla de 'inicio' y pequeño en el nivel de 'Spotlight'.

--- collapse ---
---
title: No pasa nada cuando hago clic en el insecto
---

¿Olvidaste volver a unir el código al bloque `al hacer clic en este objeto`{:class="block3events"}?

--- /collapse ---

--- /task ---