# Задача 0.1. Бинарный поиск

*Имя входного файла: стандартный ввод*

*Имя выходного файла: стандартный вывод*

*Ограничение по времени: 2 с*

*Ограничение по памяти: 256 МБ*

Необходимо реализовать бинарный поиск на отсортированном в неубывающем порядке массиве чисел.
Использование готовых функций бинарного поиска из стандартных библиотек запрещается.

**Формат входных данных**

В первой строке записано число nn (0 < n \le 3 \cdot 10^50<n≤3⋅10 
5
 ) — длина массива чисел. Во второй строке записано nn чисел через пробел.
В третьей строке записано число kk (0 < k \le 3 \cdot 10^50<k≤3⋅10 
5
 ) запросов. В четвертой строке записано kk чисел-запросов, разделённых пробелом.

**Формат выходных данных**

Для каждого числа-запроса xx в отдельной строке выведите через пробел числа bb, ll и rr, где bb равно 11, если xx присутствует в массиве, и 00 в противном случае, ll — индекс первого элемента, большего либо равного xx, rr — индекс первого элемента, большего xx.
