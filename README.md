using System;

delegate void Message();

class Demo
{
    public void Welcome()
    {
        Console.WriteLine("Welcome Students");
    }

    public void Learn()
    {
        Console.WriteLine("Learning C# delegate");
    }
}

class Program
{
    static void Main(string[] args)
    {
        Demo d = new Demo();

        Message msg = d.Welcome;
        msg += d.Learn;

        msg();

        Console.WriteLine("Vijaylaxmi Vishwakarma");
    }
}
