# Vettori
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Vettori
{
    internal class Vector
    {
        public int x1 {  get; set; }
        public int y1 { get; set; }
        public int x2 { get; set; }
        public int y2 { get; set; }

        public override string ToString()
        {
            return string.Format("vettore :{0}; {1}", x1, y1);
        }


        public Vector(int x1, int y1)
        {
            this.x1 = x1;
            this.y1 = y1;

        }


        public int Somma1(int x1, int x2)
        {
            return x1 + x2;
        }

        public int Somma2(int y1, int y2)
        {
            return y1 + y2;
        }
    }
}
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Vettori
{
    internal class Program
    {
        static void Main(string[] args)
        {

            int x1 = 2;
            int y1 = 2;
            int x2 = 3;
            int y2 = 3;
            Vector v1 = new Vector(x1, y1) ;
            Vector v2 = new Vector(x2, y2) ;
            //int sommax = 0;


            int sommax = v1.Somma1(x1, x2);
            int sommay = v2.Somma1(y1, y2);

            Console.WriteLine("{0}; {1}", sommax, sommay);
            Console.ReadLine();
        }
    }
}
