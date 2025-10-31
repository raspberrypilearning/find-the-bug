--- question ---
---
מקרא: שאלה 2 מתוך 3
---

השתמשת בלולאה `אינסוף`{:class="block3control"} כדי לגרום לספרייט **תוכי** לעוף בצורה מעצבנת.

ניסינו להוסיף עוד ספרייט של הסחת דעת, אבל הוא זז רק פעם אחת כשאנחנו לוחצים על הדגל הירוק ואז נעצר. איך נוכל לתקן את זה?

![ספרייט  הרקטה.](images/rocket-sprite.png)

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

- () שנה את המספר בבלוק `תנועה`{:class="block3motion"}

  --- feedback ---

אם תשנו את המספר בבלוק `תנועה`{:class="block3motion"}, תשנו את המרחק שבו הספרייט נע בעת לחיצה על הדגל הירוק, אך שינוי זה לא יגרום לרקטה להמשיך לנוע.

  --- /feedback ---

- () הסר את הבלוק `אם הוא על הקצה, קפוץ`{:class="block3motion"}

  --- feedback ---

הבלוק `אם על הקצה, קפוץ`{:class="block3motion"} גורם לספרייט לקפוץ מקצה הבמה. אם תסיר אותו, הרקטה תיתקע בקצה הבמה.

  --- /feedback ---

- () הוסף עוד `אינסוף`{:class="block3control"} בלוק

--- feedback ---

סקריפט יכול להכיל רק בלוק אחד `אינסוף`{:class="block3control"}. האם שמת לב שאי אפשר להוסיף בלוק מתחת לבלוק `אינסוף`{:class="block3control"}?

--- /feedback ---

- (x) גרור את הבלוק `תנועה`{:class="block3motion"} בתוך הלולאה `אינסוף`{:class="block3control"}

  --- feedback ---

  כֵּן! הספרייט זז רק פעם אחת. אם תזיז את הבלוק `תנועה`{:class="block3motion"} בתוך הלולאה `אינסוף`{:class="block3control"}, הספרייט ימשיך לנוע עד שתעצור את הפרויקט.

  --- /feedback ---

--- /choices ---

--- /question ---
