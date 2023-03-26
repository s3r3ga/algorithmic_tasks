# Мощность x
Мощность целого числа ```x``` определяется как количество шагов, 
необходимых для преобразования ```x``` в ```1``` с использованием следующих шагов:<br>
если ```x``` четно, то ```x = x / 2```,
если ```x``` нечетно, то ```x = 3 * x + 1```.

Например, для ```x = 3``` сила равна ```7```. Так как для преобразования ```3``` в ```1``` нужно 7 шагов
(3 --> 10 --> 5 --> 16 --> 8 --> 4 --> 2 --> 1).

На вход передаются три целых числа: lo, hi и k. 
Задача состоит в том, чтобы отсортировать по неубыванию все целые числа в интервале [lo, hi] 
по значению мощности. Если 2 или более чисел имеют одинаковое значение мощности, отсортируйте их по возрастанию.

## Примеры:
```
Input: lo = 12, hi = 15, k = 2
Output: 13
Explanation: Степень 12 равна 9 (12 --> 6 --> 3 --> 10 --> 5 --> 16 --> 8 --> 4 --> 2 --> 1)
             Степень 13 равна 9
             Степень 14 равна 17
             Степень 15 равна 17
Интервал отсортирован по значению мощности [12, 13, 14, 15]. Для k = 2 ответом является второй элемент, который равен 13.
```

```
Input: lo = 7, hi = 11, k = 4
Output: 7
Explanation: Интервал, отсортированный по мощности, равен [8, 10, 11, 7, 9].
Четвертое число в отсортированном массиве равно 7.
```

---
<a href="https://leetcode.com/problems/sort-integers-by-the-power-value/">LeetCode</a>