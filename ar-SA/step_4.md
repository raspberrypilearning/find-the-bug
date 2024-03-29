## الببغاء المزعج

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
لتجعل من الصعب على اللاعبين العثور على الحشرة والنقر عليها، ستضيف ببغاءًا مزعجًا لإشغالهم. 
</div>
<div>

![A colourful parrot on the Stage.](images/parrot-distraction.png){:width="300px"}

</div>
</div>

### أضف كائن الببغاء

--- task ---

أضف كائن **الببغاء**.

![أيقونة "اختر كائن".](images/sprite-button.png)

--- /task ---

### حرك كائن الببغاء

في مشروع [اللحاق بالحافلة](https://projects.raspberrypi.org/ar-SA/projects/catch-the-bus){:target="_blank"}، كنت تستخدم حلقة `تكرار`{:class="block3control"}.

ستستخدم حلقة مختلفة هنا. تقوم حلقة `دائماً`{:class="block3control"} بتشغيل وحدات التعليمات البرمجية بداخلها مرارًا وتكرارًا. إنها الحلقة المثالية لببغاء مزعج لن يتوقف عن الطيران ويعترض الطريق.

--- task ---

أضف التعليمات البرمجية لجعل الببغاء يرفرف بطريقة تشتت الانتباه:

![كائن الببغاء.](images/parrot-sprite.png)


```blocks3
when flag clicked
set rotation style [left-right v] // لا تقلب رأسا على عقب
point in direction [35] // مجال العدد من -180 إلى 180
forever // استمر في الإزعاج
move [10] steps // الرَّقَم يتحكم في السرعة
if on edge, bounce // تغيير اللغة
next costume // رفرف
change [color v] effect by [5] // جرب 11 أو 50
wait [0.25] seconds // جرب 0.1 أو 0.5
end
```

--- /task ---

--- task ---

**اختبار:** انقر فوق العلم الأخضر واختبر مشروعك مرة أخرى. هل يمكنك أن تتذكر أين أخفيت الحشرة؟

في Scratch، تتوهج التعليمات البرمجية الجاري تشغيلها بمخطط أصفر:

![](images/running-code.png)

**نصيحة:** إذا أصبح الببغاء مزعجًا للغاية أثناء قيامك بكتابة التعليمات البرمجية، فيمكنك النقر فوق زر التوقف الأحمر أعلى المنصة لإيقاف تشغيل البرنامج.

--- /task ---

