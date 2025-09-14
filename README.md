# Цели:
1. Изучить основные управляющие конструкции языка Python: условный
оператор и циклы.
2. Научиться использовать управляющие структуры для решения задач
различной сложности.
3. Закрепить навыки обработки данных с использованием коллекций и
итераторов.
4. Развить умение комбинировать условия и циклы для оптимизации
алгоритмов.

# 1. Рассчитать значение f при заданном значении вещественного числа x
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

x = float(input())
if x >= 0:
    f = x**0.5 + x **2
else:
    f = 1 / x

print(round(f,2))
```
Пример вывода:

<img width="827" height="423" alt="image" src="https://github.com/user-attachments/assets/bd0f5812-aa4d-49e6-a132-0d99d99b218a" />

# 2. Определите максимальное и минимальное значения из двух различных целых чисел
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com


a1 = int(input("Введите первое число: "))
a2 = int(input("Введите первое число: "))

# Переменная 'a_min' должна содержать минимум, 'a_max' - максимум
if a1 > a2:
  a_min = a2
  a_max = a1
else:
  a_min = a1
  a_max = a2
print(f"Минимальное значение: {a_min}, максимальное значение: {a_max}")
```
Пример вывода:

<img width="1187" height="707" alt="image" src="https://github.com/user-attachments/assets/062c13c3-aa6c-4c3a-91fa-46078b4edc27" />

# 3. Вася пытается высунуть голову в форточку размерами a и b см. Приняв условно,что его голова - круглая диаметром d см, определите, сможет ли Вася сделать это. Для прохождения головы в форточку необходим зазор в 1 см. с каждой стороны. Все величины - целые числа
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

a = int(input("Ширина форточки: "))
b = int(input("Высота форточки: "))
d = int(input("Диаметр головы: "))

# Введенные числа должны быть положительными, если так - осуществляем
# расчет, иначе выводим "Проверьте ввод"

if a < 0 or b < 0 or d < 0:
  print ("Проверьте ввод")

if d + 2 <= a and d + 2 <= b:
  print ("Да")
else:
  print ("Нет")
```
Пример вывода:

<img width="1752" height="825" alt="image" src="https://github.com/user-attachments/assets/f3434742-0828-4c48-a0ef-13143c68812a" />

# 4. Известны год и номер месяца сегодняшнего дня, а также год и номер месяца рождения человека (нумерация месяцев с 1: январь - 1 и т.д.). Определите возраст человека (число полных лет).
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

year_today = int(input("Введите текущий год: "))
month_today = int(input("Введите текущий месяц: "))

year = int(input("Введите год рождения: "))
month = int(input("Введите месяц рождения: "))

# Результат необходимо записать в переменную 'age'

if month_today >= month:
  age = year_today - year
else:
  age = year_today - year - 1
print("Число полных лет: ", age)
```
Пример вывода:

<img width="1634" height="788" alt="image" src="https://github.com/user-attachments/assets/a1ca68d6-c51d-4a0e-ab38-6ddc2f039639" />

# 5. Дана точка с целыми ненулевыми координатами (x;y). Определить номер четверти координатной плоскости, которой она принадлежит
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

x = int(input("Введите координату x: "))
y = int(input("Введите координату y: "))

if x > 0 and y > 0:
  print("1-я четверть")
elif x < 0 and y > 0:
  print("2-я четверть")
elif x < 0 and y < 0:
  print("3-я четверть")
else:
  print("4-я четверть")
```
Пример вывода:

<img width="885" height="666" alt="image" src="https://github.com/user-attachments/assets/d6ded5dc-09dc-4994-96ab-93dede6f54d3" />

# 6. Даны вещественные числа a, b, c (a≠0). Решите уравнение ax^2+bx+c=0. При выводе значений оставьте 1 знак после запятой
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

a = float(input("Введите a: "))
b = float(input("Введите b: "))
c = float(input("Введите c: "))
d = b**2 - (4 * a * c)
if d < 0:
  print("Нет корней")
elif d == 0:
  x = - b / 2 * a
  print(round(x, 1))
else:
  x_1 = (- b - d**0.5) /(2 * a)
  x_2 = (- b + d**0.5) /(2 * a)

  print(round(x_1, 1))
  print(round(x_2, 1))
```
Пример вывода:

