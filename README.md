# Eligibility-for-Admission

## Aim:
To write C# program to find the eligibility for admission to an engineering course

## Algorithnm:
### Step 1:
Create new class

### Step 2:
Initiate the variables for maths, physics and chemistry and get the value from the user.

### Step 3:
Convert the values to integer values.

### Step 4:
Calculate the sum of all three subjects and maths-physics total.

### Step 5:
Check for the given criteria for eligibility using if-else statements.

### Step 6:
Display whether the person is eligible for admission or not based on the given criteria.

### Step 7:
Exit the Program.

## Program:
```cs
using System;

namespace exp1
{
    class Eligibility
    {
        static void Main(string[] args)
        {
            string name;
            int math, phy, chem;
            Console.Write("Enter your name:");
            name = Console.ReadLine();
            Console.Write("Enter Maths Marks:");
            math = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter Physics Marks:");
            phy = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter Chemistry Marks:");
            chem = Convert.ToInt32(Console.ReadLine());
            int Sum = math + phy + chem;
            int MPTot = math + phy;
            if (math >= 65 && phy >= 55 && chem >= 50)
            {
                if (Sum >= 180 || MPTot >= 140)
                {
                    Console.WriteLine(name + " is eligible for admission to an engineering course.");
                }
                else
                {
                    Console.WriteLine(name + " is not eligible for admission to an engineering course due to insufficient marks.");
                }
            }
            else
            {
                Console.WriteLine(name + " is not eligible for admission to an engineering course due to insufficient marks.");
            }
            Console.Read();
        }
    }
}
```
## Output:
![ss2](https://user-images.githubusercontent.com/93427254/225370643-b50cd18d-292f-42c8-ab02-3681cfaf78dc.png)
![ss1](https://user-images.githubusercontent.com/93427254/225370653-face51d5-2412-4a75-99ae-0451e1a9a676.png)

## Result:
Thus a C# program to check eligibility for admission is executed successfully.
