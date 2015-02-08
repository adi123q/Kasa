using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace ConsoleApplication1
{
    class Program
    {
        class Produkt
        {
            public int Ilość_Produktów;
            public int Cena_Produktów;
          
            public void Zniżka()
            {
                Console.WriteLine("Zniżka dla Ciebie wynosi 20%, czyli zapłacisz tylko :"+Ilość_Produktów* Cena_Produktów* 0.8);
            }
        }
        class Pokaz

        {
            static void Main(string[] args)
            {
                
                Produkt Mleko = new Produkt();
                
                
                Mleko.Ilość_Produktów = 5;
                Mleko.Cena_Produktów = 2;
                Console.WriteLine("Zniżka");
                Mleko.Zniżka();
            }
        }
    }
}
