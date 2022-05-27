# Recursive-function

## Aim: 
To write a C# program to reverse a number using recursive function.

## Algorithm:

## Program:
```c#
using System;

namespace exp7
{
    class Program
    {
        int rem = 0, rev = 0;
        public int reverse(int n)
        {
            rem = n % 10;
            if (rem == 0) return rev;
            else
            {
                rev = rev * 10 + rem;
                return reverse(n / 10);
            }
        }
        static void Main(string[] args)
        {
            int n;
            Console.WriteLine("Enter a Number to reverse: ");
            n = Convert.ToInt32(Console.ReadLine());

            Program p1 = new Program();
            Console.WriteLine("Reversed Number is "+ p1.reverse(n));
        }
    }
}
```
## Output:
![image](https://user-images.githubusercontent.com/75235488/170664396-8221d957-d4d8-425b-b6df-dfc121360d52.png)

## Result:
C# program to reverse a number using recursive function is executed successfully.
