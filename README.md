# Assignment2
STM_Assignment
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using NUnit.Framework;
using Assignment_STM;

namespace STM_Unittest
{
    [TestFixture]
    class STM_Unittest
    {
        [Test]
        public static void input10_input10_input10_outputEquilateral()
        {
            string output = string.Empty;
            string expectedoutput = string.Empty;
            string actualresult = string.Empty;

            //Arrange
            int f = 10;
            int s = 10;
            int t = 10;
            output = TriangleSolver.Analyze(f, s, t);
            expectedoutput = output;

            //Act
            actualresult = "........Given Triangle is Equilateral.......";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }

        [Test]
        public void input5_input6_input7_outputScalene()
        {
            string output = string.Empty;
            string expectedoutput = string.Empty;
            string actualresult = string.Empty;

            //Arrange
            int f = 5;
            int s = 6;
            int t = 7;
            output = TriangleSolver.Analyze(f, s, t);
            expectedoutput = output;

            //Act
            actualresult = "........Given Triangle is Scalene........";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }

        [Test]
        public void input8_input6_input8_outputIsosceles()
        {
            string output = string.Empty;
            string expectedoutput = string.Empty;
            string actualresult = string.Empty;

            //Arrange
            int f = 8;
            int s = 6;
            int t = 8;
            output = TriangleSolver.Analyze(f, s, t);
            expectedoutput = output;

            //Act
            actualresult = "........Given Triangle is Isosceles.......";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }

        [Test]
        public void input12_input12_input24_outputnotTriangle()
        {
            string output = string.Empty;
            string expectedoutput = string.Empty;
            string actualresult = string.Empty;

            //Arrange
            int f = 12;
            int s = 12;
            int t = 24;
            output = TriangleSolver.Analyze(f, s, t);
            expectedoutput = output;

            //Act
            actualresult = ".........Is not a triangle........";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }

        [Test]
        public void input22_input22_input22_outputEquilateral()
        {
            string output = string.Empty;
            string expectedoutput = string.Empty;
            string actualresult = string.Empty;

            //Arrange
            int f = 22;
            int s = 22;
            int t = 22;
            output = TriangleSolver.Analyze(f, s, t);
            expectedoutput = output;

            //Act
            actualresult = "........Given Triangle is Equilateral.......";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }

        [Test]
        public void input7_input11_input5_outputScalene()
        {
            string output = string.Empty;
            string expectedoutput = string.Empty;
            string actualresult = string.Empty;

            //Arrange
            int f = 7;
            int s = 11;
            int t = 5;
            output = TriangleSolver.Analyze(f, s, t);
            expectedoutput = output;

            //Act
            actualresult = "........Given Triangle is Scalene........";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }

        [Test]
        public void input11_input11_input5_outputIsosceles()
        {
            string output = string.Empty;
            string expectedoutput = string.Empty;
            string actualresult = string.Empty;

            //Arrange
            int f = 11;
            int s = 11;
            int t = 5;
            output = TriangleSolver.Analyze(f, s, t);
            expectedoutput = output;

            //Act	
            actualresult = "........Given Triangle is Isosceles.......";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }

        [Test]
        public void input18_input9_input9_outputnotTriangle()
        {
            string output = string.Empty;
            string expectedoutput = string.Empty;
            string actualresult = string.Empty;

            //Arrange
            int f = 18;
            int s = 9;
            int t = 9;
            output = TriangleSolver.Analyze(f, s, t);
            expectedoutput = output;

            //Act
            actualresult = ".........Is not a triangle........";

            //Assert
            Assert.AreEqual(expectedoutput, actualresult);
        }
    }
}
