## Tela final

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Você criará uma tela 'final' para mostrar o número de segundos que o jogador levou para encontrar os insetos. 
</div>
<div>

![O inseto com a quantidade de segundo em balão.](images/end-screen.png){:width="300px"}

</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
Às vezes, apenas vencer um jogo não é suficiente. Os jogadores gostam de saber como se saíram contra outros jogadores ou contra eles próprios. Você consegue pensar em um jogo que mostra quão bem você se saiu?</p>

--- task ---

Adicione o cenário **Chalkboard (Quadro-negro)** da categoria de **Interior**.

![O cenário quadro-negro na biblioteca de cenários.](images/chalkboard.png)

**Dica:** No Scratch, você pode adicionar o mesmo cenário mais de uma vez.

--- /task ---

--- task ---

Clique na aba **Cenários** para abrir o editor Paint.

![O cenário quadro-negro no editor Paint.](images/chalkboard2-paint.png)

--- /task ---

--- task ---

Altere o nome do cenário para `fim`:

![O nome do cenário mudou no editor Paint.](images/end-screen-name.png)

**Dica:** Você nomeia o cenário com o nome de **fim** para facilitar a compreensão do seu código.

--- /task ---

--- task ---

Clique no **inseto** e adicione código para posicionar o inseto na tela 'fim':

![O ator inseto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [fim v]
set size to [100] % // tamanho máximo
go to x: [0] y: [30] // no quadro
```

--- /task ---

Quanto tempo você leva para localizar e clicar nos insetos? Scratch tem um `temporizador`{:class="block3sensing"} que você pode usar para descobrir.

--- task ---

O bloco `temporizador`{:class="block3motion"} está na categoria `Detecção` no menu. Adicione código para fazer o inseto `falar`{:class="block3looks"} o `temporizador`{:class="block3sensing"} na tela 'final':

![O ator inseto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [fim v]
set size to [100] % // tamanho máximo
go to x: [0] y: [30] // no quadro
+say (timer) // segundos gastos
```

![Inserindo um bloco 'temporizador' em um bloco 'falar'.](images/inserting-blocks.gif)

--- /task ---

--- task ---

**Teste:** Clique na bandeira verde e teste suas habilidades de localização. Quanto tempo você leva achar o inseto?

--- /task ---

Para voltar à tela 'início', clique no inseto na tela 'fim'.

--- task ---

Adicione código para fazer o inseto parar de falar `temporizador`{:class="block3sensing"} quando você tiver que ir para a tela 'início':

![O ator inseto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [início v]
set size to [100] % // tamanho máximo
go to x: [0] y: [30] // no quadro
+say [] // não diga nada
```

--- /task ---

Se você jogar o jogo uma segunda vez, o `temporizador`{:class="block3sensing"} continuará contando.

--- task ---

Adicione código para `zerar o cronômetro`{:class="block3sensing"} quando o `cenário mudar para`{:class="block3events"} o primeiro nível:

![O ator inseto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v] // primeiro nível
set size to [20] % // minúsculo
go to x: [13] y: [132] // na bola de discoteca
+reset timer // temporizador
```

--- /task ---

--- task ---

**Teste:** Clique na bandeira verde e comece jogar. O cronômetro deve zerar quando você clicar no inseto na tela 'início' para passar para o primeiro nível. Quando você clicar no inseto na tela 'fim', você deve retornar à tela 'inicial' e verificar que o inseto não está dizendo `temporizador`{:class="block3sensing"}.

--- /task ---

--- save ---
