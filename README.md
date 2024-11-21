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

struct Point

{
    public int X, Y; 
}

Point p = new Point { X = 1, Y = 1 };

> Arrays

int[] digits = { 1, 2, 3, 4 };

> Classes & Encapsulation

class Knight

{
    public int Position {get; set;}
    public string Color { get; set; }
    public string GetColor() => Color;
    public void Move()
}


> Abstraction

abstract class Car

{
    public abstract void Start();
}


class Vroom : Car

{ 
    public override Start() => Console.WriteLine("Vroom Vroom Vroom Engine started");
}


> Inheritance

class Weapon

{
    public string Jump { get; set; }
    public int ExcellentDamage { get; set; }
}

class Shield : Weapon

{ 
    public Shield(string Jump, int ExcellentDamge) : base (Jump, ExcellentDamage) {}  
}


> Polymorphism

class Man

{
    public virtual void Run(int meters) => Console.WriteLine($"Running {meters} meters.");
}

class Nike : Man

{
    public override void Run(int meters) => Console.WriteLine($"Running {meters} meters with jumping!");
}

> Access Modifiers

public: Accessible anywhere.

private: Accessible only within the class.

protected: Accessible in the class and derived classes.

internal: Accessible within the same assembly.

protected internal: Accessible within the same assembly or by derived classes.

    
