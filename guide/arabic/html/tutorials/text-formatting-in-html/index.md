---
title: Text Formatting in HTML
localeTitle: تنسيق النص في HTML
---
## تنسيق النص في HTML

يوفر لك HTML الكثير من العناصر المفيدة لتنسيق النص. يسمح لك بعمل النص الخاص بك: غامق ، مائل ، علامة وأكثر من ذلك بكثير. إن تغيير نمط النص الخاص بك ليس بدون أي سبب - الشيء الرئيسي هو مجرد جعل القارئ يلقي نظرة على بعض الملاحظات المهمة.

### جريئة وقوية

يمكنك بسهولة تغيير معنى النص الخاص بك باستخدام عنصر `<b>` HTML. يجعل الكلمات جريئة ، والتي تعمل على إفراد جزء التسلسل. فمثلا:

```
The most important part of your code is <b>the end</b>, because if you <b>don't close</b> the element, it will affect to <b>everything</b>!
``` 

يمكنك أيضًا استخدام `<strong>` أيضًا - إنها تضيف أيضًا أهمية "قوية" دلالية. لا يتعرف متصفحك على فرق بين هذين العنصرين ، ولكنه موجود.

### مائل وتأكيده

عادة ما تستخدم عند اقتباس شيء ما أو وضع ترجمة للكلمة في الكثير من المقالات. يجعلها مائلة - فقط تخيل ركلها قليلاً في الأحرف الصحيحة. فمثلا:

```
Theatre - <i>teatos</i>, <i>teates</i> and <i>teatron</i>.
``` 

يمكنك أيضًا استخدام `<em>` أيضًا - حيث تضيف أيضًا أهمية دلالية "مؤكدة". لا يتعرف متصفحك على فرق بين هذين العنصرين ، ولكنه موجود.

### صغير

يجعل النص الخاص بك أصغر من الحجم العادي للخط المستخدم. تم تغيير معنى هذا العنصر في HTML5 - وهو يمثل التعليقات الجانبية والطباعة الصغيرة.

`Normal, <small>small</small>, normal, <small>small</small>!`

### ملحوظ

يجعل العنصر `<mark>` نصك مميزًا - بكلمات مختلفة ، مما يجعل النص محددًا. يمكنك استخدامه لإخبار القراء بأنه أحد الأشياء المهمة في مقالك. فمثلا:

`HTML is full of things and <mark>it's our journey</mark> to get known them better!`

### تم الحذف

يجعل العنصر `<del>` نصك مبتوراً في المركز. من المفيد إظهار التغييرات في مستنداتك.

`WWI started in <del>1913</del> 1914 year.`

### إدراج

العلامة `<ins>` تجعل النص الخاص بك مدرجًا في المقالة. استخدام الكلمات الأخرى التي تجعل الأمر أسهل للفهم - إضافة. فإنه يظهر خط تحت النص المدرج.

`HTML isn't boring. <ins>You can make a lot of combinations of elements!</ins>`

### التي تشترك

يمنحك استخدام العنصر `<sub>` تنسيقًا مفيدًا كنص برمجي منخفض (يُظهر أنه أصغر في الأسفل). هناك رمز المثال:

`This was in 2003 year <sub>(needs a link).`

### Superscripted

إذا كنت تريد إجراء عكس النص الذي تم تسجيله ، فيمكنك بسهولة استخدام عنصر `<sup>` . يُظهر نصًا أصغر في الأعلى.

`10<sup>x+y</sup> = 1000`