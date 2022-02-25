# Секция Javascript

## Типы данных

> Какие типы данных есть в Javascript?

> Что выведет консоль в примерах ниже?
```javascript
var x = 3;
var y = "3";
// console.log(x + y);

var x = 24;
var y = "Hello";
// console.log(x + y);

var x = "Hello my";
var y = "dear friend";
// console.log(x + y);

var x = 3;
var y = "3";
// console.log(x - y);

var x = 3;
var y = "three";
// console.log(x - y, typeof(x - y));


const obj = {
  id: 3,
  name: 'John'
};
const arr = [true, true, true];
const obj1 = {};
const arr1 = [];

// console.log(
//   Boolean(obj),
//   Boolean(arr),
//   Boolean(obj1),
//   Boolean(arr1),
// );
```

> Что выведет консоль в примерах ниже?
```javascript
let variable = 1;
let variable2 = variable;

variable2 = 2;
// console.log(variable, variable2);


let obj = { name: "Alex", age: 23 };
let obj2 = obj;

obj2.name = 'Stan';
// console.log(obj, obj2); 


let arr = [1, 1, 1, 1];
let arr2 = arr;

arr2[2] = 2;
// console.log(arr, arr2);
```

[Типы данных](https://learn.javascript.ru/types)

[Преобразование типов данных](https://learn.javascript.ru/type-conversions)

[Простые и ссылочные типы](https://learn.javascript.ru/object-copy)

## Функции

> Что такое Function expression и Function declaration?

[Function declaration](https://learn.javascript.ru/function-basics)
[Function expression](https://learn.javascript.ru/function-expressions)

## Область видимости

> Какие виды областей видимости есть в JS?

> Что выведет консоль в примерах ниже?
```javascript
// console.log(a);
var a = 'a';

var test = 1;
test = 2;
var test = 3;
// console.log(test);

function hoist() {
  insideFunc = 20;
}
hoist();
// console.log(insideFunc);


function doSomething(){
  x = 33;
  console.log(x);
  var x;
}
// console.log(x);
```

> Что такое hoisting?

## Объекты
> Что такое прототип, прототипное наследование?

> Что такое контекст, примеры потери контекста?

> Для чего нужны методы call, bind, apply

## ES6

> В чем отличие объявления переменных через var, let и const

> Чем отличаются стрелочные функции от function expression и function declaration

> Что вы знаете о классах в Javascript

> Что такое rest и spread операторы?

> Как работает деструтуризация объектов, массивов

> Что такое Promise, зачем нужен этот механизм? (плюс async, await) 

> Опишите струтуру данных Map, Set (плюс WeakMap, WeakSet)

> В чем разница между именованным импортом и импортом по дефолту

[var, let, const](https://learn.javascript.ru/let-const)

[Стрелочные функции](https://learn.javascript.ru/arrow-functions-basics)

[Классы](https://learn.javascript.ru/classes)

[Rest и spread операторы](https://learn.javascript.ru/rest-parameters-spread-operator)

[Деструктуризация](https://learn.javascript.ru/destructuring-assignment)

[Promise](https://learn.javascript.ru/async)

[Типы данных (Map, Set, WeakMap, WeakSet)](https://learn.javascript.ru/data-types)

[Экспорт, импорт](https://learn.javascript.ru/import-export)

## Общее

> Что такое замыкание? Примеры использования

> Что такое рекурсия?

> Что такое event loop? В чем отличие микротасок от макротасок

> Что выведет консоль в примере ниже? 
```javascript
console.log('1');
Promise.resolve().then(() => console.log('2'));
setTimeout(() => console.log('3'), 0);
console.log('4');
```

> Что такое Ajax? 

[Замыкания](https://learn.javascript.ru/closure)

[Рекурсия](https://learn.javascript.ru/recursion)

[Event loop](https://learn.javascript.ru/event-loop)

[Ajax](https://developer.mozilla.org/en-US/docs/Web/Guide/AJAX)

## Работа с методами Array.prototype (forEach, map, reduce, filter, every, find) [must have] 

```
Задача:
    Реализовать функцию calculateSum, которая принимает от 0 до N аргументов и возвращает результат их сложения
Входные данные:
    Aргументы типа number. Допустимы положительные, отрицательные и нулевые значения
Выходные данные:
    Сумма всех аргументов типа number
Пример:
    calculateSum(1, 2, 3, 4) // Ожидаемый результат равен 10
```

```
Задача:
 Реализовать функцию removeFalsyValues, которая удаляет все ложные значения из массива
 (Ложные значения это значение которые при приведении к boolean равняются false)
 Входные значения:
 	Массив смешанных примитивных типов (boolean, string, number, null, undefined)
 Выходные значения:
 	Массив смешанных примитивных типов в котором отсутствуют ложные значения
 Пример:
 	removeFalsyValues([0, 1, '', 'test', null, 4]) // Ожидаемый результат [1, 'test', 4]
```

```
Задача:
		Реализовать функцию appendAdditionalInfo(items, itemsAdditionalData) которая добавляет дополнительную информацию для работ
	Входные данные:
		- Массив работ [{ id: number, name: string, price: number }]
		- Дополнительная информация { 123: Object, ... , 222: Object } (ключи это id работ)
	Выходные данные:
		- Массив работ с добавленной дополнительной информацией
	Пример:
	    Входные данные:
            const items = [
                {
                    id: 1,
                    name: 'Варежки',
                    price: 220,
                },
                {
                    id: 2,
                    name: 'Перчатки',
                    price: 330,
                }
            ];
            const itemsAdditionalData = {
                1 : {
                    inFavorite: true,
                },
                2 : {
                    inFavorite: true,
                    upListPromoted: true,
                    discountCost: 113,
                },
            };
        Выходные данные:
            const resultItems = [
                {
                    id: 1,
                    name: 'Варежки',
                    price: 220,
                    inFavorite: true,
                },
                {
                    id: 2,
                    name: 'Перчатки',
                    price: 330,
                    inFavorite: true,
                    upListPromoted: true,
                    discountCost: 113,
                }
            ];
            
```

```javascript
/* 
	Задача:
		Реализовать функцию groupShopsByLegalStatus которая группирует магазины по юридическому статусу
	Входные данные:
		Массив магазинов [{ name: string, type: LEGAL_STATUS }]
	Выходные данные:
		Объект со сгруппированными магазинами: { [LEGAL_STATUS.PHYSICAL_ENTITY]: array, [LEGAL_STATUS.LEGAL_ENTITY]: array }
 */

/**
 * Типы юридических статусов
 */
const LEGAL_STATUS = {
    PHYSICAL_ENTITY: 0,
    LEGAL_ENTITY: 2,
}
```

[Методы Array.prototype](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#instance_methods)

