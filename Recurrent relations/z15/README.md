# Задача 15. Полигон

*Имя входного файла: input.txt*

*Имя выходного файла: output.txt*

*Ограничение по времени: от 1 с до 2 с*

*Ограничение по памяти: нет*


Существует игра для одного игрока, которая начинается с задания Полигона с n вершинами. Пример графического представления Полигона показан на рис. 1, где n = 4. Для каждой вершины Полигона задаётся значение — целое число, а для каждого ребра — метка операции + (сложение) либо × (умножение). Ребра Полигона пронумерованы от 1 до n.

![image](https://user-images.githubusercontent.com/43014199/116208951-1532c780-a74a-11eb-8109-c1e8728439b5.png)

Рис. 1. Графическое представление Полигона

Первым ходом в игре удаляется одно из рёбер. Каждый последующий ход состоит из следующих шагов:

выбирается ребро e и две вершины v1 и v2, которые соединены ребром e;
ребро e стягивается, то есть вершины v1 и v2 удаляются и заменяются новой вершиной v со значением, равным результату выполнения операции, определённой меткой ребра e, над значениями вершин v1 и v2. В рёбрах, отличных от e и инцидентных вершинам v1 и v2, эти две вершины заменяются на вершину v.
Игра заканчивается, когда больше нет ни одного ребра. Результат игры — это число, равное значению оставшейся вершины.
Пример игры
Рассмотрим Полигон на рис. 1. Игрок начал игру с удаления ребра 3 (см. рис. 2).

![image](https://user-images.githubusercontent.com/43014199/116209202-56c37280-a74a-11eb-81cf-dfbd60d8f7a8.png)

Рис. 2. Удаление ребра 3

После этого, игрок выбирает ребро 1 (см. рис. 3), затем ребро 4 (см. рис. 4),

![image](https://user-images.githubusercontent.com/43014199/116209318-75c20480-a74a-11eb-8ef9-3669ef61097c.png)

Рис. 3. Результат выбора ребра 1

![image](https://user-images.githubusercontent.com/43014199/116209349-7fe40300-a74a-11eb-90d5-af7847f5728e.png)

Рис. 4. Результат выбора ребра 4

и, наконец, ребро 2. Результатом игры будет число 0 (см. рис. 5).

![image](https://user-images.githubusercontent.com/43014199/116209395-8a9e9800-a74a-11eb-8236-297702cd3fc0.png)

Рис. 5. Результат выбора ребра 2.

Напишите программу, которая по заданному Полигону, вычисляет максимальное значение оставшейся вершины и выводит список всех тех рёбер, удаление которых на первом ходу игры позволяет получить это значение.

**Формат входных данных**

В первой строке записано число n (3 ≤ n ≤ 500). Вторая строка содержит метки рёбер с номерами 1, …, n, между которыми записаны через пробел значения вершин (первое из них соответствует вершине, инцидентной рёбрам 1 и 2, следующее — инцидентной рёбрам 2 и 3, и так далее, последнее — инцидентной рёбрам n и 1). Метка ребра — это буква t, соответствующая операции +, или буква x, соответствующая операции ×.
Гарантируется, что при любой последовательности ходов значения вершин находятся в пределах от −9 223 372 036 854 775 808 до 9 223 372 036 854 775 807.

**Формат выходных данных**

В первой строке выведите максимальное значение оставшейся вершины, которое может быть достигнуто для заданного Полигона. Во второй строке — список всех тех рёбер, удаление которых на первом ходу, позволяет получить это значение. Номера рёбер должны быть записаны в возрастающем порядке и отделяться друг от друга одним пробелом.
