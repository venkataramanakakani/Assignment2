# Assignment2
STM_Assignment
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Assignment_STM
{
    public static class TriangleSolver
	{
        public static string Analyze(int f, int s, int t)
        {
            string output = string.Empty;

            if (f + s > t && s + t > f && t + f > s)
            {
                Console.WriteLine("......Forms a Triangle.......");

                if (f == s && s == t && t == f)
                {
                    output = "........Given Triangle is Equilateral.......";
                }
                else if (f == s || s == t || t == f)
                {
                    output = "........Given Triangle is Isosceles.......";
                }
                else
                {
                    output = "........Given Triangle is Scalene........";
                }
            }
            else
            {
                output = ".........Is not a triangle........";
            }
            return output;
        }
    }
}
