# ProjetoForMedia
Exercicio em classe

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ProjetoForMedia
{
    public class Program
    {
        static void Main(string[] args)
        {
            /*Crie um projeto chamado ProjetoForMedia e receba o nome do aluno
             * e utilize o for para receber 3 notas inteiras, no final calcu-
             * le a media.
            */
            string nomeAluno;
            int nota, media, soma =0;

            Console.WriteLine("Informe o nome do aluno: ");
            nomeAluno = Console.ReadLine();

            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"Informe a {i}ª nota: ");
                nota = Convert.ToInt32(Console.ReadLine());
                soma += nota;
            }
            media = soma / 3;
            Console.WriteLine("Media das 3 notas: " + media);

            Console.ReadKey();
        }
    }
}