<img width="881" height="765" alt="image" src="https://github.com/user-attachments/assets/de9dd1ba-62ae-4c30-a76b-ff76148ab1d9" />

# 7.Дана непустая последовательность целых чисел, оканчивающаяся нулем. Найти сумму и количество введенных чисел.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

nums_sum = 0  # сумма
nums_count = 0  # количество

x = int(input("Введите последовательность: "))
while x != 0:
  nums_sum += x % 10
  nums_count += 1
  x = x // 10

print(f"Сумма: {nums_sum}, количество: {nums_count}")
```
Пример вывода:

<img width="1004" height="492" alt="image" src="https://github.com/user-attachments/assets/aadb1fb8-f693-421a-9d0d-1f8050bdd16a" />

# 8. Дано число n. Из чисел 0,5,10,15,20,25,... напечатать те, которые не превышают n.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите число: "))
for i in range(0, n+1, 5):
  print(i)
```
Пример вывода:

<img width="956" height="434" alt="image" src="https://github.com/user-attachments/assets/156af5a3-4148-4866-abcf-ee402f743680" />

# 9. Дано вещественное число a. Найдите наименьшее натуральное n, для которого верно выражение.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

a = float(input())
n = 0
while a >= 0:
  n += 1
  a = a - (1/n)
print (n)
```
Пример вывода:

<img width="681" height="400" alt="image" src="https://github.com/user-attachments/assets/50f766f2-fc69-4a83-9f95-8511bcd1295e" />

# 10. Дано натуральное число. Определите сумму и количество его цифр
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите значение: "))
n_sum = 0
n_count = 0
while n > 0 :
  n_sum += n % 10
  n_count += 1
  n = n//10
print(f"Сумма цифр: {n_sum}, количество цифр: {n_count}" )
```
Пример вывода:

<img width="1073" height="592" alt="image" src="https://github.com/user-attachments/assets/ebfbd16a-69b5-4926-a3bf-944bd22d308a" />

# 11. Вывести в строку 10 первых натуральных чисел, оканчивающихся на цифру k, кратных числу s и находящихся в интервале, левая граница которого равна start
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

start = int(input("Введите стартовое значение: "))
k = int(input("Введите конечное значение: "))
s = int(input("Введите значение делителя: "))
n_count = 0
c = 1
res = []
while n_count < 10:
    if c % s == 0 and c % 10 == k and c > start:
      res.append(str(c))
      n_count += 1
    c += 1
print(" ".join(res))
```
Пример вывода:

<img width="1019" height="660" alt="image" src="https://github.com/user-attachments/assets/97abcf4d-f89c-4b9f-a8d3-c8d94f77ad09" />

# 12. Даны целые числа a и b (a может быть больше b). Напечатайте: 1.числа от минимального до максимального в строчку (разделяя пробелом); 2.числа от максимального до минимального «столбиком».
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com


a = int(input("Введите значение a: "))
b = int(input("Введите значение b: "))
mx = max(a,b)
mn = min(a,b)
s = []
o =[]
for i in range(mn, mx+1, 1):
  s.append(str(i))
print(" ".join(s))

for i in range(mx, mn-1, -1):
  print(i)
```
Пример вывода:

<img width="938" height="774" alt="image" src="https://github.com/user-attachments/assets/3191314b-ccd6-4237-bfb5-9e5f009c2b53" />

