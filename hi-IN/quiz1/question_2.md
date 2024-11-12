--- question ---
---
legend: तीन में से दूसरा प्रश्न
---

आपने **Parrot** स्प्राइट को चारों ओर परेशान करने के तरीके से उड़ने के लिए `forever`{:class="block3control"} लूप का उपयोग किया।

हमने एक और ध्यान भटकाने वाले स्प्राइट जोड़ने की कोशिश की है, लेकिन यह सिर्फ एक बार हिलता है जब हम हरे झंडे पर क्लिक करते हैं और फिर रुक जाता है। हम इसे कैसे ठीक कर सकते हैं?

![Rocket स्प्राइट।](images/rocket-sprite.png)

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

- ( ) `move`{:class="block3motion"} ब्लॉक में संख्या बदलें

  --- feedback ---

अगर आप `move`{:class="block3motion"} खंड में नंबर बदलते हैं, तो हरे झंडे को क्लिक करने पर आप यह बदल देंगे कि स्प्राइट कितनी दूर तक जाता है, लेकिन यह बदलाव रॉकेट को गतिमान नहीं बनाएगा। .

  --- /feedback ---

- ( ) `यदि किनारे पर है, बाउंस`{:class="block3motion"} ब्लॉक को हटा दें

  --- feedback ---

`if on edge, bounce`{:class="block3motion"} ब्लॉक स्प्राइट को Stage के किनारे से उछाल देता है। अगर आपने इसे हटा दिया, तो रॉकेट Stage के किनारे पर फंस जाएगा।

  --- /feedback ---

- ( ) एक और `forever`{:class="block3control"} ब्लॉक जोड़ें।

--- feedback ---

एक स्क्रिप्ट में केवल एक ही `forever`{:class="block3control"} खंड हो सकता है। क्या आपने देखा है कि आप `forever`{:class="block3control"} ब्लॉक के नीचे एक और ब्लॉक नहीं जोड़ सकते हैं?

--- /feedback ---

- (x) `मूव`{:class="block3motion"} ब्लॉक को `फॉरएवर`{:class="block3control"} लूप के अंदर लाए

  --- feedback ---

  हाँ! स्प्राइट केवल एक बार चलता है। यदि आप `move`{:class="block3motion"} ब्लॉक को `forever`{:class="block3control"} लूप के अंदर ले जाते हैं, तो स्प्राइट तब तक चलता रहेगा जब तक आप अपना प्रोजेक्ट बंद नहीं कर देते।

  --- /feedback ---

--- /choices ---

--- /question ---
