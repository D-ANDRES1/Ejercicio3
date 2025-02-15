# Ejercicio3
using System.Xml;

int resultado = 0;
void saludar()
{
    Console.WriteLine("que onda");
}


int suma (int n1, int m2)
{
  
    resultado = n1 + m2;
    return resultado;
}

int multiplicacion (int n1, int m2)
{
    
    resultado = n1 * m2;
    return resultado;
}
int resta(int n1, int m2)
{
    
    resultado = n1 - m2;
    return resultado;
}
int division(int n1, int m2)
{
    
    resultado = n1 / m2;
    return resultado;
}


saludar();

Console.WriteLine("ingrese un numero");
int num1 = int.Parse(Console.ReadLine());

Console.WriteLine("ingrese el segundo numero");
int num2 = int.Parse(Console.ReadLine());


Console.WriteLine("**Que quieres hacer con los dos numeros**");
Console.WriteLine("eligie una opcion");
Console.WriteLine("1. sumar");
Console.WriteLine("2. restar");
Console.WriteLine("3. multiplicar");
Console.WriteLine("4. division");

int opcion;
 opcion = int.Parse(Console.ReadLine());

switch (opcion)
{
    case 1:
        
        Console.WriteLine($"la suma es: {suma(num1, num2)}");
        break;
    case 2:
        Console.WriteLine($"la resta es: {resta(num1, num2)}");
        break;
       case 3:
        Console.WriteLine($"la multiplicacion es: {multiplicacion(num1, num2)}");
        break;
       case 4:
        Console.WriteLine($"la division es: {division(num1, num2)}");
        break;
        default: Console.WriteLine("opcion invalida");
        break;
}
