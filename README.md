# CF_228A_Horseshoe

using System;
 
namespace string_generation
{
    class Program
    {
        static void Main(string[] args)
        {
            string[] text = (Console.ReadLine()).Split(' ');
            int[] arr = new int[4];
            for(int i=0;i<4;i++)
            {
                arr[i] = int.Parse(text[i]);
            }
            Array.Sort(arr);
            int flag = 0;
 
            for(int i=0;i<3;i++)
            {
                if (arr[i] == arr[i + 1]) 
                flag++;
            }
            Console.WriteLine(flag);
        }
    }
}
