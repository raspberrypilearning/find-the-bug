--- question ---
---
legend: Umbuzo 2 kwemi 3
---

Usebenzise iluphu `naphakade`{:class="block3control"} ukuze wenze isprite **Isikhwenene** sibhabhe ngendlela edikayo.

Sizamile ukongeza esinye i-sprite sokuphazamiseka, kodwa sishukuma kanye xa sicofa iflegi eluhlaza siyeke emvakoko. Sinokuyilungisa njani?

![I-Rocket sprite.](images/rocket-sprite.png)

```blocks3
when flag clicked
set rotation style [jikelele v] 
move [6] steps 
forever 
if on edge, bounce 
next costume 
change [umbala v] effect by [25] 
wait [0.5] seconds 
end
```

--- choices ---

- ( ) Guqula inani kwibhloko `hamba`{:class="block3motion"}

  --- feedback ---

Ukuba utshintsha inani kwibholoki `hamba`, uzakube utshintsha umgama ohanjwa sisprite xa iflegi eluhlaza icofiwe, kodwa lento ayizokweza irocket iqhubeke ngokuhamba.

  --- /feedback ---

- ( ) Susa ibhloko `ukuba usekugqibeleni, gxuma`{:class="block3motion"}

  --- feedback ---

Ibhloko `ukuba usekugqibeleni, gxuma`{:class="block3motion"}  yenza i-sprite sitsibe xa sifika kumda weQonga. Ukuba uyisusile, i-rocket iya kuxinga kumda weqonga

  --- /feedback ---

- ( ) Yongeza enye ibhloko ka `naphakade`{:class="block3control"}

--- feedback ---

Umbhalo uvumeleke ibholoki enye ka `naphakade`{:class="block3control"}  Uqaphele ukuba awukwazi ukongeza ibhloko ngaphantsi kwe bhloko `naphakade`{:class="block3control"}?

--- /feedback ---

- (x) Tsala bhloko `hamba`{:class="block3motion"} ngaphakathi kwe luphu `naphakade`{:class="block3control"}

  --- feedback ---

  Ewe! I-sprite ihamba kanye kuphela. Ukuba usa ibhloko `hambisa`{:class="block3motion"}  ngaphakathi kwe luphu `naphakade`{:class="block3control"}, i-sprite siyakuhlala sihamba ude uyeke iprojekthi yakho.

  --- /feedback ---

--- /choices ---

--- /question ---
