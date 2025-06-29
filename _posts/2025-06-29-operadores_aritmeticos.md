---
layout: post
title: "¿Cómo usar los operadores aritméticos en C#?"
date: 2025-06-23
author: Juan De Dios
categories: [CSharp, Fundamentos]
tags: [operadores, csharp, aritmetica, programacion-basica]
---

En programación, los operadores aritméticos son herramientas básicas que permiten **realizar cálculos matemáticos**. En C#, estos operadores se usan para sumar, restar, multiplicar, dividir y más.

Hoy te explico cómo usarlos con ejemplos simples para que puedas comenzar a aplicarlos en tus propios programas.



## ¿Qué son los operadores aritméticos?

Son símbolos que indican al programa que debe realizar una **operación matemática** entre dos valores (o variables). Por ejemplo:

```csharp
int resultado = 5 + 3;
```
Aquí, el + es un operador aritmético.



| Operador | Nombre           | Ejemplo  | Resultado |
| -------- | ---------------- | -------- | --------- |
| `+`      | Suma             | `5 + 3`  | `8`       |
| `-`      | Resta            | `10 - 4` | `6`       |
| `*`      | Multiplicación   | `7 * 2`  | `14`      |
| `/`      | División         | `20 / 5` | `4`       |
| `%`      | Módulo (residuo) | `10 % 3` | `1`       |



## Ejemplos en código
```csharp
using System;

class Program
{
    static void Main()
    {
        int a = 10;
        int b = 3;

        Console.WriteLine("Suma: " + (a + b));         // 13
        Console.WriteLine("Resta: " + (a - b));        // 7
        Console.WriteLine("Multiplicación: " + (a * b)); // 30
        Console.WriteLine("División: " + (a / b));     // 3
        Console.WriteLine("Módulo: " + (a % b));       // 1
    }
}
```

## Consideraciones importantes
División entre enteros
En C#, si divides dos números enteros (int), el resultado también será entero (descarta los decimales).
```csharp
int resultado = 7 / 2;
Console.WriteLine(resultado); // 3, no 3.5
```

Si querés obtener un decimal, usá double:
```csharp
double resultado = 7.0 / 2;
Console.WriteLine(resultado); // 3.5
```

## Precaución con el módulo
El operador % devuelve el resto de una división. Es útil, por ejemplo, para saber si un número es par:
```csharp
if (numero % 2 == 0)
{
    Console.WriteLine("El número es par");
}
```

## Conclusión
Los operadores aritméticos son fundamentales en cualquier lenguaje de programación, y en C# se usan de manera muy intuitiva. Dominarlos te va a permitir resolver cálculos, crear validaciones y desarrollar lógica cada vez más útil y potente.


¡Nos leemos pronto!
