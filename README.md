# INHERITANCE
## AIM:
To write a C# program to print some messages using hierarchical inheritance.

## ALGORITHM:
### STEP 1:
Create a base class.

### STEP 2:
Create two child class.

### STEP 3:
Create a constructor in the base class and print a message.

### STEP 4:
Create a function in child class to print a message.

## PROGRAM:
```
NAME : PAARKAVY B
REG NO : 212221230072
```

```
using System;
namespace Autovechicle
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("Tyre Constructor");
        }
        public virtual void Display()
        {
            Console.WriteLine("Method in tyre class");
        }
    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("Scooter Constructor");
        }

        public override void Display()
        {
            base.Display();
            Console.WriteLine("Method in Scooter");
        }
    }

    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("Car Constructor");
        }

        public override void Display()
        {
            base.Display();
            Console.WriteLine("Method in Car");
        }
    }
    public class Program
    {
        public static void Main(string[] args)
        {
            scooter s = new scooter();
            s.Display();
            car c = new car();
            c.Display();
        }
    }
}
```

## OUTPUT:
![output](op1.png)

## RESULT:
Thus, C# program to print some messages using hierarchical inheritance is written and executed sucCessfully.