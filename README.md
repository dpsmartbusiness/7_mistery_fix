# Решатель квадратных уравнений

Функция нахождения корней квадратного уравнения

# Как использовать

Код решения квадратных уравнений находится в файле quadratic_equation.py и содержит в себе функцию решения квадратных уравнений get_roots() (с тремя параметрами - a,b,c; каждый из которых является переменной общего вида квадратного уравнения). Переменные root1 и root2 - первый и второй корни квадратного уравнения.
 
 Присвоим значения переменным a,b,c квадратного уравнения общего вида. Затем, с помощью нашего кода найдем дискриминант (переменная discriminant в функции get_roots()). В зависимости от получившегося значения дискриминанта вычисляем корни уравнения:
 1. Дискриминант > 0; Результат: уравнение имеет 2 корня (root1, root2)
 2. Дискриминант = 0; Результат: уравнение имеет 1 корень (root1, None)
 3. Дискриминант принимает любое другое значение отличное от 1. и 2. пунктов ( Дискриминант < 0); Результат: Уравнение не имеет корней (None, None)
 
```python
from quadratic_equation import get_roots


'''Дискриминант > 0'''       
root1, root2 = get_roots(1, 2, -3)
print (root1,root2)


''' Дискриминант = 0'''
root1, root2 = get_roots(1, -2, 1)
print (root1,root2)


'''Дискриминант < 0'''
root1, root2 = get_roots(1, 2, 3)
print (root1,root2)
```

# Как запустить

Скрипт требует для своей работы установленного интерпретатора Python версии 3.5

Запуск на Linux:

```bash
python tests.py # может понадобиться вызов python3 вместо python, зависит от настроек операционной системы
```

Запуск на Windows происходит аналогично.

# Цели проекта

Код создан в учебных целях. В рамках учебного курса по веб-разработке ― [DEVMAN.org](https://devman.org)
