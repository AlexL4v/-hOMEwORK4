// Задача 1: Напишите программу, которая бесконечно запрашивает целые 
// числа с консоли. Программа завершается при вводе символа ‘q’ или 
// при вводе числа, сумма цифр которого чётная.
// Решение:
bool CheckForEvenNumberSum(int n)
{
    int s = 0;
    while (n > 0)
    {
        s = s + (n % 10);
        n = n / 10;
    }
    if (s % 2 == 0)
        return true;
    else
        return false;
}

string InputNumber()
{
    Console.WriteLine("Введите число:");
    string n = Console.ReadLine()!;
    return n;
}


while (true)
{
    string c = InputNumber();
    if (c == "q")
    {
        break;
    }
    else
    if (CheckForEvenNumberSum(Int32.Parse(c)))
    {
        break;
    }
}





// Задача 2: Задайте массив заполненный случайными трёхзначными числами.
// Напишите программу, которая покажет количество чётных чисел в массиве.
// Решение:
/*int[] massiv;
int l = new Random().Next(5, 10);
massiv = new int[l];
for (int i = 0; i < l; i++) 
{
    massiv[i] = new Random().Next(100, 1000);  
    Console.Write(massiv[i] + " ");      
    
}   
Console.WriteLine();
int count = 0;
for (int i = 0; i < l; i++) 
{
    if (massiv[i]%2 == 0)
    {
        count++;
    }
}

Console.WriteLine($"Количество четных чисел в массиве {count}");

// Задача 3: Напишите программу, которая перевернёт одномерный массив 
// (первый элемент станет последним, второй – предпоследним и т.д.)
// Решение:

int[] RandomMas(int s)
{
    int[] array = new int[s];
    for (int i = 0; i < array.Length; i++)
    {
        array[i] = new Random().Next(-9,10);
    }
    return array;
}

void PrintMas(int[] mas)
{
    foreach (var item in mas)
    {
        Console.Write($"{item}, ");

    }
    Console.WriteLine();
}

void ReversMasPrint(int[] s)
{
    
    int[] mas = new int[array];
    int l = mas.Length;
    for (int i = 0; i < 1/2(array.Length); i++)
    {
        int temp = mas[i];
        mas[i] = mas[l-1];
        mas[l-1]= temp;
        l=i-1;
    }
    return mas;
}
void PrintMas2(int[] mas)
{
    foreach (var item in mas)
    {
        Console.Write($"{item} ");

    }
    Console.WriteLine();
}
Console.WriteLine("Введите размер массива: ");
int s = Convert.ToInt32(Console.ReadLine());

int[] array = RandomMas(s);
PrintMas(array);
PrintMas2(ReversMas(RandomMas(s)));

﻿int[] FillArrayRandomly(int n)
{
    int[] array = new int[n];
    for (int i = 0; i < array.Length; i++)
    {
        array[i] = new Random().Next(1, 10);
    }
    return array;
}

void PrintArray(int[] arr)
{
    foreach (var item in arr)
    {
        Console.Write($"{item}, ");
    }
    Console.Write("\b\b ");
    Console.WriteLine();
}

double TurnArrayIntoNumberBackwards(int[] arr)
{
    double s = 0;
    for (int i = 0; i < arr.Length; i++)
    {
        double p = Math.Pow(10, i);
        s = s + arr[i]*p;
    } 
    return s;
}

int CountDigits(double N)
{
    int DigitAmount = 1;
    int p = 1;
    int n = Convert.ToInt32(N);
    while (N / p > 10)
    {
        p = p * 10;
        DigitAmount = DigitAmount + 1;
    }
    Console.WriteLine(DigitAmount);
    return DigitAmount;
}

int [] NumbertoArrayStraight (double n, int a)
{
    int [] arr = new int [a];
    for (int i = 0; i < arr.Length; i++)
    {
        arr[arr.Length - i - 1] = Convert.ToInt32(n) % 10;
        n = Convert.ToInt32(n)/10;
    }
    return arr;
}

Console.WriteLine("Введите размерность массива: ");
int n = Convert.ToInt32(Console.ReadLine());
int[] a = FillArrayRandomly(n);
PrintArray(a);
double count = TurnArrayIntoNumberBackwards(a);
Console.WriteLine(count);
int digits = CountDigits(count);
int [] array = NumbertoArrayStraight(count, digits);
PrintArray(array);
*/
