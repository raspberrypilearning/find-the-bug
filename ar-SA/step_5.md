## المستوى الثاني

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
ستختار خلفية لإنشاء مستوى ثانٍ للعبتك، وتجعل من الصعب العثور على الحشرة. 
</div>
<div>

![A street scene with a hidden bug.](images/second-level.png){:width="300px"}

</div>
</div>

--- task ---

**اختر:** اختر خلفية للمستوى الثاني. لقد اخترنا **المدينة**، ولكن يمكنك اختيار الصورة التي تحبها أكثر من غيرها.

![](images/insert-urban-backdrop.png)

**نصيحة:** تذكر أن الخلفيات التي تحتوي على الكثير من الألوان والتفاصيل ستجعل من الصعب العثور على الحشرة. إلى أي مدى ستجعل لعبتك صعبة؟

--- /task ---

لتتمكن من سحب الحشرة الخاصة بك إلى موضع جديد، تحتاج إلى إيقاف تشغيل `عند النقر على الكائن` {:class="block3events"} من العمل.

--- task ---

اسحب الوحدات بعيدًا عن `عند النقر على الكائن`{: class = "block3events"} لمنعها من العمل عند النقر فوق الحشرة:

![](images/breaking-script.png)

--- /task ---

يجب أن يكون من الصعب العثور على الحشرة الخاصة بك عندما تتغير الخلفية. يمكنك تغيير حجم الحشرة لجعل العثور عليها أكثر صعوبة.

--- task ---

أضف التعليمة البرمجية `اضبط الحجم`{: class = "block3looks"} للحشرة من أجل المستوى الثاني:

![كائن الحشرة.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v] // choose your backdrop
set size to [20] % // try another size 
```

**اختبار:** انقر فوق البرنامج الجديد لتشغيله.

--- /task ---

--- task ---

اسحب الحشرة الخاصة بك على المنصة إلى مكان اختباء جيد لهذا المستوى.

![الحشرة المخبأة في نافذة المتجر في منتصف الخلفية.](images/hidden-urban-backdrop.png)

--- /task ---

ضع الحشرة في مخبأها.

--- task ---

أضف وحدة لتحديد الإحداثيات `اذهب إلى س:ع:` {:class="block3motion"} إلى برنامجك:

![كائن الحشرة.](images/bug-sprite.png)

```blocks3
when backdrop switches to [Urban v]
set size to [20] % // try another size 
+ go to x: [24] y: [13] // in the shop window
```

--- /task ---

--- task ---

انضم إلى الوحدات مرة أخرى إلى الرقم `عندالنقر على الكائن`{: class = "block3events"} بحيث عند النقر على الحشرة، تتحول الخلفية إلى الخلفية `الخلفية التالية`{:class="block3looks"}:

![](images/fixed-script.png)

--- /task ---

--- task ---

**اختبار:** انقر فوق العلم الأخضر لاختبار مشروعك.

--- /task ---

قد تكون الحشرة الآن أمام الببغاء.

--- task ---

أضف نصًا برمجيًا للتأكد من أن الحشرة دائما في `الخلف`{:class="block3looks"}:

![كائن الحشرة.](images/bug-sprite.png)

```blocks3
when flag clicked
forever
go to [back v] layer
```

الآن، ستبقى الحشرة دائمًا في الخلف، حتى إذا كنت بحاجة إلى تغيير موضعها.

--- /task ---

--- save ---