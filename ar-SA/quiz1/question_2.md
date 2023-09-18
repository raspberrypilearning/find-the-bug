--- question ---
---
القائمة: السؤال 2 من 3
---

لقد استخدمت حلقة `دائماً`{:class="block3control"} لجعل كائن **الببغاء** يطير حولك بطريقة مزعجة.

حاولنا إضافة كائن إزعاج آخر، لكنه يتحرك مرة واحدة فقط عندما نضغط على العلم الأخضر ثم يتوقف. كيف يمكننا إصلاحه؟

![كائن الصاروخ.](images/rocket-sprite.png)

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

- ( ) قم بتغيير الرقم الموجود في وحدة `تحرك`{:class="block3motion"}

  --- feedback ---

إذا قمت بتغيير الرقم في وحدة `تحرك`{:class="block3motion"} فسوف تقوم بتغيير المسافة التي يتحرك بها الكائن عند النقر فوق العلم الأخضر، ولكن هذا التغيير لن يجعل الصاروخ يستمر في الحركة.

  --- /feedback ---

- ( ) قم بإزالة وحدة `إذا كان على الحافة, اقفز`{:class="block3motion"}

  --- feedback ---

وحدة `إذا كان على الحافة ، اقفز`{:class="block3motion"} تجعل الكائن يرتد عن حافة المنصة. إذا قمت بإزالته، فسوف يبقى الصاروخ على حافة المنصة.

  --- /feedback ---

- ( ) أضف وحدة `دائماً`{:class="block3control"} من جديد

--- feedback ---

أضف وحدة `دائماً`{:class="block3control"} من جديد. هل لاحظت أنّه لا يمكنك إضافة وحدة أسفل وحدة `دائماً`{:class="block3control"}؟

--- /feedback ---

- (x) اسحب وحدة `تحرك`{:class="block3motion"} إلى داخل حلقة `دائماً`

  --- feedback ---

  نعم! يتحرك الكائن مرة واحدة فقط. إذا قمت بتحريك وحدة `تحرك`{:class="block3motion"} إلى داخل حلقة `دائماً`{:class="block3control"}, سيستمر الكائن بالحركة حتى تقوم بإيقاف مشروعك.

  --- /feedback ---

--- /choices ---

--- /question ---
