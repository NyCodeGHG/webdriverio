---
id: autocompletion
title: 'स्वत: पूर्ण'
---

## इंटेलीजे

आईडिया और वेबस्टॉर्म में स्वत: पूर्णता बेहतर तरीके से काम करती है।

यदि आप कुछ समय से प्रोग्राम कोड लिख रहे हैं, तो शायद आपको स्वत: पूर्णता पसंद है। कई कोड संपादकों में स्वत: पूर्ण उपलब्ध है।

![स्वत: पूर्ण](/img/autocompletion/0.png)

[JSDoc](http://usejsdoc.org/) पर आधारित प्रकार की परिभाषाएँ कोड के दस्तावेजीकरण के लिए उपयोग की जाती हैं। यह मापदंडों और उनके प्रकारों के बारे में अधिक अतिरिक्त विवरण देखने में मदद करता है।

![स्वत: पूर्ण](/img/autocompletion/1.png)

उपलब्ध दस्तावेज़ देखने के लिए इंटेलीजे प्लेटफ़ॉर्म पर मानक शॉर्टकट <kbd>⇧ + ⌥ + SPACE</kbd> का उपयोग करें:

![स्वत: पूर्ण](/img/autocompletion/2.png)

## विजुअल स्टूडियो कोड (VSCode)

विज़ुअल स्टूडियो कोड में आमतौर पर टाइप सपोर्ट स्वचालित रूप से एकीकृत होता है और इसके लिए किसी कार्रवाई की आवश्यकता नहीं होती है।

![स्वत: पूर्ण](/img/autocompletion/14.png)

यदि आप वेनिला जावास्क्रिप्ट का उपयोग करते हैं और उचित प्रकार का समर्थन चाहते हैं तो आपको अपने प्रोजेक्ट रूट में `jsconfig.json` बनाना होगा और उपयोग किए गए wdio पैकेजों को देखें, उदाहरण के लिए:

```json title="jsconfig.json"
{
    "compilerOptions": {
        "types": [
            "node",
            "@wdio/globals/types",
            "@wdio/mocha-framework"
        ]
    }
}
```