# 13. Для введенных с клавиатуры положительных целых чисел a и b (a≤b) определите:
# 1.сумму всех целых чисел от a до b;
# 2.произведение всех целых чисел от a до b;
# 3.среднее арифметическое всех целых чисел от a до b;
# 4.среднее геометрическое нечетных чисел от a до b.
# Отрезок поиска включает сами числа a и b. При выводе вещественных результатов оставьте два знака после запятой.

```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

import numpy as np

a = int(input("Введите значение a: "))
b = int(input("Введите значение b: "))
s = 0
p = 1
spis = []
for i in range(a, b+1):
  s += i
  p *= i
  spis.append(i)

sr = round(np.mean(spis),2)
g =  round(np.power(np.prod(spis[0::2]), 1/len(spis[0::2])),2)
print("Сумма = " , s)
print("Произведение = ", p)
print("Среднее арифметическое = " , sr)
print("Среднее геометрическое = ", g)
```
Пример вывода:

<img width="986" height="827" alt="image" src="https://github.com/user-attachments/assets/256749d0-9952-4e6f-92fc-a3704b0d66c7" />

# 14. Начав тренировки, лыжник в первый день пробежал s км. (s>0, вещественное число). Каждый следующий день он увеличивал пробег на p % (0<p≤100, вещественное число) от пробега предыдущего дня. Определите: 1.пробег лыжника за второй, третий, …, десятый день тренировок; 2.какой суммарный путь он пробежал за первые 10 дней тренировок. При выводе вещественных результатов оставьте один знак после запятой.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

s = float(input("Пробег за 1-й день (км.) = "))
p = float(input("На сколько увеличивает пробег (%) = "))
total = s

for i in range(2,11):

  s *= (p / 100) + 1
  print(f"Пробег за {i}-й день: {round(s,1)}")
  total += s

print(f"Суммарный пробег: {round(total,1)}")
```
Пример вывода:

<img width="964" height="788" alt="image" src="https://github.com/user-attachments/assets/0c3faae0-a678-47f6-b333-50c6e9616cf0" />

# 15. Известна масса каждого предмета в кг., загружаемого в грузовик. Определить, возможна ли перевозка груза, если грузоподъемность грузовика равна p кг
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

p = int(input("Введите грузоподъемность грузовика: "))
n = int(input("Введите количество предметов: "))
total = 0
for i in range(1,n+1):
   m = int(input(f"Введите вес {i} предмета: "))
   total += m
if total > p:
  print("Нет")
else:
  print("Да")
```
Пример вывода:

<img width="852" height="591" alt="image" src="https://github.com/user-attachments/assets/14edb73c-0ccb-4823-aa76-298e36559c40" />

# 16. В области несколько районов. Заданы площади, засеваемые пшеницей (га.), и средняя урожайность (ц/га) в каждом районе. Определите количество пшеницы, собранное по области. При выводе вещественных результатов оставьте один знак после запятой
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите количество районов: "))
total = 0
for i in range(1, n + 1):
  p = int(input(f"Введите количество полей {i}-го района: "))
  s = int(input(f"Введите среднюю урожаемость {i}-го района: "))
  c = p * s
  total += c
print(f"Собрано пшеницы: {round(total,1)}")
```
Пример вывода:

<img width="1020" height="597" alt="image" src="https://github.com/user-attachments/assets/0d520a88-8c4b-4c94-beb8-4086642389f1" />

# 17. Решите задачу № 2.7, организовав бесконечный цикл, который бы прерывался при выполнении условия, используя оператор break
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

total_sum = count = 0

while True:
    num = int(input("Введите число: "))
    if num == 0:  
        break     
    total_sum += num
    count += 1

print(f"Количество: {count}, Сумма: {total_sum}")
```
Пример вывода:

<img width="813" height="590" alt="image" src="https://github.com/user-attachments/assets/1a416438-74d2-4444-b5d8-e86debe2c52b" />

# 18. Предложение, введенное с клавиатуры, содержит слова из гласных и согласных букв кириллицы (регистр может быть различный), а также пробелы. Определите количество гласных и согласных букв в предложении. Для пропуска пробелов используйте оператор continue
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

