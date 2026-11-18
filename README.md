# محملين الاجهزة — QDU

منصة اختبارات تفاعلية بإعداد مقتدى الكناني، تضم 155 سؤالًا من ملف الوورد. اعتمدت المنصة ترتيب المحاضرات والأسئلة والخيارات الأصلية، ومفتاح الإجابة هو الخيار المظلّل بالأصفر في الملف.

| المحاضرة | أرقام الأسئلة في المصدر | العدد |
| --- | --- | --- |
| X-Ray Machine System & Operating Console | 1–45 | 45 |
| High-Voltage Generators, Rectification & X-Ray Circuits | 46–91 | 46 |
| X-Ray Tube Components, Design & Failure Mechanisms | 92–155 | 64 |

تظهر الأسئلة والخيارات بالإنكليزية وتُعرض ترجمتها من زر الترجمة. لكل سؤال شرح علمي باللهجة العراقية يظهر بعد الإجابة الخاطئة ومن زر «لماذا هذه الإجابة؟» وفي مراجعة النتائج. تشرح المنصة القيم التي تخص أمثلة المحاضرات أو تصاميم معيّنة من الأجهزة ضمن سياقها.

## التشغيل والفحص

الموقع ثابت ويقرأ ملفات JSON من `data/`. لتشغيله محليًا استخدم `python -m http.server` من مجلد المستودع. لفحص البيانات شغّل `node tools/validate-data.js data`، ولاختبار المحرك شغّل `node tools/test-core.js`. اختبار الواجهة متاح من مجلد `tools` بالأمر `npm run test:ui`.

## مراجع الشروح

- [دليل الفيزياء في الأشعة التشخيصية من IAEA، خصوصًا فصلي إنتاج الأشعة والتصوير الإسقاطي](https://www-pub.iaea.org/MTCD/Publications/PDF/Pub1564webNew-74666420.pdf)
- [التصوير الشعاعي من FDA](https://www.fda.gov/radiation-emitting-products/medical-x-ray-imaging/radiography)
- [التنظير التألقي من FDA](https://www.fda.gov/radiation-emitting-products/medical-x-ray-imaging/fluoroscopy)
- [دليل الوكالة الدولية للطاقة الذرية للحماية في الأشعة التشخيصية](https://nucleus.iaea.org/sites/nss-oui/Published%20Chunks/m_60b8e698-4f59-4c24-809a-dfb819ac5050/c_b5a5d3b0-697a-4b9b-8ed2-5b21e0b6bedc__9_0.Html)
- [أحمال أنبوب الأشعة ووحدات الحرارة من دليل Shimadzu](https://www.shimadzu-medical.eu/sites/shimadzu.seg.med/files/PDFs/Operation_Manual_X-ray_Tube_P324DK_M535-E263H.pdf)
- [دليل Varex لتركيب أنابيب الأشعة وتهيئتها حراريًا](https://www.vareximaging.com/wp-content/uploads/2022/07/133228-000-X-Ray-Tube-Assembly-Installation-Manual.pdf)
- [متطلبات اختبار إشعاع التسرب في المعيار الأمريكي](https://www.ecfr.gov/current/title-21/chapter-I/subchapter-J/part-1020/section-1020.30)
- [البيانات الذرية للتنغستن من NIST](https://physics.nist.gov/PhysRefData/Handbook/Tables/tungstentable1_a.htm)
