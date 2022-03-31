# Лабораторная работа 3 - Массивы

## Теория
Что нам известно о массивах? Какие они бывают:

Вот жилой массив:

<img align="center" width="400" height="350" src="https://img-fotki.yandex.ru/get/199051/87086627.23/0_1ceadf_5c2aea6e_XL.jpg">

Вот дубовый массив:

<img align="center" width="350" height="350" src="https://terrazzo-sklad.ru/wa-data/public/shop/products/48/55/5548/images/7626/7626.970x0.jpg">

Но нас интересует несколько другое)

Говоря о массивах в программировании, можно представить баночку свежезаконсервированных маслят. Каждый из них расположен на определённом месте в банке и представляет собой что-то конкретное - один цельный маслёнок, и при этом они лежат в одной общей банке.

<img align="center" width="350" height="350" src="https://sun9-77.userapi.com/impf/xeAP4haqrtAiuyvyBiN1ZzacqvXct783c9l1Vg/abizoFf-Fko.jpg?size=750x750&quality=96&sign=25b41d075a3a0516a36fa9216a0a4cda&type=album">

Так же и с массивами: `Массив` - это структура данных, представленная в виде группы ячеек одного типа, объединенных под одним именем. Массивы используются для обработки большого количества однотипных данных. Имя массива является `указателем`, что такое указатели мы выясним немного позже. Отдельная ячейка данных массива называется элементом массива.  Элементами массива могут быть  данные любого типа в том числе и пользовательского (вспоминаем структуры). Массивы могут иметь как одно, так и более одного измерений. В зависимости от количества измерений массивы делятся на одномерные массивы, двумерные массивы, трёхмерные массивы и так далее до n-мерного массива. Чаще всего в программировании используются одномерные и двумерные массивы, поэтому мы рассмотрим только эти  массивы.

### Одномерный массив

Одномерный массив — массив, с одним параметром, характеризующим количество элементов одномерного массива. Фактически одномерный массив — это массив, у которого может быть только одна строка, и n-е количество столбцов. Столбцы в одномерном массиве — это элементы массива. На рисунке показана структура целочисленного (состоящего из целых чисел) одномерного массива a. Размер этого массива — 16 ячеек (номер каждой ячейки в квадратных скобках). Обратите внимание на то, что программисты люди странные и считают с нуля (это очень важно запомнить). Именно поэтому 16 ячеек - это ячейки с 0 по 15. Номер ячеёки в массиве называют индексом. `Индекс ячейки` – это целое неотрицательное число, по которому можно обращаться к каждой ячейке массива и выполнять какие-либо действия над ней.

<img align="center" width="700" height="100" src="http://cppstudio.com/wp-content/images/article/image17.1.png">

Вариантов объявления и инициализации массивов достаточно, давайте их рассмотрим:

```c++

//синтаксис  объявления одномерного массива в С++:
/*тип данных*/  /*имя одномерного массива*/[/*размерность одномерного массива*/];
//пример объявления одномерного массива, изображенного на рисунке 1:
int a[16]; // где, int — целочисленный тип данных; а —  имя одномерного массива;

//ещё один способ объявления одномерных массивов
int mas[10], mas1[16]; // в таком способе объявления все массивы будут иметь одинаковый тип данных, в нашем случае — int

// массивы могут быть инициализированы при объявлении:
int b[16] = { 5, -12, -12, 9, 10, 0, -9, -12, -1, 23, 65, 64, 11, 43, 39, -15 }; // инициализация одномерного массива

int a[]={5,-12,-12,9,10,0,-9,-12,-1,23,65,64,11,43,39,-15}; // инициализации массива без определения его размера (он определится сам)

```

[Массивы](http://cppstudio.com/post/389/) <br/>
[Массивы](https://ravesli.com/urok-74-massivy-chast-1/) <br/>
[Статические массивы](https://ravesli.com/urok-75-massivy-chast-2/) (нужен VPN)<br/>
[Циклы и массивы](https://ravesli.com/urok-76-massivy-i-tsikly/) (нужен VPN)<br/>

## Бонус

[Сортировки](https://habr.com/ru/post/414447/)

Ой, кто это у нас такой молодец и дочитал теорию третей лабы? Ух ты ж мой красавчик! Иди и порви эти задачи!

<img align="center" width="400" height="370" src="https://sun9-23.userapi.com/impf/m1NKec8oWbcFCaZVTY9pA0Df7cMTUJeYWsMBpQ/PRTPhTZAxpc.jpg?size=600x516&quality=96&sign=7653ca48c780a49d3106e3dcbbdaa129&type=album">

<hr>

### Инструкция
В директории `sources` заготовлены несколько файлов. В них есть шаблоны для заданий. Реализуйте функции в соответствии с заданием.

### Задание
1. Дан массив. Все его элементы:
    1. увеличить в 2 раза;
    2. уменьшить на число `a`;
    3. разделить на первый элемент.

2. Определить:
    1. сумму всех элементов массива;
    2. сумму квадратов всех элементов массива;
    3. сумму шести первых элементов массива;
    4. сумму элементов массива с `k1`-го по `k2`й;
    5. среднее арифметическое всех элементов массива;
    6. среднее арифметическое элементов массива с `s1`-го по `s2`-й.

3. Дан одномерный массив из 20 элементов.  Переставить первые три и последние три элемента, сохранив порядок их следования.
4. Дан массив чисел. Сначала вводится N число элементов, после этого вводится N элементов. Посчитайте, сколько в нем пар элементов, равных друг другу. Считается, что любые два элемента, равные друг другу образуют одну пару, которую необходимо посчитать.
5. Удалить из массива:
    1. первый отрицательный элемент (если отрицательные элементы в массиве есть);
    2. удалить последний четный элемент (если четные элементы в массиве есть).

6. Дано название города. Определить, четно или нет количество символов в нем.
7. Даны две фамилии. Выведите на консоль `true`, если первая длиннее.
8. Даны названия трех городов. Запишите в `the_longest` самое длинное, а самое короткое название в `the_shortest`.

9. Дано слово. Получить его часть, образованную идущими подряд буквами, начиная с `m`-й и заканчивая `n`-й.
10. Дано слово.  Добавить к нему в начале и конце столько звездочек, сколько букв в этом слове.
11. Дано предложение. Определить долю (в %) букв `'a'` в нем.
12. Дано предложение `"Can you can a can as a canner can can a can?"`. Заменить все слова `can` на слово `new_word`.
13. (типа со звёздочкой) Продолжаем мучить вас задачами про ферзей (спасибо Никите). Известно, что на доске 8×8 можно расставить 8 ферзей так, чтобы они не били друг друга. Вам дана расстановка 8 ферзей на доске, определите, есть ли среди них пара бьющих друг друга. 
