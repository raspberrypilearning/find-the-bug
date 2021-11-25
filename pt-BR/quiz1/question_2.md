--- question ---
---
legend: Pergunta 2 de 3
---

Você usou um loop `sempre`{:class="block3control"} para fazer a **Papagaio** voar de forma irritante sem rumo.

Tentamos adicionar outro ator para distração, mas ele só se move uma vez quando se clica na bandeira verde e depois para. Como podemos conserta-lo?

![O ator Foguete.](images/rocket-sprite.png)

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

- ( ) Altere o número no bloco `mover`{:class="block3control"}

  --- feedback ---

Se você mudar o número no bloco `mover`{:class="block3motion"}, você vai alterar o quão longe o ator pode ir quando a bandeira verde for clicada, mas essa alteração não vai fazer com que o foguete continue se movendo.

  --- /feedback ---

- ( ) Remova o bloco `se tocar na borda, volte`{:class="block3motion"}

  --- feedback ---

O bloco `se tocar na borda, volte`{:class="block3motion"} faz o ator rebater na borda do Palco. Se você o remover, o foguete ficará parado na borda do Palco.

  --- /feedback ---

- ( ) Adicione um outro loop `sempre`{:class="block3motion"}

--- feedback ---

Um script pode ter somente um loop `sempre`{:class="block3motion"}. Você percebeu que não é possível adicionar um bloco abaixo do loop `sempre`{:class="block3control"}?

--- /feedback ---

- (x) Arraste o bloco `mover`{:class="block3looks"} para dentro do loop `sempre`{:class="block3control"}

  --- feedback ---

  Sim! O ator só se move uma vez. Se você colocar o bloco `mover`{:class="block3motion"} dentro do loop `sempre`{:class="block3control"}, o ator irá se mover até que você interrompa seu projeto.

  --- /feedback ---

--- /choices ---

--- /question ---
