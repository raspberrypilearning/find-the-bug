## Phucula umdlalo wakho

Ukuba unexesha, unokongeza amanqanaba amaninzi kunye nezinye iziphazamiso kumdlalo wakho. Uthanda ungasitshintsha i-sprite efihliweyo kwaye utshintshe nokubhaliweyo ebhodini.

--- task ---

Dlala umdlalo wakho ujonge ukuba ungazifumana ngokukhawuleza kangakanani iigrogro.

Ingaba ukhona omnye umntu onokuzama umdlalo wakho? Bangazibhaqa ngokukhawuleza kangakanani iigrogro? Abazukwazi apho uzifihle khona, kusenokubathatha ixesha elide!

Ingaba ikhona into ofuna ukuyitshintsha?

Unga:
- Yenza isikhwenene sidike ngakumbi
- Yenza iigrogro zibe zincinci ngakumbi
- Tshintsha `isiphuma sombala`{:class="block3looks"} ukufihla igrogro kwinqanaba ngalinye
- Tshintsha ifonti okanye umbala wokubhaliweyo

--- /task ---

### Yongeza amanye amanqanaba

--- task ---

Nazi iibhloko ozakuzidinga ukufihla igrogro kwinqanaba elitsha:

```blocks3
when backdrop switches to [inqanaba elitsha v]

set size to [20] %

go to x: [0] y: [0] // tsala ukuze ubeke igrogro kwindawo

set [umbala v] effect to [50]
```

Kwinqanaba ngalinye, kuya kufuneka:
- Yongeza umfanekiso wangemva
- Cofa kuluhlu lweqonga, emva koko kwithebhu **umfanekiso wangasemva**, emva koko tsala umfanekiso wangasemva omtsha uwubeke phambi komfanekiso wangasemva u-**isiphelo**
- Faka ibhloko `xa umfanekiso wasemva utshintshela`{:class="block3events"} ukuze uthsintshe umva kwaye ufake ikhowudi kwindawo yayo kufihleke igrogro

**Ingcebiso:** Ukutsalala igrogro yakho kwindawo entsha yokufihla, uzakufuna 'ukwaphula' ikhowudi ukuze umfanekiso ongasemva ungatshintshi xa ucofa kwigrogri ukuyimisa kwindawo yokuyifihla kwinqanaba elitsha.

--- /task ---

### Yongeza ezinye iziphazamiso

--- task ---

Unokongeza ezinye izikhwenene okanye ukhethe esienye isprite ukuba isebenze njenge siphazamisi.

Nantsi ikhowudi oyisebenzise kwisikhwenene:

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

[Ingcebiso:](https://scratch.mit.edu/projects/1236322817/) Ungatsala i **Parrot** ikhowudi ye-sprite kwenye i-sprite ukuyenza ikhawuleze ukwenza enye i-sprite yokuphazamiseka.

![Tsala ikhowudi ukusuka kwindawo yekhowudi ukuyise kwesinye isprite kuluhlu lwezisprite.](images/drag-parrot-code.gif)

--- /task ---

--- collapse ---
---
title: Iprojekthi egqityiweyo
---

Ungajonga [egqityiweyo iprojekthi apha](https://scratch.mit.edu/projects/1236322817/){:target="_blank"}.

--- /collapse ---