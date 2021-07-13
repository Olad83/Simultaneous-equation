# Simultaneous-equation


using System.Dynamic;
using System.Data;
using System;

namespace crammers_2
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Simultaneous equation by crammers method!");

            Console.Write("a = ");
            double a = Convert.ToInt32(Console.ReadLine());

            Console.Write("b = ");
            double b = Convert.ToInt32(Console.ReadLine());

            Console.Write("e = ");
            double e = Convert.ToInt32(Console.ReadLine());

            Console.Write("c = ");
            double c = Convert.ToInt32(Console.ReadLine());
            
            Console.Write("d = ");
            double d = Convert.ToInt32(Console.ReadLine());

            Console.Write("f = ");
            double f = Convert.ToInt32(Console.ReadLine());

            double Dx = e*d - b*f;
            double Dy = a*f - e*c;
            double D  = a*d - b*c;

            double x = Dx/D;
            double y = Dy/D;

            if (D == 0)
            {Console.WriteLine("The Equation has no Solution");
                
            }
            else
            {
                Console.WriteLine("X = " + x);
                Console.WriteLine("Y = " + y);
            }


        }
