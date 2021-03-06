---
title: CSS Selectors Cheat Sheet
localeTitle: CSS المختارات الغش ورقة
---
# مختارات CSS

في CSS ، تكون المحددات هي الأنماط المستخدمة لتحديد عناصر DOM.

هنا مثال على استخدام المحددات. في التعليمة البرمجية التالية ، تكون `a` و `h1` محددات:

```css
a {
  color: black;
}

h1 {
  font-size 24px;
}
``` 

## قائمة الغش من المحددات

| محدد | يختار |  
| --- | --- | | `head` | يحدد العنصر مع علامة `head`  
| `.red` | يختار جميع العناصر مع الطبقة "الحمراء"  
| `#nav` | يحدد العناصر التي تحتوي على "nav" Id |  
| `div.row` | يحدد كل العناصر بعلامة `div` وفئة 'row' | | `[aria-hidden="true"]` | يحدد جميع العناصر ذات السمة `aria-hidden` بقيمة "true" | | `*` | اختيار حرف البدل. يحدد كل عناصر DOM. انظر أدناه لاستخدامه مع محددات أخرى |

يمكننا الجمع بين المحددات بطرق مثيرة للاهتمام. بعض الأمثلة:

| المختارون | يختار |  
| --- | --- | | `li a` DOM descendant combinator. كل `a` العلامات التي طفلا من `li` علامات |  
| `div.row *` | يقوم بتحديد كل العناصر التي تكون تابعة (أو الطفل) للعناصر ذات علامة `div` وفئة 'row' |  
| `li > a` | اختلاف combinator. حدد أحفاد مباشرة ، بدلا من كل أحفاد مثل محددات السليل |  
| `li + a` | combinator المجاور. فإنه يحدد العنصر الذي يسبقه مباشرة العنصر السابق. في هذه الحالة ، فقط أول `a` بعد كل `li` . |  
| `li, a` | يختار كل `a` العناصر وكل `li` العناصر. |  
| `li ~ a` | الأخت الأصطف. يختار `a` عنصر بعد `li` عنصر. |

من المفيد أيضًا اختيار محددات الزائفة أو الطبقات الهيكلية الزائفة لتحديد العناصر الهيكلية من DOM. فيما يلي بعض منها:

| المختارون | يختار | | --- | --- |  
| `:first-child` | استهدف العنصر الأول مباشرة داخل (أو طفل) عنصر آخر  
| `:last-child` | استهدف العنصر الأخير مباشرة داخل (أو تابع) عنصر آخر  
| `:nth-child()` | استهدف العنصر n مباشرة داخل عنصر آخر (أو تابع لـ). يعترف الأعداد الصحيحة ، `even` ، `odd` ، أو الصيغ |  
| `a:not(.name)` | يختار كل `a` العناصر التي ليست من `.name` الطبقة |  
| `::after` | يسمح بإدخال محتوى على صفحة من CSS بدلاً من HTML. في حين أن النتيجة النهائية ليست في الواقع في DOM ، فإنها تظهر على الصفحة كما لو كانت كذلك. يتم تحميل هذا المحتوى بعد عناصر HTML. |  
| `::before` | يسمح بإدخال محتوى على صفحة من CSS بدلاً من HTML. في حين أن النتيجة النهائية ليست في الواقع في DOM ، فإنها تظهر على الصفحة كما لو كانت كذلك. يتم تحميل هذا المحتوى قبل عناصر HTML. |

يمكننا استخدام فصول زائفة لتحديد حالة خاصة لعنصر DOM ولكن لا تشير إلى عنصر في حد ذاته. بعض الأمثلة:

| فئة زائفة | يختار | | --- | --- | | `:hover` | يحدد عنصر يحوم مؤشر الماوس  
| `:focus` | يحدد عنصر تلقي التركيز من لوحة المفاتيح أو برمجيًا | | `:active` | يحدد عنصر يتم النقر بواسطة مؤشر الماوس  
| `:link` | يختار كل الروابط التي لم يتم النقر بعد |  
| `:visited` | يحدد الرابط الذي تم بالفعل النقر |

## ألعاب

[CSS Diner](http://flukeout.github.io) هي لعبة الويب التي تعلم كل شيء تقريبا هناك لمعرفة الجمع بين المحددات.

## مرجع إضافي

هناك العديد من محددات CSS! تعرف عليهم في [CodeTuts](http://code.tutsplus.com/tutorials/the-30-css-selectors-you-must-memorize--net-16048) ، [CSS-tricks.com](https://css-tricks.com/almanac/selectors/) ، [w3schools.com](http://www.w3schools.com/cssref/css_selectors.asp) أو في [موزيلا شبكة مطوري](https://developer.mozilla.org/en/docs/Web/Guide/CSS/Getting_started/Selectors) .