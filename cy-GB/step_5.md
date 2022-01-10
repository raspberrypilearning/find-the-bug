## Ail lefel

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Byddi di'n dewis cefndir i wneud ail lefel ar gyfer dy gêm, ac yn ei gwneud hi'n anodd dod o hyd i'r chwilen. 
</div>
<div>

![Golygfa stryd gyda chwilen guddiedig.](images/second-level.png){:width="300px"}

</div>
</div>

--- task ---

**Dewis:** Dewisa gefnlen ar gyfer dy ail lefel. Rydyn ni wedi dewis y gefnlen **Urban**, ond gallet ti ddewis yr un rwyt ti'n ei hoffi fwyaf.

![](images/insert-urban-backdrop.png)

**Awgrym:** Cofia bydd cefndiroedd gyda llawer o liwiau a manylion yn ei gwneud hi'n anoddach dod o hyd i'r chwilen. Pa mor anodd wyt ti am wneud dy gêm?

--- /task ---

Er mwyn gallu llusgo dy chwilen i leoliad newydd, bydd angen i ti rwystro'r sgript `pan gaiff y corlun hwn ei glicio`{:class="block3events"} rhag rhedeg.

--- task ---

Llusga'r blociau i ffwrdd o'r bloc `pan gaiff y corlun hwn ei glicio`{:class="block3events"} i'w rhwystro rhag rhedeg pan fyddi di'n clicio ar y chwilen:

![](images/breaking-script.png)

--- /task ---

Mae angen i dy chwilen fod yn anodd dod o hyd iddi pan fydd y gefnlen yn newid. Galli di newid maint y chwilen i'w gwneud hi'n anoddach dod o hyd iddi.

--- task ---

Ychwanega god i `osod maint`{:class="block3looks"} y chwilen ar gyfer yr ail lefel:

![Y corlun chwilen.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**Prawf:** Clicia ar dy sgript newydd i'w rhedeg.

--- /task ---

--- task ---

Llusga dy chwilen ar i'r Llwyfan i guddfan dda ar gyfer y lefel hon.

![Y chwilen wedi'i chuddio yn ffenestr y siop yng nghanol y gefnlen.](images/hidden-urban-backdrop.png)

--- /task ---

Rho dy chwilen yn ei chuddfan.

--- task ---

Ychwanega floc `mynd i x: y:`{:class="block3motion"} at dy god:

![Y corlun chwilen.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

--- task ---

Cysyllta'r blociau yn ôl i'r bloc `pan gaiff y corlun hwn ei glicio`{:class="block3events"} fel bod y gefnlen yn newid i'r `gefnlen nesaf`{:class="block3looks"} pan gaiff y chwilen ei chlicio:

![](images/fixed-script.png)

--- /task ---

--- task ---

**Prawf:** Clicia ar y faner werdd i brofi dy brosiect.

--- /task ---

Efallai fod dy chwilen nawr o flaen y parot.

--- task ---

Ychwanega sgript i wneud yn siŵr fod dy chwilen bob amser yn y `cefn`{:class="block3looks"}:

![Y corlun chwilen.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Nawr, bydd dy chwilen bob amser yn aros yn y cefn, hyd yn oed os bydd angen i ti newid ei safle.

--- /task ---

--- save ---
