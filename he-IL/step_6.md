## מסך סיום

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
צרו מסך 'סיום' כדי להראות את מספר השניות שלקח לשחקן למצוא את הבאגים. 
</div>
<div>

![הבאג עם כמות הזמן בבועת דיבור.](images/end-screen.png){:width="300px"}

</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
לפעמים, רק לנצח משחק זה לא מספיק. שחקנים אוהבים לדעת איך הם הצליחו מול שחקנים אחרים או מול עצמם. האם אתה יכול לחשוב על משחק שמראה לך כמה טוב עשית?</p>

### הוסף רקע נוסף

--- task ---

הוסף את רקע **לוח הגיר** מהקטגוריה **בתוך הבית**.

![רקע לוח הגיר בספריית הרקעים.](images/chalkboard.png)

**טיפ:** בסקראץ׳, ניתן להוסיף את אותו רקע יותר מפעם אחת.

--- /task ---

### עריכת הרקע

--- task ---

לחצו על הכרטיסייה **רקעים** כדי לפתוח את עורך הציור.

![רקע לוח הגיר בעורך הציור.](images/chalkboard2-paint.png)

--- /task ---

--- task ---

שנה את שם הרקע ל- `סוף`:

![שם הרקע השתנה בעורך הציור.](images/end-screen-name.png)

**טיפ:** עליך לשנות את שם הרקע ל- **סוף-** כדי להקל על הבנת הקוד.

--- /task ---

### מקם את הבאג

--- task ---

לחצו על הספרייט **באג** והוסיפו קוד למיקום הבאג במסך ה'סוף':

![ספרייט הבאג.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
```

--- /task ---

### הוסף טיימר

כמה זמן לוקח לך למצוא את הבאגים וללחוץ עליהם? לסקראץ׳ יש `טיימר`{:class="block3sensing"} שתוכלו להשתמש בו כדי לגלות.

--- task ---

הבלוק `טיימר`{:class="block3sensing"} מגיע מתפריט הבלוקים `חושים`{:class="block3sensing"}. הוסף קוד כדי ליצור את הבאג `אמור`{:class="block3looks"} את ה `טיימר`{:class="block3sensing"} במסך 'הסיום':

![ספרייט הבאג.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
+say (timer) // seconds taken
```

![הוספת בלוק 'טיימר' לתוך בלוק 'אמור'.](images/inserting-blocks.gif)

--- /task ---

--- task ---

**בדיקה:** לחץ על הדגל הירוק כדי לבחון את כישורי המציאה שלך. כמה זמן לוקח לך למצוא את הבאג?

--- /task ---

כדי לחזור למסך ה"התחלה", לחצו על הבאג במסך ה"סיום".

--- task ---

הוסף קוד כדי לגרום לבאג להפסיק לומר את ה`טיימר`{:class="block3sensing"} כשאתה ניגש למסך 'התחלה':

![ספרייט הבאג.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
+say [] // say nothing
```

--- /task ---

### עצור את הטיימר

אם תשחקו את המשחק פעם שנייה, ה`טיימר`{:class="block3sensing"} ימשיך לספור.

--- task ---

הוסף קוד ל- `לאפס את הטיימר`{:class="block3sensing"} כאשר הרקע `עובר ל-`{:class="block3events"} בשלב הראשון:

![ספרייט הבאג.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v] // first level
set size to [20] % // tiny
go to x: [13] y: [132] // on the disco ball
+reset timer // start the timer
```

--- /task ---

--- task ---

**בדיקה:** לחצו על הדגל הירוק ושחקו את המשחק. הטיימר אמור להתאפס כשתלחצו על הבאג במסך 'התחל' כדי לעבור לשלב הראשון. כאשר תלחצו על הבאג במסך 'הסיום', עליכם לחזור למסך 'התחלה' ולראות שהבאג אינו מציין את ה`טיימר`{:class="block3sensing"}.

--- /task ---

