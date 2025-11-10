# lab2_2
# Цель
Получить практические навыки импорта и использования
функций, классов и констант из стандартной библиотеки Python для решения
прикладных задач.
# 2.2.1 Используя модуль math, вычислите площадь круга по заданному радиусу.
```
import math

def circle_area(radius):
  return math.pi * radius**2
try:
  radius_input = input()
  radius = float(radius_input)
  area = circle_area(radius)
  print(f"Площадь круга: {area:.2f}")
except ValueError:
  print("Ошибка: Введено нечисловое значение.")
```
# 2.2.2 Используя модуль random, сгенерируйте случайное целое число в заданном
диапазоне (включительно).
```
import random

def random_int_in_range(start, end):
    return random.randint(start, end)

try:
    start_input = input()
    end_input = input()
    start = int(start_input)
    end = int(end_input)
    random_num = random_int_in_range(start, end)
    print(f"Случайное число: {random_num}")
except ValueError:
    print("Ошибка: Введено нечисловое значение.")
```
# 2.2.3 Используя модуль datetime, выведите текущую дату и время в формате ГГГГ-ММДД ЧЧ:ММ:СС.
```
import datetime

def current_datetime():
    now = datetime.datetime.now()
    return now.strftime("%Y-%m-%d %H:%M:%S")

try:
    current_dt = current_datetime()
    print(f"Текущая дата и время: {current_dt}")
except Exception as e:
    print(f"Ошибка: {e}")
```
# 2.2.4 Используя модуль math, вычислите длину гипотенузы прямоугольного треугольника по двум заданным катетам.
```
import math

def hypotenuse(a, b):
    return math.sqrt(a**2 + b**2)

try:
    a_input = input()
    b_input = input()
    a = float(a_input)
    b = float(b_input)
    hyp = hypotenuse(a, b)
    print(f"Длина гипотенузы: {hyp:.2f}")
except ValueError:
    print("Ошибка: Введено нечисловое значение.")
```
# 2.2.5 Используя модуль random, сгенерируйте случайное число с плавающей точкой в диапазоне [0.0, 1.0).
```
import random

def random_float():
    return random.random()

try:
    random_num = random_float()
    print(f"Случайное число: {random_num:.4f}")
except Exception as e:
    print(f"Ошибка: {e}")
```
# 2.2.6 Используя модуль math, найдите синус угла, заданного в радианах
```
import math

def sin_radians(angle_rad):
    return math.sin(angle_rad)

try:
    angle_input = input()
    angle = float(angle_input)
    sin_val = sin_radians(angle)
    print(f"Синус угла: {sin_val:.4f}")
except ValueError:
    print("Ошибка: Введено нечисловое значение.")
```
# 2.2.7 Используя модуль random, перемешайте элементы списка.
```
import random

def shuffle_list(lst):
    random.shuffle(lst)
    return lst

try:
    list_input = input()
    original_list = list_input.split()
    shuffled_list = shuffle_list(original_list.copy())
    print(f"Перемешанный список: {shuffled_list}")
except Exception as e:
    print(f"Ошибка: {e}")
```
# 2.2.8 Используя модуль datetime, вычислите количество дней между двумя датами.
```
import datetime
def days(d1, d2):
    dif = abs(d1 - d2)
    return dif.days

try:
    d1 = input()
    d2 = input()
    d_f = "%Y-%m-%d"
    d_st = datetime.datetime.strptime(d1, d_f).date()
    d_end = datetime.datetime.strptime(d2, d_f).date()
    day = days(d_st, d_end)
    print(f"Количество дней между {d_st} и {d_end}: {day}")

except ValueError:
    print("Ошибка: Некорректный формат даты.")
```
# 2.2.9 Используя модуль math, найдите целую часть числа (отбросьте дробную часть).
```
import math

def integer_part(number):
    return math.trunc(number)

try:
    num_input = input()
    number = float(num_input)
    int_part = integer_part(number)
    print(f"Целая часть: {int_part}")
except ValueError:
    print("Ошибка: Введено нечисловое значение.")
```
# 2.2.10 Используя модуль random, выберите один случайный элемент из списка.
```
import random

def random_choice(lst):
    return random.choice(lst)

try:
    list_input = input()
    choice_list = list_input.split()
    random_element = random_choice(choice_list)
    print(f"Случайный элемент: {random_element}")
except Exception as e:
    print(f"Ошибка: {e}")
```
# Вывод
Получили практические навыки импорта и использования
функций, классов и констант из стандартной библиотеки Python для решения
прикладных задач.
