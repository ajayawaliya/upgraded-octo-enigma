# upgraded-octo-enigma
using System;
using System.Threading;

class Program
{
    static void Main()
    {
        int bikePosition = 0;
        int speed = 5;

        // Loop runs 20 times
        for (int i = 0; i < 20; i++)
        {
            // Move the bike forward
            bikePosition += speed;

            // Print activity
            Console.WriteLine("Bike is moving! Current position: " + bikePosition);

            // Simulate some waiting time (like a frame)
            Thread.Sleep(500); // 500ms pause
        }

        Console.WriteLine("Race finished!");
    }
}
