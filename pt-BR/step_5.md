## Nível 2

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Você escolherá um cenário para criar um segundo nível para o jogo e dificultar a localização do inseto. 
</div>
<div>

! [Uma cena na rua com um inseto oculto.] (Images/second-level.png){:width="300px"}

</div>
</div>

### Adicione outro plano de fundo

--- task ---

**Escolha:** Escolha um cenário para o nível 2. Escolhemos o cenário **Urbano**, mas você pode escolher o que quiser.

![O inseto e o papagaio em um cenário urbano.](images/insert-urban-backdrop.png)

**Dica:** Lembre-se de que cenários com muitas cores e detalhes irão dificultar a localização do inseto. O quão difícil você vai tornar o seu jogo?

--- /task ---

### Parar a execução do código

--- task ---

Arraste os blocos para longe do bloco `quando este ator for clicado`{:class="block3events"} para impedi-los de executarem quando você clicar no inseto:

![Quebrando o código.](images/breaking-script.png)

--- /task ---

### Redimensione o Inseto

--- task ---

Adicione o código `definir tamanho`{:class="block3looks"} do inseto no segundo nível:

![O sprite do inseto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**Teste:** Clique em seu novo script para executá-lo.

--- /task ---

### Esconda seu inseto

--- task ---

Arraste seu inseto no Palco para um bom esconderijo para este nível.

![O inseto escondido na vitrine da loja no meio do cenário.](images/hidden-urban-backdrop.png)

--- /task ---

Posicione o inseto no esconderijo.

--- task ---

Adicione um bloco `vá para x: y:`{:class="block3motion"}:

![O sprite do inseto.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

### Teste seu código

--- task ---

Junte os blocos ao bloco `quando este ator for clicado`{:class="block3events"} para que, quando o inseto for clicado, o cenário mude para o `próximo cenário`{:class="block3looks"}:

![Os blocos são unidos novamente.](images/fixed-script.png)

--- /task ---

--- task ---

**Teste:** Clique na bandeira verde e teste o seu projeto.

--- /task ---

Seu inseto agora pode estar na frente do papagaio.

--- task ---

Adicione um script para assegurar que o inseto fique sempre na posição `por trás`{:class="block3looks"}:

![O sprite do inseto.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

Agora, o inseto sempre vai ficar por atrás, mesmo que você precise alterar sua posição.

--- /task ---
