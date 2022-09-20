# Знакомство с языком C#

## Комманды в терминале

**dotnet new console** - создание новаго проекта

**dotnet run** - запуск проекта

## Синтаксис

### _Через **Console** мы обращаемся к системному терминалу_

**Write()** - вывод в одну строку

**WriteLine()** - в конце перейти на новую строку

**ReadLine()** - считать строку из терминала

**new Random().Next(min, max)** - даст случайное целое число от **min** до **max**

**.ToLower()** - приводит значение регистра к маленьким строчный бурквал

**Convert.ToInt32()** - Конвертирует в int

**Console.Clear()** - Очистить терминал

**Console.WriteLine($"{Названние переменной} Hello"};** - Позволяет удобно склеивать текст

**break;** // Прерывает цикл

**string a = String.Empty;** // Создать пустую строку

### _Типы данных_ 
* **int** - челые числа
* **double** - дробные числа
* **string** - текст
* **bool** - истина или лож (true / fales)

## Цикл for:
    
    for(int i = 0; i < x; i++)
    {
        //действие
    }   
## Функции:
    int [название функции](int a, int b, int c)
    {
        //какое то действие
        return название переменной; // возвращает значение
    }

## void:
    void название(int a, int b, int c)
    {
        //процедура которая не возвращает результат
    }

## while
    while (условие)
    {
        //Действие
    }
    
## Массив
    int [] x = {1,2,3,4,5}; // Создаст массив [1,2,3,4,5]

    int []arrey = new int [10] // Создали новый массив в котором 10 элементов

    Console.WriteLine("[" + string.Join(",", arrey) + "]"); // так красиво можно выводить содержимое массива
    // Выведет на экран [1, 2, 3, ...]
    
## Двумерные массивы
    int[,] matrix = new int[3, 3]; // Создать двумерный массив 3 столбца, 3 строки
    
    
    // Рандомное заполнение массива
    void InputMatrix(int[,] matrix)
    {
        for (int i = 0; i < matrix.GetLength(0); i++)
        {
            for (int j = 0; j < matrix.GetLength(1); j++)
                matrix[i, j] = new Random().Next(-10, 11);
        }
    }
    
    
    // Вывод массива в консоль
    void PrintMatrix(int[,] matrix)
    {
        Console.WriteLine();
        for (int i = 0; i < matrix.GetLength(0); i++)
        {
            for (int j = 0; j < matrix.GetLength(1); j++)
                Console.Write(matrix[i, j] + " \t");
                Console.WriteLine();
        }
    }

## Сумма арефметической прогрессии
    //Формула ((A1 + An) / 2) * An 
    double n = Convert.ToInt32(Console.ReadLine());  // При использовании этой формулы не забыть поставить double
        
        // // Вариант 1
        //int sum = 0;
        // for (int i = 1; i <=n; i++)
        // {
        //     sum += i; //sum = sum + i; 
        // }
        //Console.Write(sum);
        й
    // Вариант 2
     Console.Write((1+n)/2*n); // 


