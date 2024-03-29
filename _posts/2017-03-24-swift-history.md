---
layout: post
title: Swift
tags: history swift
---

## Кто?
Крис Латтнер (компания Apple)

## Что?
Swift - преемник Objective-C.

Расширения файлов: .swift

## Когда?
2014г.

## Какой?
Мультипарадигмальный (протоколо-ориентированный, объектно-ориентированный, функциональный, императивный).
Строгая типизация с выводом типа (возможность компилятора самому логически вывести тип значения у выражения).

## Пример кода

```swift
// однострочный комментарий

/* многострочный
комментарий */

/* многострочные комментарии
   /* могут быть вложенными */
   поэтому можно помещать комментарии в блоки
*/

/* объявление переменной в Swift начинается со служебного слова "var", после которого должно 
идти имя переменной, тип переменной и начальное значение */
var explicitDouble: Double = 70

// если тип переменной не указано, Swift выберет его автоматически, основываясь на начальном значении
var implicitInteger = 70
var implicitDouble = 70.0
var 国 = "日本"

/* объявление константы в Swift начинается со служебного слова "let", после которого должно 
идти имя переменной, тип переменной и начальное значение */
let numberOfBananas: Int = 10

// если тип константы не указано, Swift выберет его автоматически, основываясь на начальном значении
let numberOfApples = 3
let numberOfOranges = 5

// значение переменных и констант могут быть вставлены в строки (переменные типа string) следующим образом:
let appleSummary = "I have \(numberOfApples) apples."
let fruitSummary = "I have \(numberOfApples + numberOfOranges) pieces of fruit."

// объявление массива данных
var fruits = ["mango", "kiwi", "avocado"]

// пример оператора if; функций .isEmpty, .count
if fruits.isEmpty {
    print("Фрукти відсутні у масиві даних.")
} else {
    print("В масиві даних є \(fruits.count) фруктів")
}

// пример объявления "словаря" (dictionary ) из 4 элементов, каждый из которых содержит имя и возраст
let people = ["Anna": 67, "Beto": 8, "Jack": 33, "Sam": 25]

// используя возможности языка Swift, мы напечатаем оба значения в одном цикле
for (name, age) in people {
    print("\(name) is \(age) years old.")
}

// объявление методов начинается со служебного слова "func" 
// тип результата описывается посля "->"
func sayHello(personName: String) -> String {
    let greeting = "Hello, " + personName + "!"
    return greeting
}

// Вывести "Hello, Jane!", используя метод выше
print(sayHello("Jane"))
```