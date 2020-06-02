# calculo_raio_circulo
//Programa para calcular a Área de um círculo. Usuário faz input de dados (valor do Raio). *Programa criado para estudo
//Program made to calculate an Area of circle. User needs to input data (valeu of Raio). *Program was created just for practice

using System;
using System.Globalization;

namespace exemplo
{
    class Program
    {
        static void Main(string[] args)
        {
            //Pede para usuario inserir valor do Raio
            Console.WriteLine("Digite o valor do RAIO: ");

            //Input de dados pelo usuario (valor do Raio)
            double raio =double.Parse(Console.ReadLine(), CultureInfo.InvariantCulture);

            var PI = 3.14159;

            //calculo da area
            var area = PI * Math.Pow(raio,2);

            //Imprime o valor da Area com 4 casas decimais
            Console.WriteLine("Area igual a: " + area.ToString("F4",CultureInfo.InvariantCulture));
        }
    }
}
