# Синтаксис Python

**range()** # Переберает числ
    range(stop) 
    range(start, stop[, step])
    
    range(5) -> 0 1 2 3 4
    range(1, 5) -> 1 2 3 4
    range(1, 5, 2) -> 1 3
Источник: https://pythonstart.ru/osnovy/funktsiya-range-python

**len()** # Возвращает количество элементов (длину) в объекте.

    x = "привет"
    len(x) == 6

Источник: https://pythonstart.ru/osnovy/len-python 


**.pop()** # Удаляет элемент по заданному индексу из списка и возвращает удаленный элемент.

**.remove()** # Удаляет значение из списка 

**.append()** # Добавляет в конец списка значение

Источник: https://pythonstart.ru/list/metod-pop-remove-python 

**max()** # Находит максимальное значение 

**min()** # Находит минимальное значение

**from random import randint** # Добавляет библиотеку с рандомом

**randint(-10, 10)** # Генерирует случайное число из диапазона 

**.split()** # Разбивает строку по указанному разделителю и возвращает список строк.

Источник: https://pythonstart.ru/string/metod-str-split-python 

**find()** # Возвращает наивысший индекс подстроки (если найден). Если не найден, возвращается -1.

    str.rfind(sub[, start[, end]] )


**find()** # Возвращает индекс первого вхождения подстроки (если найден).

Источник: https://pythonstart.ru/string/find-python 

**round()** # Возвращает число с плавающей запятой, округленное до указанного количества десятичных знаков.

Источник: https://pythonstart.ru/osnovy/round-python 

    def func(a_1, a_2, *args, **kwargs): # под '*' кортеж, под '**' словарь 
        return a_1, a_2, args, kwargs

    print(func(1, 2, 3, 4, 542, 124, 'wetwet', key_1=10, key_2=30))

    Вывод: (1, 2, (3, 4, 542, 124, 'wetwet'), {'key_1': 10, 'key_2': 30})

**bin()** # Переводит целое число в двоичное

**Найти корень квадратного уравнения Ax²+Bx+C=0**

https://all-python.ru/primery/kvadratnoe-uravnenie.html

https://skysmart.ru/articles/mathematic/kak-najti-diskriminant-kvadratnogo-uravneniya


**Работа с файлами**

    with open(f_path, 'a') as my_print:
        my_print.writelines(f'привет\n')
        
https://pythonstart.ru/osnovy/open-python

**type()** # Выводит тип объекта (str, int, float)

**try except**
    
    try: # Если при выполнении try возникнет ошибка, выполняется except
        print(fib.index(a))
    except:
        print('Такого числа нет в последовательности')

**text.index(что нужно найти)** # Найти индекс по элементу

https://pythonist.ru/kak-opredelit-indeks-elementa-spiska-v-python/

**lambda** # Как описать функцию если она нужна только один раз

    def maxi( a, b):
        if a > b:
            return a
        else:
            return b
    print(maxi(4, 5))
**Более компактный вариант:**

    # print((lambda a, b: a if a > b else b)(4, 5))

**abs()** # Возвращает абсолютное значение заданного числа.

Источник: https://pythonstart.ru/osnovy/funktsiya-abs-python 
