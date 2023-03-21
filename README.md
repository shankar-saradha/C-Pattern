# Ex.No:3 Pattern
## Aim:
To write a C# program for a pascal's triangle
## Equipment Required:
Microsoft Visual Studio 2022 (or Lower) or Any other C# compiler
## Algorithm:
### Step 1:
Create a new Class.
### Step 2:
Declare two variables of int data type one to store the input from user for no.of rows and another the value for printing.
### Step 3:
Get the number of rows from the user.
### Step 4:
Using for loop print the rows and columns and space.
### Step 5:
Check the first and last rows of the triange is 1 using if condition.
### Step 6:
Otherwise use else to print the inner value
```val = val * (i - j + 1) / j```
### Step 7:
Print the program.
### Step 8:
End of the Program.
## Program:
Program Developed by: Shankar Saradha
<br/>
Register No.: 212221240052
```C#
using System;
using System.Collections.Generic;
using System.Globalization;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Pascal_Triangle
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int row;
            Console.Write("Enter no. of rows: ");
            row = Convert.ToInt32(Console.ReadLine());
            int c = 1;
            for (int i = 0; i < row; i++)
            {
                for (int j = 1; j <= row - i; j++)
                    Console.Write(" ");
                for (int k = 0; k <= i; k++)
                {
                    if (k == 0 || i == 0)
                        c = 1;
                    else
                        c = c * (i - k + 1) / k;
                    Console.Write(c + " ");
                }
                Console.WriteLine();
            }
            Console.Read();
        }
    }
}
       
```
## Output:
![image](https://user-images.githubusercontent.com/93427017/226514500-abbdb171-470d-4f89-be4e-b789de370442.png)
## Result:
Hence, a C# program for a pascal's triangle is executed successfully.