s = str(input("Введите предложение: "))
low_reg = s.lower()
count_gl = 0
count_sogl = 0

for i in low_reg:
  if i in 'аеёиоуыэюя':
    count_gl += 1
  elif i == " ":
    continue
  else:
    count_sogl += 1
print(f"Количество гласных: {count_gl}, Количество согласных: {count_sogl}")
```
Пример вывода:

<img width="1053" height="599" alt="image" src="https://github.com/user-attachments/assets/a1102d04-8a13-484a-b486-4ce30a6dd4cb" />


# 19. Выведите на экран (в строку) все целые числа от a до b, кратные некоторому числу c
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

a = int(input("Введите число начала: "))
b = int(input("Введите число конца: "))
c = int(input("Введите число-делитель: "))
d = []
for i in range(a, b + 1):
  if i % c == 0:
    d.append(str(i))
    i += 1
print(" ".join(d))
```
Пример вывода:

<img width="764" height="521" alt="image" src="https://github.com/user-attachments/assets/b07a3e2b-e249-4714-826c-676616aae5ec" />


# 20. Выведите на экран (в строку) все трехзначные натуральные числа, сумма цифр которых равна целому числу n (0<n≤27).
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите число: "))
s = []
for i in range(100,1000):
  с_3 = i % 10
  с_2 = (i // 10) % 10
  c_1 = i // 100
  if с_3 + с_2 + c_1 == n:
    s.append(str(i))
print(" ".join(s))
```
Пример вывода:

<img width="761" height="476" alt="image" src="https://github.com/user-attachments/assets/b1983052-44a2-4e51-a148-20dbaf92b9a8" />


# 21. Известно количество учеников в классе и их рост (см.); рост мальчиков условно задан отрицательными числами. Определите средний рост мальчиков и средний рост девочек. При выводе вещественных результатов оставьте один знак после запятой.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите количество учеников: "))

r_sr_m = 0.0
r_sr_d = 0.0
kol_m = 0
kol_d = 0
for i in range(1, n +1):
  k = float(input((f"Введите рост {i} ученика: ")))
  if k < 0:
    r_sr_m += k
    kol_m += 1
  else:
    r_sr_d += k
    kol_d += 1
  i += 1
sr_m = (r_sr_m / kol_m) * (-1)
sr_d = r_sr_d / kol_d

print("Средний рост мальчиков: {:.1f}".format(sr_m))
print("Средний рост девочек: {:.1f}".format(sr_d))
```
Пример вывода:

<img width="1025" height="966" alt="image" src="https://github.com/user-attachments/assets/9e44b103-6805-4a27-96d9-aca721920f84" />


# 22. Даны n вещественных чисел. Определите максимальное и минимальное из них. При выводе вещественных результатов оставьте два знака после запятой.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите количество чисел: "))
s = []
for i in range(1, n+1):
   k = float(input(f"Введите {i} число: "))
   s.append(k)
   i += 1
mx = max(s)
mn = min(s)
print(f"Максимум: {mx}, минимум: {mn}")
```
Пример вывода:

<img width="866" height="551" alt="image" src="https://github.com/user-attachments/assets/a7669130-a8c3-4042-8563-d72703bf561f" />

# 23. Дано натуральное число n. Определите, является ли оно членом последовательности Фибоначчи
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите число: "))
a = 0
b = 1
if n < 0:
  print ("Нет")
elif n == 0 or n == 1:
  print ("Да")
else:
  while b < n:
    c = a + b
    a = b
    b = c
  if b == n:
    print ("Является")
  else:
    print ("Не является")
```
Пример вывода:

<img width="872" height="665" alt="image" src="https://github.com/user-attachments/assets/75744039-300d-4f06-89a2-b44939ce2239" />


# 24. Дано n вещественных чисел. Определите, является ли последовательность упорядоченной по возрастанию. В случае отрицательного ответа выведите порядковый номер числа, нарушающего такую упорядоченность.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите количество чисел: "))

index = -1
s = []
for i in range(1, n + 1):
    num = float(input(f"Введите {i} число = "))
    s.append(num)


for j in range(0, n - 1):
    if s[j] >= s[j + 1]:
        index = j + 2
        break

if index == -1:
    print("Последовательность упорядочена по возрастанию")
else:
    print(f"Не является упорядоченной, порядковый номер числа: {index}")
```
Пример вывода:

<img width="1299" height="860" alt="image" src="https://github.com/user-attachments/assets/4bf23c1b-2d7b-4481-98a9-736a09ddeb31" />

# 5. Выведите на экран таблицу умножения на n (2<n≤9) в виде:
```
n = int(input("Введите число n: "))
if n <= 2 or n > 9:
    print("n должно быть в диапазоне 2 < n ≤ 9")
else:
    for i in range(1, n+1):
        for j in range(1, n+1):
            print(f"{i} × {j} = {i*j:2}", end="   ")
        print()
```
Пример вывода:

<img width="902" height="516" alt="image" src="https://github.com/user-attachments/assets/85943e42-ab79-4bc0-9ae7-eafcaa334c8a" />

# 26. Выведите графическое изображения делимости чисел от 1 до n (значение n вводится с клавиатуры) - в каждой строке напечатайте очередное число и столько символов * , сколько делителей у этого числа. Например, если n=4, на экране должно быть напечатано: 1 * 2 ** 3 ** 4 ***
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите количество чисел: "))
for i in range(1, n + 1):
  k = 0
  for j in range(1, i + 1):
    if i % j == 0:
      k += 1
  print(i , k * "*")
```
Пример вывода:

<img width="837" height="483" alt="image" src="https://github.com/user-attachments/assets/60b5b2b1-a6cb-41af-8385-3505b1353b24" />

# 27. Выведите на экран (в строку) n первых простых чисел.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите число: "))

spisok = []
a = 2
while len(spisok) < n:
  deliteli = 0
  for i in range(1, a + 1):
    if a % i == 0:
      deliteli += 1
  if deliteli == 2:
    spisok.append(str(a))
  a += 1
print(" ".join(spisok))
```
Пример вывода:

<img width="836" height="584" alt="image" src="https://github.com/user-attachments/assets/54bcee53-1b54-45a1-b01c-8c302424a71b" />

# 28. Составьте программу для нахождения всех натуральных решений уравнения x^2+y^2+z^2=k^2, где x,y,z∈[1,30], а k вводится с клавиатуры.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

k = int(input("Введите значение k: "))
for x in range(1, 31):
  for y in range(1, 31):
    for z in range(1, 31):
      if (x ** 2) + (y ** 2) + (z ** 2) == k ** 2:
        print(f"x = {x}, y = {y}, z = {z}")
```
Пример вывода:

<img width="927" height="782" alt="image" src="https://github.com/user-attachments/assets/50671323-0129-4cd5-9a81-0c72369d11fe" />

# 29. Дан список из n вещественных чисел, введенных с клавиатуры (среди чисел есть по крайней мере одно положительное и отрицательное число). Сформируйте из него 2 списка: 1.положительных чисел, используя списковые включения; 2.отрицательных чисел, не используя списковые включения. Выведите на экран: 1.исходный список; 2.получившиеся списки; 3.среднее арифметическое первого списка и среднее геометрическое второго списка. При выводе вещественных результатов оставьте два знака после запятой
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

import numpy as np
n = int(input("Введите количество чисел: "))
numbers = []
for j in range(n):
    num = float(input(f"Введите число {j+1}: "))
    numbers.append(num)

polog = [num for num in numbers if num > 0]
otr = []
for k in numbers:
  if k < 0:
    otr.append(k)
ar = sum(polog) / len(polog)
sr = np.prod(otr) ** (1/len(otr))
print(f"Исходный список: {numbers}")
print(f"ПОложительные числа: {polog}")
print(f"Отрицательные числа: {otr}")
print(f"Среднее арифметическое: {round(ar,2)}")
print(f"Среднее геометрическое: {round(sr,2)}")
```
Пример вывода:

<img width="1006" height="968" alt="image" src="https://github.com/user-attachments/assets/54de83ac-795f-4361-9c69-903699fa3d5f" />

# 30. Дан список целых чисел, введенных с клавиатуры (длина неизвестна). Ответьте на вопросы: 1.являются ли все элементы положительными числами? 2.есть ли хотя бы один нулевой элемент в списке? 3.являются ли все элементы четными числами? 4.есть ли хотя бы один нечетный элемент в списке? Каждый из пунктов выполните дважды: используя стандартный проход в цикле (например, через алгоритм с флажком), и используя функции any() и/или all()
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Введите количество чисел: "))
num = []
for i in range(1 , n + 1):
  k = int(input(f"Введите число {i}: "))
  num.append(k)
# цикл положительных чисел
flag = -1
for j in num:
  if j < 0:
    flag = 1

if flag == -1:
  print("Да, все положительные")
else:
  print("Нет, есть отрицательные")


p = all(j > 0 for j in num)
if p:
  print("Да, все положительные")
else:
  print("Нет, есть отрицательные")

# цикл нулевого элемента
flag = -1
for j in num:
  if j == 0:
    flag = 1

if flag == 1:
  print("Да, есть ноль")
else:
  print("Нет, нуля нет")

n = any(j == 0 for j in num)
if n:
  print("Да, есть ноль")
else:
  print("Нет, нуля нет")

# цикл четности чисел

flag = -1
for j in num:
  if j % 2 ==  0:
    flag = 1

if flag == -1:
  print("Да, все четные")
else:
  print("Нет, есть нечетные")

c = all(j % 2 == 0 for j in num)
if c:
  print("Да, все четные")
else:
  print("Нет, есть нечетные")

#Поиск нечетного числа

flag = -1
for j in num:
  if j % 2 !=  0:
    flag = 1

if flag == 1:
  print("Да, есть нечетное")
else:
  print("Нет, все четные")

d = any(j % 2 != 0 for j in num)
if d:
  print("Да, есть нечетное")
else:
  print("Нет, все четные")
```
Пример вывода:

<img width="618" height="365" alt="image" src="https://github.com/user-attachments/assets/557bdc9e-58f2-4c35-bb6a-de38be8d6c97" />

# 31. Дано предложение. Выведите его на экран, удалив из него все слова, содержащие произвольную букву (вводится с клавиатуры)
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

sentence = input("Введите предложение: ")
letter = input("Введите букву для удаления: ")

result = ' '.join([word for word in sentence.split() if letter.lower() not in word.lower()])

print("Результат:", result)
```
Пример вывода:

<img width="1237" height="416" alt="image" src="https://github.com/user-attachments/assets/826ea25b-81e2-40e0-a3cd-39919248f15f" />

# 32. В зрительном зале кинотеатра n рядов, количество мест в которых может меняться. Разработчик смоделировал занятость мест как двумерный массив (список из списков), где каждый вложенный список содержит информацию о проданных местах в соответствующем ряду (1 - занято, 0 - свободно): [ [0, 0, 1], # 1 ряд, первые 2 места свободны [1, 1, 1, 1], # 2 ряд, все места заняты ... ] Напишите программу, которая позволит пользователю увидеть количество свободных мест, а также, введя номер ряда и места, получить информацию - свободно оно или нет. Данные о занятости мест вводятся с клавиатуры (набор из 0 и 1 для каждого ряда).

```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input('Количество рядов = '))

