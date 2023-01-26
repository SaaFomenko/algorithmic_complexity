# algorithmic_complexity
Response at algorithmic complexity calculations

Condition you see this [link](https://github.com/netology-code/algocpp-homeworks/tree/main/1/01)

# Задача 1. Оценка алгосложности программы
Дан код на языке `C++`. Ваша задача понять и описать, что он делает, определить его асимптотику, то есть время и дополнительную память, и привести аргументы, почему она именно такая.

```cpp
int calc(int* arr, int size)
{
  int ans = 0;
  for (int i = 1; i < size; i++)
  {
    ans += arr[i] - arr[i-1];
  }
  return ans;
}
```

## Ответ:
Функция calc() принемает массив из целых чисел и возвращает сумму разностей 
последующего и предыдущего элементов массива, сложность алгоритма равна:
1. По скорости O(n).
2. По памяти O(1).
