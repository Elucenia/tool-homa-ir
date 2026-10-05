<!-- ELUCENIA technical documentation · homa-ir · hi · no clinical/professional/rights approval -->

# HOMA-IR और HOMA-β

[शर्तें, स्रोत और अनुमतियाँ](https://elucenia.org/hi/tools/homa-ir)

## उपयोग कैसे करें

पोर्टल पर उपकरण का उपयोग करें या स्थानीय HTTP सर्वर के माध्यम से index.html खोलें। भाषा चुनें, फ़ील्ड भरें और गणना करें।

## इनपुट और इकाइयाँ

### उपवास रक्त ग्लूकोज़

`glicemia`

mg/dL · सीमा: 40–400

### उपवास इंसुलिन

`insulina`

µU/mL · सीमा: 0.5–300

## विधि का संस्करण

HOMA 1/Matthews 1985: IR ग्लूकोज़×इंसुलिन/22.5; बीटा 20 इंसुलिन/(ग्लूकोज़−3.5); HOMA 2 नहीं

## दस्तावेज़ित सूत्र

HOMA-IR = इंसुलिन (µU/mL) × ग्लूकोज़ (mmol/L) ÷ 22.5.

HOMA-β = 20 × इंसुलिन (µU/mL) ÷ \[ग्लूकोज़ (mmol/L) − 3.5\] (%).

ग्लूकोज़ mmol/L में = mg/dL ÷ 18.

## सीमाएँ और जनसमूह

HOMA उपवास की आधारभूत सांद्रताओं और ग्लूकोज़ तथा इंसुलिन के बीच होमियोस्टैटिक अंतःक्रिया पर निर्भर है। मूल लेख अनुमानों की कम सटीकता स्वीकार करता है। सरल HOMA1 सूत्र, HOMA2 मॉडल और आबादी के कटऑफ परस्पर बदलने योग्य नहीं हैं; परिणाम किसी व्यक्ति में इंसुलिन प्रतिरोध के निदान की पुष्टि नहीं करता।

## संदर्भ

- [Matthews DR et al. Homeostasis model assessment: insulin resistance and β-cell function from fasting plasma glucose and insulin concentrations in man. Diabetologia, 1985.](https://doi.org/10.1007/BF00280883)

- [Geloneze B et al. HOMA1-IR and HOMA2-IR indexes in identifying insulin resistance and metabolic syndrome: Brazilian Metabolic Syndrome Study (BRAMS). Arq Bras Endocrinol Metabol, 2009.](https://doi.org/10.1590/S0004-27302009000200020)

## तकनीकी परीक्षण दोहराएँ

दर्ज कृत्रिम मामलों को दोहराने के लिए इस रिपॉज़िटरी की मूल निर्देशिका में node test.cjs चलाएँ। मूल इनपुट, अपेक्षित परिणाम और सहनशीलता सीमाएँ सुरक्षित रखी गई हैं। तकनीकी परीक्षण नैदानिक सत्यापन नहीं हैं।

```sh
node test.cjs
```

tool.json में स्रोत, संस्करण और समीक्षा का दायरा दिया गया है। examples.json में कृत्रिम इनपुट और अपेक्षित परिणाम सुरक्षित हैं; results.json में प्राप्त परिणाम दर्ज हैं।

[रिकॉर्ड और संदर्भ](../tool.json) · [JavaScript कोड](../calculator.js) · [संदर्भ मामले](../examples.json) · [results.json](../results.json)

## समीक्षा और उपयोग की शर्तें

स्वतंत्र नैदानिक समीक्षा नहीं की गई है।

यह इंटरफ़ेस लेखकों द्वारा किया गया अनुवाद है, कोई आधिकारिक या प्रमाणित संस्करण नहीं। स्वतंत्र नैदानिक समीक्षा, पेशेवर भाषाई समीक्षा और उपकरणों के अधिकारों की अनुमति की प्रक्रिया पूरी नहीं हुई है।

सूत्र या वर्गीकरण का परिणाम। व्याख्या, कार्यवाही और उपयुक्तता पेशेवर मूल्यांकन और चुने गए स्रोत पर निर्भर है।

## लाइसेंस और श्रेय

Apache-2.0 केवल ELUCENIA के कोड पर लागू होता है। उपकरणों, प्रकाशनों, अनुवादों और डेटा के अधिकार उनके संबंधित अधिकारधारकों के पास रहते हैं। LICENSE और NOTICE सुरक्षित रखें।

ELUCENIA · Felipe Guedes · Copyright © 2026
