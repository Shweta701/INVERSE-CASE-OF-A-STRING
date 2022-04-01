# INVERSE-CASE-OF-A-STRING


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp7
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.Write("Enter aa string to cheak a string is inverse:");
            string s = Console.ReadLine();
            string[] arr = s.ToLower().Split();
            StringBuilder sb = new StringBuilder();
            for (int i = 0; i < arr.Length; i++)
            {
                var s1 = arr[i].ToUpper();
                string s2 = arr[i].Replace(arr[i][0], s1[0]);
                sb.Append(s2 + " ");

            }
            Console.WriteLine(sb);
            Console.ReadLine();

        }
    }
}
