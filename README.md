# RandomGame
Random x = new Random();

int pn = x.Next(0, 51);

int hn = 0;
int count = 0;

Console.WriteLine("Программой загадано число от 0 до 50.");
Console.WriteLine("Угадайте это число. Количество попыток не ограничено");

while (hn != pn)
{
    hn = Convert.ToInt32(Console.ReadLine());

    {
        Console.WriteLine("Вы не угадали число.");
    }
    count++;
    if (hn == pn)
    {
        Console.WriteLine("Поздравляем, Вы угадали число с попытки № " + count + ":");
    }
}
