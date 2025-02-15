# Method-string

## Доступ к символам
```
let str = `Hello`;

// получаем первый символ
alert( str[0] ); // H
alert( str.at(0) ); // H

// получаем последний символ
alert( str[str.length - 1] ); // o
alert( str.at(-1) ); // o
```

## Изменение регистра
```
alert( 'Interface'.toUpperCase() ); // INTERFACE
alert( 'Interface'.toLowerCase() ); // interface
```

## Поиск подстроки
```
let str = 'Widget with id';

alert( str.indexOf('Widget') ); // 0, потому что подстрока 'Widget' найдена в начале
alert( str.indexOf('widget') ); // -1, совпадений нет, поиск чувствителен к регистру

alert( str.indexOf("id") ); // 1, подстрока "id" найдена на позиции 1 (..idget with id)
```

## includes
```
alert( "Widget with id".includes("Widget") ); // true

alert( "Hello".includes("Bye") ); // false
```

## Получение подстроки
##### В JavaScript есть 3 метода для получения подстроки: substring, substr и slice.

str.slice(start [, end])
Возвращает часть строки от start до (не включая) end.
```
let str = "stringify";
// 'strin', символы от 0 до 5 (не включая 5)
alert( str.slice(0, 5) );
// 's', от 0 до 1, не включая 1, т. е. только один символ на позиции 0
alert( str.slice(0, 1) );
```

## Кавычки
#### В JavaScript есть разные типы кавычек.
Строку можно создать с помощью одинарных, двойных либо обратных кавычек:

```
let single = 'single-quoted';
let double = "double-quoted";

let backticks = `backticks`;
```

## Split
#### Метод split() возвращает новый массив. Если разделитель separator найден, он удаляется из строки, а подстроки возвращаются в массиве. Если разделитель опущен, массив будет содержать только один элемент, состоящий из всей строки. Если разделитель является пустой строкой, строка str будет преобразована в массив символов.

###### Пример: удаление пробелов из строки
```
var names = "Гарри Трамп ;Фрэд Барни; Хелен Ригби ; Билл Абель ;Крис Ханд ";

console.log(names);

var re = /\s*;\s*/;
var nameList = names.split(re);

console.log(nameList);
```

### возврат ограниченного числа подстрок
```

```
