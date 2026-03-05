# frete-calculator-csharp
using System;

class Program
{
    static double CalcularFrete(double km, double valorKm)
    {
        return km * valorKm;
    }

    static void Main()
    {
        Console.Write("Digite a distância em KM: ");
        double km = Convert.ToDouble(Console.ReadLine());

        Console.Write("Digite o valor por KM: ");
        double valorKm = Convert.ToDouble(Console.ReadLine());

        double total = CalcularFrete(km, valorKm);

        Console.WriteLine($"Valor total do frete: R$ {total:F2}");
    }
}
