## שלב השני

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
בחרו רקע כדי ליצור שלב שני למשחק שלכם, ודאגו שהבאג יהיה קשה למציאה. 
</div>
<div>

![סצנת הרחוב עם באג נסתר.](images/second-level.png){:width="300px"}

</div>
</div>

### הוסף רקע נוסף

--- task ---

**בחר:** בחר רקע לשלב השני שלך. בחרנו את הרקע **עירוני**, אבל אתם יכולים לבחור את זה שאתם הכי אוהבים.

![הבאג והתוכי על רקע עירוני.](images/insert-urban-backdrop.png)

**טיפ:** זכרו שרקעים עם הרבה צבעים ופרטים יקשו על מציאת הבאג. כמה קשה תהפוך את המשחק שלך?

--- /task ---

### לעצור את הקוד מלרוץ

--- task ---

גררו את הבלוקים הרחק מהבלוק `כאשר הספרייט הזה לחוץ`{:class="block3events"} כדי למנוע מהם לפעול כשתלחצו על הבאג:

![שבירת הקוד.](images/breaking-script.png)

--- /task ---

### שנה את גודל הבאג

--- task ---

הוסף קוד כדי `לקבוע את הגודל`{:class="block3looks"} של הבאג עבור הרמה השנייה:

![ספרייט הבאג.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**בדיקה:** לחץ על הסקריפט החדש שלך כדי להריץ אותו.

--- /task ---

### הסתר את הבאג שלך

--- task ---

גררו את החרק שלכם על הבמה למקום מסתור טוב לשלב הזה.

![הבאג שהוסתר בחלון הראווה באמצע הרקע.](images/hidden-urban-backdrop.png)

--- /task ---

מקם את הבאג שלך במקום המחבוא שלו.

--- task ---

הוסף בלוק `לך לx: y:`{:class="block3motion"} לקוד שלך:

![ספרייט הבאג.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

### בדוק את הקוד שלך

--- task ---

חברו את הבלוקים בחזרה לבלוק `כאשר הספרייט הזה נלחץ`{:class="block3events"} כך שכאשר לוחצים על הבאג, הרקע עובר ל `רקע הבא`{:class="block3looks"}:

![הבלוקים מחוברים בחזרה יחד.](images/fixed-script.png)

--- /task ---

--- task ---

**בדיקה:** לחץ על הדגל הירוק כדי לבדוק את הפרויקט שלך.

--- /task ---

ייתכן avctd שלך נמצא עכשיו לפני התוכי.

--- task ---

הוסף סקריפט כדי לוודא שהבאג שלך תמיד נמצא ב- `מאחור`{:class="block3looks"}:

![ספרייט הבאג.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

עכשיו, הבאג שלך תמיד יישאר מאחור, גם אם תצטרך לשנות את מיקומו.

--- /task ---
