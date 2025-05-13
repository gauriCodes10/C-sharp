using System;

class Program
{
    static void Main()
    {
        int[] numbers = new int[10];

        Console.WriteLine("Enter 10 integers:");

        for (int i = 0; i < numbers.Length; i++)
        {
            Console.Write($"Element {i + 1}: ");
            numbers[i] = Convert.ToInt32(Console.ReadLine());
        }

        Array.Sort(numbers);

        Console.WriteLine("\nElements in increasing order:");
        foreach (int number in numbers)
        {
            Console.Write(number + " ");
        }

        Console.WriteLine();
}
}



Enter 10 integers:
Element 1: 1
Element 2: 2
Element 3: 3
Element 4: 4
Element 5: 5
Element 6: 6
Element 7: 7
Element 8: 8
Element 9: 9
Element 10: 11

Elements in increasing order:
1 2 3 4 5 6 7 8 9 11 
