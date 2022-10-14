Сначало объявляется два массива одной длины: Потом метод, в котором цикл соразмерный длине массива, внутри цикла проверка условия ( <=3 ), если да, элемент первого массива заносится в count элемент второго массива. Переменная count чтобы поочередно закидывать из первого массива во второй и чтобы потом не было пробелов. После присвоения увеличивается переменная count на 1 и возвращается к циклу for в котором i увеличивается на 1. И так проверяется до конца.

```
string[] array1 = new string[4] {"hello", "2", "world", ":-)"};
string[] array2 = new string[array1.Length];
int count = 0;

for (int i = 0; i < array1.Length; i++)
{
if(array1[i].Length <= 3)
    {
    array2[count] = array1[i];
    count++;
    }
}

void PrintArray(string[] array)
{
    for (int i = 0; i < array.Length; i++)
    {
        Console.Write($"{array[i]} ");
    }
    Console.WriteLine();
}

 PrintArray(array2);
 ```