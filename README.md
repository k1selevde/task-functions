# Functions

Установите зависимости:

```
npm install
```

В файле `src/Functions.js` выполните следующие задания:

1. У массивов есть метод `arr.filter(callback)`, который позволяет отбирать элементы из массива. `callback` принимает на вход три параметра:

- `element` &ndash; текущий элемент
- `index` &ndash; индекс текущего элемента
- `array` &ndash; исходный массив

Результатом `callback` должен быть `boolean`:
- `true` &ndash; элемент подходит под условие
- `false` &ndash; элемент не подходит под условие

Напишите следующие фильтры:

1. `higherThan(num)` &ndash; отбирает все числа больше `num`
```javascript
console.log([1, 2, 3, 4, 5].filter(higherThan(3)));
// [4, 5]
```
2. `hasSubstring(substr)` &ndash; отбирает из массива все строки, включающие в себя `substr`. Регистр важен, т.е. строка `ABC` не включает в себя подстроку `bc`.
```javascript
console.log(['ABC', 'abc', 'bca', 'qwe'].filter(hasSubstring('bc')));
// ['abc', 'bca']
```
3. Напишите функцию `multiply(num)`, которая работает вот так:

```javascript
console.log(multiply(5)(10));
// 50
```

Проверить себя можно запустив команду `npm run test`.

После выполнения задания создайте pull request с решением.
