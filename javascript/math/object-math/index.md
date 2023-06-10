---
metaTitle: Объект Math – JavaScript Object Math – Объект Math в JS
metaDescription: Как работает объект Math в JS | База знаний PurpleSchool
author: Дмитрий Фандорин
title: Объект Math в JavaScript
preview: Объект Math - это встроенный модуль в JavaScript, который предоставляет множество математических функций...
---

Объект Math - это встроенный модуль в JavaScript, который предоставляет множество математических функций. С помощью объекта Math вы можете выполнять операции, такие как округление чисел, вычисление тригонометрических функций, генерация случайных чисел и многое другое.

## Форма записи

Вызов функций объекта Math осуществляется через точку после имени объекта, например:

```javascript
Math.round(2.4); // Возвращает 2
Math.sin(Math.PI / 2); // Возвращает 1
Math.random(); // Возвращает случайное число от 0 до 1
```

## Описание работы

Объект Math имеет множество методов, которые могут использоваться для выполнения различных математических операций. Вот некоторые из наиболее распространенных методов объекта Math:

- Math.abs(x): возвращает абсолютное значение числа x.

```javascript
Math.abs(-5); // Возвращает 5
```

- Math.ceil(x): округляет число x до ближайшего большего целого числа.

```javascript
Math.ceil(2.4); // Возвращает 3
```

- Math.floor(x): округляет число x до ближайшего меньшего целого числа.

```javascript
Math.floor(2.9); // Возвращает 2
```

- Math.max(x, y, ...): возвращает наибольшее число из переданных аргументов.

```javascript
Math.max(1, 2, 3); // Возвращает 3
```

- Math.min(x, y, ...): возвращает наименьшее число из переданных аргументов.

```javascript
Math.min(1, 2, 3); // Возвращает 1
```

- Math.pow(x, y): возводит число x в степень y.

```javascript
Math.pow(2, 3); // Возвращает 8
```

- Math.random(): возвращает случайное число от 0 до 1.

```javascript
Math.random(); // Возвращает случайное число от 0 до 1
```

- Math.round(x): округляет число x до ближайшего целого числа.

```javascript
Math.round(2.4); // Возвращает 2
```

- Math.sin(x): вычисляет синус угла x.

```javascript
Math.sin(Math.PI / 2); // Возвращает 1
```

- Math.sqrt(x): вычисляет квадратный корень числа x.

```javascript
Math.sqrt(25); // Возвращает 5
```

- Math.tan(x): вычисляет тангенс угла x.

```javascript
Math.tan(Math.PI / 4); // Возвращает 1
```

## Примеры

Пример 1: генерация случайного числа в заданном диапазоне

```javascript
function getRandomNumber(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

console.log(getRandomNumber(1, 10)); // Возвращает случайное число от 1 до 10
```

Пример 2: вычисление площади круга

```javascript
function getCircleArea(radius) {
  return Math.PI * Math.pow(radius, 2);
}

console.log(getCircleArea(5)); // Возвращает площадь круга с радиусом 5
```

Пример 3: округление числа до заданного количества знаков после запятой

```javascript
function roundNumber(num, decimalPlaces) {
  return Math.round(num * Math.pow(10, decimalPlaces)) / Math.pow(10, decimalPlaces);
}

console.log(roundNumber(2.3456, 2)); // Возвращает 2.35
```

## Заключение

Объект Math предоставляет множество полезных математических функций, которые можно использовать в вашем коде. При работе с числами вам может понадобиться округлять, генерировать случайные числа, вычислять тригонометрические функции и многое другое. Благодаря объекту Math вы сможете выполнять эти операции легко и быстро, используя готовые методы, предоставляемые этим объектом.