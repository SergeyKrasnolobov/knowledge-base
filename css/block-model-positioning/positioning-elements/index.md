---
metaTitle: Овладейте свойством Position в CSS
metaDescription: Откройте для себя ключевые концепции свойства position в CSS и узнайте, как использовать его для управления макетом и расстоянием между элементами на вашем веб-сайте. | База знаний PurpleSchool
author: Алексей Овсянников
title: Свойство Position. Особенности его применения.
preview: Использование свойств позиционирования элементов широко применяется при разработке современных макетов и предоставляет различные возможности для расположения элементов в потоке документа.
---

Использование свойств позиционирования элементов широко применяется при разработке современных макетов и предоставляет различные возможности для расположения элементов в потоке документа. В этой заметки мы рассмотрим CSS свойства position, top, left, right и bottom, а также их значения.

## **Cвойство position**

Свойство position в CSS используется для указания метода позиционирования, используемого для элемента. Это позволяет размещать элементы по отношению к окну браузера или родительскому элементу вместо того, чтобы элементы следовали обычному потоку документа.

### **Синтаксис**

```css
position: static;
position: initial;
position: relative;
position: inherit;
position: absolute;
position: fixed;
position: sticky;
```

### **Значения**

- **static**(значение по умолчанию): элементы будут спозиционированы согласно правилам нормального потока.
- **relative**: положение элемента вычисляется в соответствии с нормальным потоком. Затем элемент смещается относительно своего нормального положения, при этом не влияя на положение последующих блоков. Это смещение может привести к перекрытию блоков и появлению боковой полосы прокрутки в случае переполнения. Элемент с **position**: _relative_ всегда сохраняет свои размеры и размеры вложенных в него элементов.
- **absolute**: позволяет позиционировать элемент относительно предка с **position**: _relative_. Если ни у одного родительского элемента не установлен **position**: _relative_, элемент будет с позиционирован относительно окна браузера. Положение элемента задается с помощью свойств right, left, top и bottom
- **sticky**: элемент закрепляется в определенной позиции на экране при прокрутке пользователем вниз. Может использоваться для создания фиксированной шапке / боковой панели сайта, которая будет оставаться видимой при прокрутке страницы вниз, обеспечивая легкий доступ к навигации сайта.
- **fixed**: позиционирует элемент относительно окна браузера и закрепляет его в области просмотра при прокрутке страницы. Элемент с фиксированным позиционирование не вернется к своему обычному положению в потоке документа, даже если пользователь прокрутит страницу до точки, где элемент был изначально расположен. Этим фиксированное положение отличается от липкого(sticky) позиционирования.
- **initial**: Устанавливает значение свойства в значение по умолчанию.
- **inherit**: Наследует значение свойства от родительского элемента.

## **Свойства top, right, bottom, left**

Свойства **top**, **right**, **bottom** и **left** используются для указания расстояния элемента от краев содержащего его блока. Эти свойства используются в сочетании со свойством **position**. По умолчанию значение каждого свойства установлено в значение **auto**.

- Свойство **right** указывает расстояние, на которое элемент смещен влево от правого края содержащего блока. Для относительного позиционирования смещение вычисляется относительно правого края самого элемента.
- Свойство **bottom** указывает расстояние, на которое элемент смещен вверх относительно нижнего края содержащего блока. Для относительного позиционирования смещение вычисляется относительно нижнего края самого элемента.
- Свойство **left** указывает расстояние, на которое элемент смещен вправо от левого края содержащего блока. Для относительного позиционирования смещение вычисляется относительно левого края самого элемента.
- Свойство **top** задает расстояние, на которое элемент смещается ниже верхнего края содержащего блока. Для относительного позиционирования смещение вычисляется относительно верхнего края самого элемента

### **Синтаксис**

```css
left: 50px;
bottom: -3ch;
right: 0.75rem;
top: 40%;
bottom: initial;
right: inherit;
```

### **Значения**

- **фиксированное значение длины**: Смещение на фиксированном расстоянии от указанного края. Отрицательные значения допускаются
- **%**: положительное значение в процентах от высоты содержащего блока. Для элементов с **position**: _sticky_ вычисление рассчитываются относительно высоты корневого элемента.
- **initial**: Устанавливает значение свойства в значение по умолчанию
- **inherit**: Наследует значение свойства от родительского элемента