seats = []
for i in range(n):
    row = [int(item) for item in input().split()]
    seats.append(row)


n_p, m_p = [int(item) for item in input("Введите ряд и место через пробел: ").split()]

row_index = n_p - 1
seat_index = m_p - 1


if row_index < 0 or row_index >= len(seats):
    print("Такого ряда не существует")
elif seat_index < 0 or seat_index >= len(seats[row_index]):
    print("Такого места не существует")
else:
    is_free = seats[row_index][seat_index] == 0
    print(f"Место свободно: {is_free}") 
```
Пример вывода:

<img width="1200" height="934" alt="image" src="https://github.com/user-attachments/assets/ce50169a-e8f1-4e4d-897b-1b9f708ca013" />

# 33. Вводится список из n сотрудников в указанном формате. Далее: определите самого «молодого» и самого «старого» сотрудника, используя функцию sorted() ; сформируйте 2 отельных списка: мужчин и женщин и ответьте, в каком из списков больше имен, начинающихся на букву k (вводится с клавиатуры).
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input('n = '))

employees = []

for i in range(n):
  data = input().split()
  data[4] = int(data[4])
  employees.append(data)

sort = sorted(employees, key=lambda x: x[4])

employee_min = sort[0]
employee_max = sort[-1]
print("Cамый \"молодой\": {}".format(" ".join(employee_min[:3])))
print("Cамый \"старый\": {}".format(" ".join(employee_max[:3])))


men = [emp for emp in employees if emp[3] == "М"]
women = [emp for emp in employees if emp[3] == "Ж"]

k = input("Введите букву начала имени = ").upper()

men_k_count = 0
for man in men:
    if man[1][0].upper() == k:
        men_k_count += 1

women_k_count = 0
for woman in women:
    if woman[1][0].upper() == k:
        women_k_count += 1

if men_k_count > women_k_count:
    print("У мужчин таких имен больше")
elif women_k_count > men_k_count:
    print("У женщин таких имен больше")
else:
    print("Количество таких имен одинаково")
```
Пример вывода:

