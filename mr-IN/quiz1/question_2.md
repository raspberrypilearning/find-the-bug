--- question ---
---
legend: प्रश्न 3 पैकी 2
---

तुम्ही `forever`{:class="block3control"} लूप वापरून **Parrot** स्प्राइटला त्रासदायक मार्गाने उड्डाण केले.

आम्ही आणखी एक डिस्ट्रक्शन स्प्राईट जोडण्याचा प्रयत्न केला आहे, परंतु जेव्हा आम्ही हिरव्या ध्वजावर क्लिक करतो तेव्हा ते एकदाच हलते आणि नंतर थांबते. आपण ते कसे दुरुस्त करू शकतो?

![Rocket स्प्राईट.](images/rocket-sprite.png)

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

- ( ) `move`{:class="block3motion"} ब्लॉकमधील क्रमांक बदला

  --- feedback ---

जर तुम्ही `move`{:class="block3motion"} ब्लॉकमधील संख्या बदलली, तर हिरवा झेंडा क्लिक केल्यावर स्प्राइट किती अंतरावर सरकतो ते तुम्ही बदलाल, परंतु या बदलामुळे रॉकेट पुढे सरकत नाही.

  --- /feedback ---

- ( ) `if on edge, bounce`{:class="block3motion"} ब्लॉक काढा

  --- feedback ---

`if on edge, bounce`{:class="block3motion"} ब्लॉक स्प्राइटला Stage च्या काठावरून बाऊन्स करतो. जर आपण ते काढले तर रॉकेट Stage च्या काठावर अडकेल.

  --- /feedback ---

- ( ) आणखी `forever`{:class="block3control"} ब्लॉक जोडा

--- feedback ---

स्क्रिप्टमध्ये फक्त एक `forever`{:class="block3control"} ब्लॉक असू शकतो. तुमच्या लक्षात आले का की तुम्ही `forever`{:class="block3control"} ब्लॉकच्या खाली ब्लॉक जोडू शकत नाही?

--- /feedback ---

- (x) `move`{:class="block3motion"} ब्लॉक `forever`{:class="block3control"} लूपमध्ये ड्रॅग करा

  --- feedback ---

  होय! स्प्राइट फक्त एकदाच फिरते. तुम्ही `move`{:class="block3motion"} ब्लॉकला `forever`{:class="block3control"} लूपमध्ये हलवल्यास, तुम्ही तुमचा प्रोजेक्ट थांबेपर्यंत स्प्राइट हलत राहील.

  --- /feedback ---

--- /choices ---

--- /question ---
