#Задача:
Написать программу, 
которая из имеющегося массива строк формирует массив из строк, 
длина которых меньше либо равна 3 символа. 
Первоначальный массив можно ввести с клавиотуры, 
либо задать на старте выполнения алгоритма. 
При решении не рекомендуется пользоваться коллекциями, 
лучше обойтись исключительно массивами.

Примеры :

["hello","2","world",":-)"]->["2",":-)"]
["1234","1567","-2","computer science"]->["-2"]
["Russia","Denmark","Kazan"]->[]

## Общие положения:
Программа состоит из ***3 функций:***
- `FindSizeResultАrray` - функция, позволяющая задать размер массива;
- `FindТheЕlementsАrray` - функция поиска в массиве текстовой информации, длина которой меньше четырех символов.
- `PrintArray` - функция вывода массива на экран.

## Функция `FindSizeResultАrray`.


Данная функция позволяет определить размер массива в который будут записываться результаты.
Данная функция принимает заранее заполненный массив.
Для перебирания элементов оригинального массива используем цикл. Как только функция находит элемент, который менее 4 символов, то счетчик **`count`** прирастает на 1. По окончанию работы функции возвращаем ей значение **`count`** , это и будет размер выходного массива.

## Функция `FindТheЕlementsАrray`

Функция предназначения для поиска текстовых данных, имеющих длину менее 4 символов, и внесение найденных значений в новый массив.
Данная функиця принимает заранее заданный массив и пустой массив для записи

Далее функция перебирает каждый элемент заранее заданного массива и как только находит элемент в котором менее 4 символов, то этот элемент копируется в пустой массив для записи на позицию с интексом **`count`** , после записи элемента **`count`** прирастает на 1.
Таким образом, массив заполняется данными, длина которых **менее 4 символов**.

## Функция `PrintArray`.

Данная функция предназначена для вывода данных, хранящихся в массиве.

## Вывод конечного результата
Результатом выполнения программы является вывод исходного и результирующего массива в формате представленном в примере выполнения задания.