<img width="729" height="230" alt="image" src="https://github.com/user-attachments/assets/0859131b-9dce-4d17-87b1-1d70ce95cc58" />

# 34. Вводится список из n годовых вкладов, предлагаемых банками, в указанном формате. Далее определите (гарантируется, что искомый банк - один): самый доступный банк (с наименьшей первоначальной суммой); самый выгодный банк, принимая, что за год прибыль = сумма * процент / 100 . При выводе финансовых значений оставьте два знака после запятой.
```
# Выполнил: Воробьева Екатерина Романовна
# Группа: АБП - 231
# E-mail: kw849667@gmail.com

n = int(input("Количество банков = "))

deposits = []
for i in range(n):
    data = input().split()
    bank_dict = {
        "name": data[0],
        "initial_sum": int(data[1]),
        "rate": float(data[2])
    }
    deposits.append(bank_dict)

# 2. Самый доступный банк (с минимальной первоначальной суммой)
min_bank = deposits[0]
for bank in deposits:
    if bank['initial_sum'] < min_bank['initial_sum']:
        min_bank = bank

# 3. Самый выгодный банк (с максимальной прибылью)
max_profit_bank = deposits[0]
max_profit = deposits[0]['initial_sum'] * deposits[0]['rate'] / 100

for bank in deposits:
    profit = bank['initial_sum'] * bank['rate'] / 100
    if profit > max_profit:
        max_profit = profit
        max_profit_bank = bank

print(f"Самый доступный банк: {min_bank['name']}, первоначальная сумма: {min_bank['initial_sum']:.2f} руб.")
print(f"Самый выгодный банк: {max_profit_bank['name']}, прибыль: {max_profit:.2f} руб.")
```
Пример вывода:

<img width="1036" height="189" alt="image" src="https://github.com/user-attachments/assets/cc83bce1-0c20-405b-915e-0f439c695018" />

# Вывод:
Я изучила основные управляющие конструкции языка Python: условный оператор и циклы, научилась использовать управляющие структуры для решения задач различной сложности, развила умение комбинировать условия и циклы для оптимизации алгоритмов.
