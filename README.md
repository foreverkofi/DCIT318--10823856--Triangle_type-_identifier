using System;
namespace TriangleTypeIdentifier
{  class Program
  {
        static void Main(string[] args)
        {
            // enter the lengths of the three sides of the triangle
            Console.Write("Enter the length of the first side of the triangle: ");
            double side1 = double.Parse(Console.ReadLine());

            Console.Write("Enter the length of the second side of the triangle: ");
            double side2 = double.Parse(Console.ReadLine());

            Console.Write("Enter the length of the third side of the triangle: ");
            double side3 = double.Parse(Console.ReadLine());

            // the triangle based on the side lengths
            if (side1 == side2 && side2 == side3)
            {
                Console.WriteLine("The triangle is Equilateral.");
            }
            else if (side1 == side2 || side2 == side3 || side1 == side3)
            {
                Console.WriteLine("The triangle is Isosceles.");
            }
            else
            {
                Console.WriteLine("The triangle is Scalene.");
            }
        }
    }
}
