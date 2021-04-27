# Задача 56. Острова

*Имя входного файла: input.txt*

*Имя выходного файла: output.txt*

*Ограничение по времени: 1 с*

*Ограничение по памяти: 256 МБ*

Одно небольшое малоизвестное государство размещается на N островах, омываемых бескрайними водами Тихого океана. На трёх островах расположены три больших города — крупные промышленные узлы государства. Правительство разрабатывает проект строительства автомобильных мостов между некоторыми парами островов, чтобы обеспечить надёжную транспортную связь между городами. Цель — сделать возможным беспрепятственный проезд на автомобиле из каждого города в любой другой.

Инженеры разработали M проектов мостов между парами островов и оценили стоимость реализации всех проектов (каждая пара островов рассматривалась не более одного раза, причём строительство кольцевых мостов из острова в него же никого не интересует). Мосты предполагают двустороннее движение транспорта по ним.

Строить все мосты дорого, да и нет необходимости: достаточно связать лишь три острова, на которых располагаются города, можно не напрямую, а через другие острова. Какой минимальный объём финансирования потребуется для этого?

**Формат входных данных**

В первой строке входного файла записаны через пробел целые числа N (3 ≤ N ≤ 100 000) и M (1 ≤ M ≤ 100 000) — соответственно количество островов и количество мостов, которые можно построить. Острова имеют номера от 0 до N − 1.
В последующих M строках описываются мосты: каждая строка содержит три числа A, B (0 ≤ A, B < N) и K (1 ≤ K ≤ 1 000 000), которые свидетельствуют, что строительство моста между островами A и B стоит K у. е.

В последней строке записано три различных числа X, Y и Z (0 ≤ X, Y, Z < N) — номера островов, между которыми следует организовать сухопутные перемещения.

**Формат выходных данных**

Выведите одно число — минимальную сумму (в у. е.), которую потребуется потратить на строительство мостов. Гарантируется, что решение существует.