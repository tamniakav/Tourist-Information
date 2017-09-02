# Tourist-Information
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4.Tourist_Information
{
    class Program
    {
        static void Main(string[] args)
        {
            string imperialUnits = Console.ReadLine();
            double value = double.Parse(Console.ReadLine());
            double metricValue = 0;

            switch (imperialUnits)
            {
                case "miles": metricValue = value * 1.6;
                    Console.WriteLine($"{value} {imperialUnits} = {metricValue:f2} kilometers");
                    break;
                case "inches":
                    metricValue = value * 2.54;
                    Console.WriteLine($"{value} {imperialUnits} = {metricValue:f2} centimeters");
                    break;
                case "feet":
                    metricValue = value * 30;
                    Console.WriteLine($"{value} {imperialUnits} = {metricValue:f2} centimeters");
                    break;
                case "yards":
                    metricValue = value * 0.91;
                    Console.WriteLine($"{value} {imperialUnits} = {metricValue:f2} meters");
                    break;
                case "gallons":
                    metricValue = value * 3.8;
                    Console.WriteLine($"{value} {imperialUnits} = {metricValue:f2} liters");
                    break;
            }
        }
    }
}
