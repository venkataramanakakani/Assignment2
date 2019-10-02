# Assignment2
STM_Assignment
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Assignment_STM
{
class Program
{
    static void Main(String[] args)
    {
        string uInput = "";
        bool menuItem = false;
        while (menuItem == false)
        {
            Console.WriteLine("1=Enter Triangle dimensions");
            Console.WriteLine("2 = Exit \n");
            Console.WriteLine("Choose the option above to continue:");
            uInput = Console.ReadLine();
            if (uInput != "1" && uInput != "2")
            {
                Console.WriteLine("You have choosen wrong option, please try  again:");
            }
            else if (uInput == "1")
            {
                Console.WriteLine("Enter all the sides of traingle:");
                Console.WriteLine("Enter First side:");
                int x = int.Parse(Console.ReadLine());

                Console.WriteLine("Enter Second side:");
                int y = int.Parse(Console.ReadLine());

                Console.WriteLine("Enter Third side:");
                int z = int.Parse(Console.ReadLine());

                string empty = string.Empty;
                empty = TriangleSolver.Analyze(x, y, z);
                Console.WriteLine("{0}", empty);
            }
            else
            {
                menuItem = true;
                break;
            }
        }
    }
}
}
