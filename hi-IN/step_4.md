## तोते के माध्यम से ध्यान भटकाना

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
खिलाड़ियों के लिए बग को ढूंढना और उस पर क्लिक करने को कठिन बनाने के लिए, आप उन्हें भटकाने के लिए एक तोता जोड़ देंगे। 
</div>
<div>

![Stage पर एक रंगीन तोता।](images/parrot-distraction.png){:width="300px"}

</div>
</div>

### Add the Parrot sprite

--- task ---

**Parrot** स्प्राइट जोड़ें।

!['Choose a Sprite' आइकन](images/sprite-button.png)

--- /task ---

### Animate the Parrot sprite

[बस पकड़े](https://projects.raspberrypi.org/en/projects/catch-the-bus){:target="_blank"} प्रोजेक्ट में, आपने `repeat`{:class="block3control"} लूप का उपयोग किया था।

आप यहां एक अलग लूप का उपयोग करेंगे। एक `forever`{:class="block3control"} लूप इसके अंदर रखे कोड ब्लॉक को बार-बार चलाता रहेगा। यह एक परेशान करने वाले तोते के लिए एकदम सही लूप है जो इधर-उधर उड़ना और रास्ते में आना बंद नहीं करेगा।

--- task ---

Add code to make the parrot flap around in a distracting way. Look at the comments on the code blocks for some different numbers to try:

![Parrot स्प्राइट।](images/parrot-sprite.png)


```blocks3
when flag clicked
set rotation style [left-right v] // do not go upside down
point in direction [35] // number from -180 to 180
forever // keep being annoying
move [10] steps // the number controls the speed
if on edge, bounce // stay on the Stage
next costume // flap
change [color v] effect by [5] // try 11 or 50
wait [0.25] seconds // try 0.1 or 0.5
end
```

--- /task ---

--- task ---

**परीक्षण:** हरी झंडी पर क्लिक करें और अपने प्रोजेक्ट का परीक्षण करें। क्या आपको याद है कि आपने बग कहाँ छिपाया था?

Scratch में, चल रहा कोड पीले रंग की आउटलाइन के साथ चमकता है:

![](images/running-code.png)

**टिप:** यदि आपके द्वारा कोडिंग करते समय तोता बहुत अधिक परेशान करता है, तो आप कोड को चलने से रोकने के लिए Stage के ऊपर लाल स्टॉप बटन पर क्लिक कर सकते हैं।

--- /task ---

