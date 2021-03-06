---
title: Transition
localeTitle: Переход
---
## Свойство Transition

Свойство `transition` позволяет вам изменять значения свойств плавно (от одного значения к другому) в течение заданной продолжительности. 

```css 
  transition: all 300ms;
```
### Несколько значений свойств
 
Мы можете задавать несколько значений свойств для свойства `transition`. 

```css 
  transition: width 300ms, height 2s;
```
### Кривая изменения скорости перехода
 
 Вы можете задавать кривую скорости изменения свойства. 
 
```css 
  transition: height 2s linear;
```
или с помощью отдельного свойства `transition-timing-function`:

```css 
  transition-timing-function: linear;
```

### Различные значения функции времени `transition-timing-function`

- `ease` - указывает эффект перехода с медленным запуском, затем быстро, затем заканчивается медленно (это значение по умолчанию)
- `linear` - определяет эффект перехода с одинаковой скоростью от начала до конца
- `ease-in` - указывает на эффект перехода с медленным запуском
- `ease-out` - указывает эффект перехода с медленным завершением
- `ease-in-out` - определяет эффект перехода с медленным запуском и завершением
- `cubic-bezier(n,n,n,n)` - позволяет вам определять свои собственные значения в функции кубического безье-преобразования

#### Дополнительная информация:

*   MDN Документация: [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)
*   Easings ссылка: [Easings](http://easings.net/en)
