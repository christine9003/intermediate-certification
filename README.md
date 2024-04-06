//Задача 1: Задайте значения M и N. Напишите программу, которая выведет все натуральные числа в промежутке от M до N. 
//Использовать рекурсию, не использовать циклы.

Console.Clear();
int Prompt(string message)
{
    Console.Write(message);
    int result = Convert.ToInt32(Console.ReadLine());
    return result;
}

int SumOfElements(int n, int m)
{
    if (n == m) return n;
    else return SumOfElements(n + 1, m) + n;
}
