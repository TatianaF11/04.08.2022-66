//void Zadacha66()
{
// Задача 66: Задайте значения M и N. Напишите программу, которая найдёт сумму 
// натуральных элементов в промежутке от M до N.
// M = 1; N = 15 -> 120
// M = 4; N = 8. -> 30
    Console.WriteLine("Введите число- М:");
    int M = Convert.ToInt32(Console.ReadLine());
    Console.WriteLine("Введите число- N:");
    int N = Convert.ToInt32(Console.ReadLine());
    Console.Write($"Сумма чисел от {M} до {N} ровна: ");
    SumNumbers(M, N);
}

void SumNumbers(int m, int n, int sum = 0)
{
    if (m > n)
    {
        Console.Write(sum);
        return;
    }
    sum = sum + m;
    m++;
    SumNumbers(m, n, sum);
}
//Zadacha66();
