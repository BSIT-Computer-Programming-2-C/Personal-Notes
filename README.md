# Personal-Notes

Encapsulation: Protects object data and controls access.

Abstraction: Hides implementation details, showing only essential functionality.

Inheritance: Allows classes to derive from other classes.

Polymorphism: Enables methods to take different forms based on the object type.


Primitive Data Types in C#

int num1 = 9;           // 32-bit integer

double num2 = 2.1;      // 64-bit floating point

float num3 = 3.1f;      // 32-bit floating point (need 'f')

bool num4 = true;       // true or false

byte num5 = 121;        // 8-bit integer (0-255

char num6 = 'U';        // Single character

string num7 = "HelloWorld";  // Sequence of characters


> Structures (Value Types)

using System;

struct Point
{
    public int X, Y;
}

class Program
{
    static void Main(string[] args)
    
{
    
// Initialize the Point struct

Point p = new Point { X = 1, Y = 1 };

// Output the values of X and Y

Console.WriteLine($"Point coordinates: X = {p.X}, Y = {p.Y}");

}

}

![Screenshot 2024-11-28 211812](https://github.com/user-attachments/assets/fdf3b3e0-f71c-4935-8879-91e7856c8643)


> Arrays

using System;

class Knight

{

// Properties with automatic getters and setters (encapsulation)

public int Position { get; set; }

public string Color { get; set; }

// Method to get the color of the knight

public string GetColor() => Color;

// Method to move the knight (for now it will just print a message)

public void Move()
{
Console.WriteLine("The knight is moving.");
}
}

class Program

{

static void Main(string[] args)

{

// Create an instance of the Knight class

Knight knight = new Knight

{

Position = 1, // Initial position

Color = "White" // Knight color

};

// Display knight's color and position

Console.WriteLine($"Knight Color: {knight.GetColor()}");

Console.WriteLine($"Knight Position: {knight.Position}");

// Move the knight

knight.Move();

}

}

![Screenshot 2024-11-28 212157](https://github.com/user-attachments/assets/ca0a0451-f594-47c3-ae1c-619ed8199622)


> Abstraction

abstract class Car

{

public abstract void Start();

}

class Vroom : Car

{

public override void Start();

{

Console.WriteLine("Vroom Vroom Vroom Engine Started");

}

}

class Program

{

static void Main(String[] args)

{

Car myCar = new Vroom();

myCar.Start();

}

}

![Screenshot 2024-11-30 225026](https://github.com/user-attachments/assets/c0355604-28b0-45f0-9733-9ff9c5b49157)


> Inheritance

using System;

abstract class Weapon

{

public string Jump { get; set; }

public int ExcellentDamage { get; set; }

public Weapon(string jump, int excellenDamage)

{

Jump = jump;

ExcellentDamage = excellentDamage;

}

public virtual void Attack()

{

Console.WriteLine($"Weapon attacks with {ExcellentDamage} damage!");

}

public override string ToString()

{

return $"Weapon [Jump = {Jump}, Excellent={ExcellentDamage}]";

}

}

class Shield : Weapon

{

public int Defence { get; set; }

public Shield (string jump, int excellentDamage, int defence)

:base(jump, excellentDamage)

{

Defence = defence;

}

public override void Attack()

{

Console.WriteLine($"Shield attacks with {ExcellentDamage} damage and defends with {Defence} defence.");

}

public void Defend()

{

Console.WriteLine($"Shield provedes defence of {Defence}!":

}

public override string ToString()

{

return $"Shhield [Jump = {Jump}, ExcellentDamage={EcxellentDamage}, Defence={Defence}";

}

}

class program

{

static void Main()

{

Shield myShield = new Shield("High Jump", 50, 20);

myShield.Attack();

myShield.Defend();

Console.WriteLine(myShield.ToString());

}

}

![Screenshot 2024-11-30 231311](https://github.com/user-attachments/assets/fca2f5e3-b4a4-4ddd-9d19-9804fa371e4e)


> Polymorphism

using System;

class Man

{

public virtual void Run(int meters)

{

Console.WriteLine($"Running {meters} meters.");

}

public virtual void DisplayDetails()

{

Console.WriteLine("This is a generic man.");

}
}

> Access Modifiers

public: Accessible anywhere.

private: Accessible only within the class.

protected: Accessible in the class and derived classes.

internal: Accessible within the same assembly.

protected internal: Accessible within the same assembly or by derived classes.

    
