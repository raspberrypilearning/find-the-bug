## IsiKhwenene esiphazamisayo

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Ukwenza kube nzima ukubhaqa igrogro kubadlali kunye nokoyicofa, uya kufaka isikhwenene esidikayo kuze baphazamiseke. 
</div>
<div>

![Isikhwenene esimibalabala eqongeni.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

### Faka isprite IsiKhwenene

--- task ---

Faka isprite [Isikhwenene](https://projects.raspberrypi.org/xh-ZA/projects/catch-the-bus).

![Uphawu 'Khetha iSprite '.](images/sprite-button.png)

--- /task ---

### Yenza isprite Isikhwenene sibe ngupopayi

Kwiprojekthi [Leqa ibhasi](https://projects.raspberrypi.org/xh-ZA/projects/catch-the-bus){:target="_blank"}, usebenzise iluphu `phinda`{:class="block3control"}.

Uya kusebenzisa iluphu eyahlukileyo apha. Iluphu `ngonaphakade`{:class="block3control"} iqhuba iibhloko zekhowudi engaphakathi kuyo kwakhona kwaye kwakhona. Yeyona luphu ifanele isikhwenene esidikayo esingayekiyo ukubhabha sijikeleze kwaye singene endleleni.

--- task ---

Yongeza ikhowudi ukwenza isikhwenene siphakuzele sijikeleze ngendlela ephazamisayo. Jonga izimvo kwiibhloko zekhowudi ujonge amanani athile ahlukeneyo uwazame:

![iSprite Isikhwenene.](images/parrot-sprite.png)


```blocks3
when flag clicked
set rotation style [ekhohlo-ekunene v] // unga jonge phantsi-phezulu
point in direction [35] // inani ukusuka -180 ukuya 180
forever // hlala udikiwe
move [10] steps // inani lilawula isantya
if on edge, bounce // hlala eQongeni
next costume // phakuzelisa
change [umbala v] effect by [5] // zama 11 okanye 50
wait [0.25] seconds // zama 0.1 okanye 0.5
end
```

--- /task ---

--- task ---

**Uvavanyo:** Cofa kwiflegi eluhlaza ukuze uvavanye iprojekthi yakho kwakhona. Ngaba uyakhumbula ukuba uyifihle phi igrogro yakho?

KuScratch, ikhowudi esebenzayo iyakhazimla ngolwandlalo olutyheli:

![](images/running-code.png)

**Ingcebiso:** Ukuba isikhwenene sidika kakhulu ngelixa ukhowudayo, ungcofa iqhosha elibomvu ngaphezulu kweQonga lokumisa ukumisa ikhowudi engasebenzi.

--- /task ---

