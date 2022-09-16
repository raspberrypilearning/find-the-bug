--- question ---
---
legend : Question 3 sur 3
---

Tu as ajouté ce script au sprite **bug**:

![Le sprite bug.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % 
go to x: [0] y: [30] 
+ say (timer) 
```

Comment le bloc `dire`{:class="block3looks"} `chronomètre`{:class="block3sensing"} donne-t-il l'apparence de la scène quand l'arrière-plan passe à **fin** ?

--- choices ---

- ( ) ![Un perroquet disant la valeur du chronomètre "4.52".](images/quiz_parrot_number.png)

  --- feedback ---

Revois le script et réfléchis au sprite qui est le personnage principal du jeu (le perroquet n'est qu'une distraction agaçante).

  --- /feedback ---

- ( ) ![Un perroquet prononçant le mot "chronomètre".](images/quiz_parrot_timer.png)

  --- feedback ---

Le bloc `chronomètre`{: class = "block3sensing"} vient du menu blocs `capteurs`{: class = "block3sensing"} . Le sprite ne dit pas le mot "chronomètre". Pense également à quel sprite utilise ce code.

  --- /feedback ---

- (x) ![Un bug indiquant la valeur du chronomètre "4.52".](images/quiz_bug_number.png)

  --- feedback ---

Oui. Le bloc `chronomètre`{:class="block3sensing"} indique le temps écoulé depuis le démarrage du projet ou depuis la réinitialisation du chronomètre. The `say`{:class="block3looks"} block creates a speech bubble next to bug.

  --- /feedback ---

- ( ) ![Un bug disant le mot "chronomètre".](images/quiz_bug_timer.png)

  --- feedback ---

Le bloc `chronomètre`{: class = "block3sensing"} vient du menu blocs `capteurs`{: class = "block3sensing"} . Le sprite ne dit pas le mot "chronomètre".

  --- /feedback ---

--- /choices ---

--- /question ---





