--- question ---
---
legend: तीन में से तीसरा प्रश्न
---

आपने इस स्क्रिप्ट को **bug** स्प्राइट में जोड़ा है:

![बग स्प्राइट।](images/bug-sprite.png)

```blocks3
when backdrop switches to [end v]
set size to [100] % 
go to x: [0] y: [30] 
+ say (timer) 
```

जब बैकड्रॉप **end** पर स्विच करता है तो `say`{:class="block3looks"} `timer`{:class="block3sensing"} ब्लॉक Stage को कैसा दिखाता है?

--- choices ---

- ( ) ![एक तोता कह रहा है टाइमर मान "4.52"।](images/quiz_parrot_number.png)

  --- feedback ---

स्क्रिप्ट को फिर से देखें, और सोचें कि कौन सा स्प्राइट गेम का मुख्य पात्र है (तोता सिर्फ ध्यान भटकाने के लिए है)।

  --- /feedback ---

- ( ) ![एक तोता "timer"शब्द कह रहा है।](images/quiz_parrot_timer.png)

  --- feedback ---

`Sensing`{:class="block3sensing"} ब्लॉक मेन्यू से `timer`{:class="block3sensing"} ब्लॉक आता है। स्प्राइट "टाइमर" शब्द नहीं कहता है। यह भी सोचें कि कौन सा स्प्राइट इस कोड का उपयोग करता है।

  --- /feedback ---

- (x) ![एक बग कह रहा है टाइमर मान "4.52"](images/quiz_bug_number.png)

  --- feedback ---

हाँ! `timer`{:class="block3sensing"} खंड प्रोजेक्ट शुरू होने के बाद या टाइमर रीसेट होने के बाद के समय की रिपोर्ट करता है। `Say`{:class="block3looks"} ब्लॉक बग के बगल में एक स्पीच बबल बनाता है।

  --- /feedback ---

- ( ) ![एक बग "timer" शब्द कह रहा है](images/quiz_bug_timer.png)

  --- feedback ---

`Sensing`{:class="block3sensing"} ब्लॉक मेन्यू से `timer`{:class="block3sensing"} खंड आता है। स्प्राइट "टाइमर" शब्द नहीं कहता है।

  --- /feedback ---

--- /choices ---

--- /question ---





