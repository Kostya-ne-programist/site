public class Animal
{
    public virtual void Speak() => Console.WriteLine("...");
}

public class Dog : Animal
{
    public override void Speak() => Console.WriteLine("Гав!");
}

public class Cat : Animal
{
    public override void Speak() => Console.WriteLine("Мяу!");
}

Animal dog = new Dog();
Animal cat = new Cat();

dog.Speak(); // Гав!
cat.Speak(); // Мяу!
