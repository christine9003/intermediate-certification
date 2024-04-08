//Задача 1: Задайте значения M и N. Напишите программу, которая выведет все натуральные числа в промежутке от M до N. 
//Использовать рекурсию, не использовать циклы.




//Задача 2: Напишите программу вычисления функции Аккермана с помощью рекурсии. Даны два неотрицательных числа m и n.

using System;

public class Program
{
    public static void Main()
    {

        int AkkermanFunc(int m, int n)
        {
            if (m == 0)
            {
                return n + 1;
            }
            if (m > 0 && n == 0)
            {
                return AkkermanFunc(m - 1, 1);
            }
            return AkkermanFunc(m - 1, AkkermanFunc(m, n - 1));
        }

        Console.WriteLine(AkkermanFunc(3, 2));
    }
}



//Задача 3: Задайте произвольный массив. Выведете его элементы, начиная с конца. Использовать рекурсию, не использовать циклы.

class Program

{

    static void Main(string[] args)

    {

        int[] array = { 1, 2, 5, 7, 8, 0, 10, 20, 25, 34 };

        PrintArrayReversed(array, array.Length - 1);

    }


    static void PrintArrayReversed(int[] array, int index)

    {

        if (index >= 0)

        {

            Console.Write(array[index] + " ");

            PrintArrayReversed(array, index - 1);

        }

    }

}
  
