using System;

class Program
{
    static void Main()
    {
        Console.Write("ساعت را وارد کنید (0 تا 24): ");
        int hour = int.Parse(Console.ReadLine());

        if (hour >= 0 && hour <= 24)
        {
            if (hour >= 0 && hour < 6)
            {
                Console.WriteLine("نیمه شب بخیر");
            }
            else if (hour >= 6 && hour < 12)
            {
                Console.WriteLine("صبح بخیر");
            }
            else if (hour >= 12 && hour < 18)
            {
                Console.WriteLine("بعد از ظهر بخیر");
            }
            else
            {
                Console.WriteLine("شب بخیر");
            }
        }
        else
        {
            Console.WriteLine("سارا خانم، لطفا عددی در بازه ی ۰ تا ۲۴ وارد کن");
        }
    }
}
