# pythongeekbrains.lesson1
# задача1
a = 2 + 4 # задача1
print(a)

b = -1 + 3
print(b)

print(a, b)

numbers = input("Введите возраст >>>")
name = input("Введите имя >>>")
surname = input("Введите фамилию >>>")

# задача2
value_sec = int(input("Введите секунды >>>")) # задача2

minutes = value_sec // 60
if minutes >= 60:
    hours = minutes // 60
    minutes = minutes % 60
else:
    hours = 0
seconds = value_sec % 60
print("{:0>2}:{:0>2}:{:0>2}".format(hours, minutes, seconds))

# задача3
number = int(input("Введите число >>>")) 
a = number
print(a)
b = int('{}{}'.format(number, number))
print(b)
c = int('{}{}'.format(b, number))
print(c)
value = a + b + c
print(value)

# задача4
num = int(input("Введите целое число ,больше 9 >>>")) # задача4
a = 0
if num < 10:
    print("Вы ввели неверное число")
else:
    while num > 0:
        b = num % 10
        #print(b)
        if b > a:
            a = b
            #print(a)
        num = num // 10
print(a)

# задача5
value = float(input("Введите выручку >>>"))
costs = float(input("Введите издержки >>>"))
fin_res = value - costs
print("Прибыль =", fin_res)
if fin_res > 0:
    print("Выручка больше издержек")
    rent = fin_res / value
    print("Рентабельность =", rent)
else:
    print("Издержки больше выручки")
staff = int(input("Введите численность сотрудников >>>"))
fin_res_st = fin_res / staff
print(fin_res_st)


