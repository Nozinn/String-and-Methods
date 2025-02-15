# String-and-Methods
## Строки (String) в JavaScript
#### В JavaScript строка (string) — это последовательность символов, заключённая в кавычки:
~~~
js

let str1 = "Привет";  // Двойные кавычки
let str2 = 'Мир';     // Одинарные кавычки
let str3 = `!`;       // Косые кавычки (шаблонные строки)
~~~
### Косые кавычки позволяют вставлять переменные и выражения через ${}:
~~~
js

let name = "Нозина";
let message = `Привет, ${name}!`;
console.log(message); // Привет, Нозина!
~~~
## Методы строк в JavaScript
#### Методы строк позволяют изменять, искать и манипулировать текстом.

## 1. charAt(index), at(index)
#### Получает символ строки по указанному индексу.
~~~
js

let str = "JavaScript";
console.log(str.charAt(4)); // "S"
console.log(str.at(-1));    // "t" (отрицательный индекс работает только в `at()`)
~~~
## 2. toString()
#### Преобразует объект (например, число) в строку.
~~~
js

let num = 123;
console.log(num.toString());  // "123"
console.log((true).toString());  // "true"
~~~
## 3. concat()
#### Объединяет строки.
~~~
js

let str1 = "Hello";
let str2 = "World";
console.log(str1.concat(" ", str2, "!")); // "Hello World!"
~~~
## 4. trim()
#### Удаляет пробелы в начале и конце строки.
~~~
js

let text = "   JavaScript   ";
console.log(text.trim()); // "JavaScript"
~~~
## 5. includes(substring)
#### Проверяет, есть ли подстрока в строке.
~~~
js

let phrase = "I love JavaScript";
console.log(phrase.includes("love")); // true
console.log(phrase.includes("Python")); // false
~~~
## 6. indexOf(substring), lastIndexOf(substring)
#### Находит индекс первого/последнего вхождения подстроки.
~~~
js

let text = "Hello, JavaScript!";
console.log(text.indexOf("JavaScript"));  // 7
console.log(text.lastIndexOf("o"));  // 4
~~~
## 7. replace(old, new), replaceAll(old, new)
#### Заменяет часть строки.
~~~
js

let str = "I love Python";
console.log(str.replace("Python", "JavaScript"));  // "I love JavaScript"

let text = "apple, apple, apple";
console.log(text.replaceAll("apple", "banana"));  // "banana, banana, banana"
~~~
## 8. substring(start, end), slice(start, end)
#### Извлекает подстроку.
~~~
js

let text = "JavaScript";
console.log(text.substring(4, 10)); // "Script"
console.log(text.slice(-6));  // "Script" (slice поддерживает отрицательные индексы)
~~~
## 9. split(delimiter)
#### Разделяет строку на массив по разделителю.
~~~
js

let data = "html,css,js";
console.log(data.split(","));  // ["html", "css", "js"]
~~~
## 10. toLowerCase(), toUpperCase()
#### Изменяет регистр.
~~~
js

let word = "JavaScript";
console.log(word.toLowerCase());  // "javascript"
console.log(word.toUpperCase());  // "JAVASCRIPT"
~~~
