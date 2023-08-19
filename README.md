# معدل ضيق شوارع الاحياء في الرياض 📊

## المقدمة والأهداف 🎯
### ايش اكثر مشكلة تعرفها لما احد يقولك كيف السكن بالرياض؟

![image](https://github.com/RynHb/Bootcamp-Project-3-Interactive-Data-Visualization/assets/62115163/9c32de1a-c3fc-4127-b431-a88df898d260)





في مشروعنا هذا نهدف الى تحليل بيانات عقارات فلل الرياض ونرى اين توجد مشاكل ضيق الشوارع وماهي اسبابها، نستخدم في مشروعنا مجموعة البيانات المتاحة على [Kaggle](https://www.kaggle.com/datasets/reemamuhammed/riyadh-villas-aqar) وتحتوي على الكثير من المعلومات عن عقارات الفلل الرياض.


# أعضاء الفريق 👥
1. ريان العوفي: عمل على اختيار الفكرة وتجهيز وتنظيف البيانات وملف التعليمات
2. الوليد الخضيري: عمل على الرسوم البيانية
3. طيف الشمراني: عملت على تنظيف البيانات ولوحة المعلومات

## نظرة عامة على مجموعة البيانات ومصدرها 📈
في هذا المشروع، سنستخدم مجموعة البيانات التي تم الحصول عليها من موقع Kaggle. تحتوي هذه المجموعة على معلومات حول الفلل في منطقة الرياض. يمكن العثور على مجموعة البيانات من هنا [Riyadh Villas Aqar](https://www.kaggle.com/datasets/reemamuhammed/riyadh-villas-aqar)


## تجهيز البيانات وتنظيفها 🧹
بعد رفع مجموعة البيانات باستخدام مكتبة Pandas، تم اتخاذ عدة خطوات لتجهيز وتنظيف البيانات قبل استخدامها في التحليل والتصور:

- تم استعراض شكل مجموعة البيانات باستخدام df.shape لفهم عدد الصفوف والأعمدة.
- تم عرض معلومات عن الأعمدة والنوع وعدد القيم غير الفارغة باستخدام df.info().
- تم التأكد من عدم وجود صفوف مكررة باستخدام df.duplicated().sum().
- تم تغيير اسم العمود 'Unnamed: 0' إلى 'ID' باستخدام df.rename(columns={'Unnamed: 0': 'ID'}, inplace=True).
- تم حذف الصفوف التي تحتوي على قيم مفقودة في الأعمدة 'lounges'، 'streetWidth'، 'price'، 'square price'.
- تم حذف الصفوف التي تحتوي على موقع 'وسط الرياض'.
- تم تحويل قيم العمود 'bathrooms' إلى أنماط صحيحة بواسطة تعويض العلامة '+' وتحويلها إلى نوع البيانات الصحيحة.
- تم تطبيق نفس الإجراءات لتنظيف وتحويل أنماط البيانات في الأعمدة 'apartments' و 'lounges'.
- تم تغيير أنواع البيانات في العديد من الأعمدة إلى أنماط البيانات الصحيحة، مثل 'stairs'، 'propertyAge'، 'driverRoom'، وما إلى ذلك.
- تم تنظيف البيانات في العمود 'neighbourhood' باستخدام function لتجهيز أسماء الأحياء وإزالة القيم غير المرغوب فيها.

## لوحة المعلومات 📋
ا ب ب س اب س ب ل ا س ا 

## الرسوم البيانية والأفكار 📊
يتضمن في الرسوم البيانية والافكار تصور العلاقات واكتشاف جذور المشكلة بين البيانات المختلفة مع بيانات عرض الشارع

### 1. (اسم الشكل) 📈
   
![image](https://github.com/RynHb/Bootcamp-Project-3-Interactive-Data-Visualization/assets/62115163/726ff9bd-6853-4ab7-b230-c1ca072d6b37)

### بعض الأفكار من ( اسم الشكل ):
-
-
-

---


### 2. (اسم الشكل) 📈
   
(الصورة)

### بعض الأفكار من ( اسم الشكل ):
-
-
-

---



للحصول على معلومات برمجية مفصلة واكثر، يرجى الرجوع إلى ملف الكود Python الموجود في هذا المستودع.
