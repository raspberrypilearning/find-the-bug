--- question ---
---
legend: Cwestiwn 2 o 3
---

Wnes di ddefnyddio dolen `am byth`{:class="block3control"} i wneud i'r corlun **Parot** hedfan o gwmpas mewn ffordd annifyr.

Rydyn ni wedi ceisio ychwanegu corlun arall i dynnu sylw, ond dim ond unwaith mae'n symud pan fyddwn ni'n clicio ar y faner werdd ac wedyn mae'n stopio. Sut allwn ni ddatrys hyn?

![Y corlun Rocket.](images/rocket-sprite.png)

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

- ( ) Newidia y rhif yn y bloc `symud`{:class="block3control"}

  --- feedback ---

Os wyt ti'n newid y rhif yn y bloc `symud`{:class="block3motion"} byddi di'n newid pa mor bell mae'r corlun yn symud pan fydd y faner werdd yn cael ei chlicio, ond fydd y newid hwn ddim yn gwneud i'r roced ddal ati i symud.

  --- /feedback ---

- ( ) Tynna'r bloc `os ar yr ymyl, bowndio`{:class="block3motion"}

  --- feedback ---

Mae'r bloc `os ar yr ymyl, bowndio`{:class="block3motion"} yn gwneud i'r corlun fownsio oddi ar ymyl y Llwyfan. Pe byddi di'n ei dynnu, yna byddai'r roced yn mynd yn sownd ar ymyl y Llwyfan.

  --- /feedback ---

- ( ) Ychwanega floc `am byth`{:class="block3control"}

--- feedback ---

Dim ond un bloc `am byth`{:class="block3control"} all sgript gael. Wnes di sylwi nad oes modd ychwanegu bloc dan y bloc `am byth`{:class="block3control"}?

--- /feedback ---

- (x) Llusga'r bloc `symud`{:class="block3motion"} i mewn i'r ddolen `am byth`{:class="block3control"}

  --- feedback ---

  Grêt! Dim ond unwaith mae'r corlun yn symud. Os symudi di'r bloc `symud`{:class="block3motion"} i mewn i'r ddolen `am byth`{:class="block3control"}, bydd y corlun yn parhau i symud nes i ti stopio dy brosiect.

  --- /feedback ---

--- /choices ---

--- /question ---
