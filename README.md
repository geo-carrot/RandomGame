# RandomGame
Random x = new Random(); 

int pn = x.Next(0, 51);

    int hn = 0;
    int count = 0;

Console.WriteLine("Программой загадано число от 0 до 50.");
Console.WriteLine("Угадайте это число. Количество попыток - 10");

int i = Convert.ToInt32(Console.ReadLine());

while (count <= 10)
{
    if (hn == pn)
    {
        Console.WriteLine("Поздравляем, Вы угадали число!");
        break;
    }
    else
    {
        count++;
        if (count == 11)
        {
            Console.WriteLine("Вы не угадали число.");
            break;
        }
        Console.WriteLine("Вы не угадали число. Попытка № " + count + ":");
        hn = Convert.ToInt32(Console.ReadLine());
    }
}
Console.ReadLine();
