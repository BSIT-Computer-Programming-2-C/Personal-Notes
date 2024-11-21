# Personal-Notes

Encapsulation: Protects object data and controls access.

Abstraction: Hides implementation details, showing only essential functionality.

Inheritance: Allows classes to derive from other classes.

Polymorphism: Enables methods to take different forms based on the object type.


Primitive Data Types in C#

int num1 = 1;           // 32-bit integer

double num2 = 1.1;      // 64-bit floating point

float num3 = 1.1f;      // 32-bit floating point (need 'f')

bool num4 = true;       // true or false

byte num5 = 111;        // 8-bit integer (0-255)

char num6 = 'A';        // Single character

string num7 = "Hello";  // Sequence of characters

Structures (Value Types)

struct Point

{
    public int X, Y;
    
}

Point p = new Point { X = 1, Y = 1 };

Arrays

int[] digits = { 1, 2, 3, 4 }; // Array of integers

Classes & Encapsulation

class Knight

{

    public int Position { get; set; }  // Property with getter and setter
    
    public string Color { get; set; }
    
    public string GetColor() => Color;
    
    public void Move() { /* Movement logic */ }
    
}

Abstraction

abstract class Car

{

    public abstract void Start();
    
}

class Vroom : Car

{

    public override void Start() => Console.WriteLine("Vroom started");
    
}

Inheritance

class Weapon

{

    public string Type { get; set; }
    
    public int Damage { get; set; }
    
}

class Sword : Weapon

{
    public Sword(string type, int damage) : base(type, damage) { }
    
}

Polymorphism

class Car

{

    public virtual void Drive(int miles) => Console.WriteLine($"Driving {miles} miles.");
    
}

class SportsCar : Car

{

    public override void Drive(int miles) => Console.WriteLine($"Driving {miles} miles with style!");
    
}

Access Modifiers

public: Accessible anywhere.

private: Accessible only within the class.

protected: Accessible in the class and derived classes.

internal: Accessible within the same assembly.

protected internal: Accessible within the same assembly or by derived classes.

    
