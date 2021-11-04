## شاشة النهاية

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ستنشئ شاشة "نهاية" لإظهار عدد الثواني التي استغرقها اللاعب للعثور على الحشرات. 
</div>
<div>

![The bug with the amount of time in a speech bubble.](images/end-screen.png){:width="300px"}

</div>
</div>

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
في بعض الأحيان، لا يكفي مجرد الفوز في لعبة. يحب اللاعبون معرفة ما فعلوه ضد لاعبين آخرين أو ضد أنفسهم. هل يمكنك التفكير في لعبة تظهر لك مدى جودة أدائك؟</p>

--- task ---

أضف خلفية **السبورة** من القسم **الداخلي**.

![خلفية السبورة في مكتبة الخلفية.](images/chalkboard.png)

**نصيحة:** في Scratch، يمكنك إضافة نفس الخلفية أكثر من مرة.

--- /task ---

--- task ---

انقر فوق علامة تبويب **الخلفيات** لفتح محرر الرسام.

![خلفية السبورة في محرر الرسام.](images/chalkboard2-paint.png)

--- /task ---

--- task ---

قم بتغيير اسم الخلفية إلى `نهاية`:

![تم تغيير اسم الخلفية في محرر الرسام.](images/end-screen-name.png)

**نصيحة:** يمكنك إعادة تسمية الخلفية إلى **نهاية** لتسهيل فهم البرنامج الخاص بك.

--- /task ---

--- task ---

انقر على كائن **الحشرة** وأضف تعليمات برمجية لوضع الحشرة على شاشة "النهاية":

![كائن الحشرة.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
```

--- /task ---

كم من الوقت يستغرق البحث عن الحشرات والنقر عليها؟ يحتوي Scratch على `مؤقت`{:class="block3sensing"} يمكنك استخدامه لحساب الوقت.

--- task ---

وحدة `المؤقت`{:class="block3sensing"} تكون موجودة في قائمة وحدات`الاستشعار`. أضف برنامجاً لجعل الحشرة`تقول`{:class="block3looks"}` 
المؤقت`{:class="block3sensing"} على شاشة "النهاية":

![كائن الحشرة.](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
+say (timer) // seconds taken
```

![إدراج وحدة "مؤقت" في وحدة "قل".](images/inserting-blocks.gif)

--- /task ---

--- task ---

**اختبار:** انقر فوق العلم الأخضر لاختبار مشروعك. كم من الوقت يستغرق العثور عن الحشرات؟

--- /task ---

للرجوع إلى شاشة "البداية" ، انقر فوق الحشرة الموجودة في شاشة "النهاية".

--- task ---

أضف تعليمات برمجية لجعل الحشرة تتوقف عن قول `مؤقت`{:class="block3sensing"} عندما تذهب إلى شاشة "البداية":

![كائن الحشرة.](images/bug-sprite.png)

```blocks3
when backdrop switches to [start v]
set size to [100] % // full-sized
go to x: [0] y: [30] // on the board
+say [] // say nothing
```

--- /task ---

إذا لعبت اللعبة مرة ثانية، فإنّ `المؤقت` سيستمر بالعدّ.

--- task ---

أضف تعليمات برمجية إلى `إعادة تعيين المؤقت`{:class="block3sensing"} عندما `تتغير الخلفية إلى`{:class="block3events"} المستوى الأول:

![كائن الحشرة.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Spotlight v] // first level
set size to [20] % // tiny
go to x: [13] y: [132] // on the disco ball
+reset timer // start the timer
```

--- /task ---

--- task ---

**اختبار:** انقر على العلم الأخضر والعب اللعبة. يجب إعادة ضبط المؤقت عند النقر فوق الحشرة في شاشة "البدء" للانتقال إلى المستوى الأول. عند النقر على حشرة على الشاشة "نهاية"، يجب العودة إلى شاشة "ابدأ" ونرى أن الحشرة لا تقول ل `الموقت`{: فئة = "block3sensing"}.

--- /task ---

--- save ---