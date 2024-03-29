## Parot i dynnu sylw

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Er mwyn ei gwneud hi'n anoddach i chwaraewyr ddod o hyd i'r chwilen a chlicio arni, byddi di'n ychwanegu parot annifyr i dynnu eu sylw. 
</div>
<div>

![Parot lliwgar ar y Llwyfan.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

--- task ---

Ychwanega'r corlun **Parrot**.

![Yr eicon 'Dewiswch Gorlun'.](images/sprite-button.png)

--- /task ---

Yn y prosiect [Dal y bws](https://projects.raspberrypi.org/cy-GB/projects/catch-the-bus){:target="_blank"}, fe wnes di ddefnyddio dolen `ailadrodd`{:class="block3control"}.

Byddi di'n defnyddio dolen wahanol yma. Mae dolen `am byth`{:class="block3control"} yn rhedeg y blociau cod tu mewn iddi dro ar ôl tro. Dyma'r ddolen berffaith ar gyfer parot annifyr sy'n hedfan o gwmpas a mynd yn y ffordd drosodd a throsodd.

--- task ---

Ychwanega god i wneud i'r parot ffflapioio o gwmpas mewn ffordd sy'n tynnu sylw:

![Y Corlun Parrot.](images/parrot-sprite.png)


```blocks3
when flag clicked
set rotation style [left-right v] // peidio mynd wyneb i waered
point in direction [35] // rhif rhwng -180 a 180
forever // dal ati i fod yn annifyr
move [10] steps // mae'r rhif yn rheoli'r cyflymder
if on edge, bounce // aros ar y Llwyfan
next costume // fflapio
change [color v] effect by [5] // rho gynnig ar 11 neu 50
wait [0.25] seconds // rho gynnig ar 0.1 neu 0.5
end
```

--- /task ---

--- task ---

**Prawf:** Clicia ar y faner werdd a phrofi dy brosiect eto. Allet ti gofio lle wnes di guddio'r chwilen?

Yn Scratch, mae cod sy'n rhedeg yn tywynnu gydag amlinelliad melyn:

![](images/running-code.png)

**Awgrym:** Os ydy'r parot yn mynd yn rhy annifyr wrth godio, gallwch glicio ar y botwm stop coch uwchben y Llwyfan i atal y cod rhag rhedeg.

--- /task ---

--- save ---
