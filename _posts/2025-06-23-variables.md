---
layout: default
title: "¿Qué son y cómo usar las variables en C#?"
date: 2025-06-23
author: Juan De Dios
categories: [CSharp, Fundamentos]
tags: [variables, csharp, programacion-basica]
---

Cuando comenzás a programar en C#, uno de los primeros conceptos que vas a encontrar son las **variables**. Y aunque suenen simples, entender bien cómo funcionan es clave para avanzar con seguridad en el resto del lenguaje.

---

## 🧠 ¿Qué es una variable?

Una **variable** es un espacio en la memoria donde podés guardar datos que pueden cambiar mientras el programa se ejecuta. Por eso se llama *variable*: porque su valor puede variar.

En C#, toda variable necesita tener un **tipo de dato**, un **nombre** y, opcionalmente, un **valor inicial**.

Ejemplo básico:

```csharp
int edad = 30;

Esto significa: "Reservá un espacio en memoria llamado edad que va a guardar un número entero, y su valor inicial es 30."

Tipos de variables comunes
En C# existen muchos tipos de datos, pero los más usados cuando estás empezando son:

| Tipo     | Descripción                  | Ejemplo                  |
| -------- | ---------------------------- | ------------------------ |
| `int`    | Número entero                | `int cantidad = 5;`      |
| `double` | Número decimal               | `double precio = 10.5;`  |
| `char`   | Un solo carácter             | `char letra = 'A';`      |
| `string` | Texto o cadena de caracteres | `string nombre = "Ana";` |
| `bool`   | Verdadero o falso            | `bool esMayor = true;`   |

Reglas para nombrar variables
En C# podés nombrar tus variables como quieras, pero seguí estas buenas prácticas:

Usá nombres descriptivos: nombre, totalCompra, esActivo.

Comenzá con una letra (no con números o símbolos).

Evitá usar nombres reservados del lenguaje como int, class, if, etc.

Se recomienda usar camelCase: la primera palabra en minúscula y las siguientes con mayúscula.

Ejemplo:
```csharp
int edadUsuario = 25;
string mensajeBienvenida = "Hola, bienvenido!";

Declarar y usar variables
Podés declarar una variable y asignarle un valor más adelante:
```csharp
int cantidad;
cantidad = 10;


O hacer todo en una sola línea:
```csharp
int cantidad = 10;


Y luego usarla:
```csharp
Console.WriteLine("La cantidad es: " + cantidad);


¿Qué pasa si uso una variable sin inicializarla?
C# no te deja usar variables sin asignarles un valor primero. Te va a lanzar un error de compilación. Por ejemplo, esto no funciona:
```csharp
int x;
Console.WriteLine(x); // ❌ Error: variable no asignada

Siempre asegurate de inicializar tus variables antes de usarlas.

¿Qué es var en C#?
var es una forma implícita de declarar variables. El compilador deduce el tipo a partir del valor asignado.
```cshar
var nombre = "Juan"; // El compilador entiende que es string
var edad = 28;         // El compilador entiende que es int

⚠️ Consejo: usá var solo cuando el tipo sea claro. No lo uses si va a generar confusión.


Ejemplo completo
```csha
using System;

class Program
{
    static void Main()
    {
        string nombre = "Lucía";
        int edad = 24;
        bool esMayor = edad >= 18;

        Console.WriteLine("Nombre: " + nombre);
        Console.WriteLine("Edad: " + edad);
        Console.WriteLine("¿Es mayor de edad?: " + esMayor);
    }
}


Conclusión
Las variables son la base de cualquier programa. Son como pequeñas cajas donde guardás información que después usás para tomar decisiones, mostrar resultados o hacer cálculos.

Conocer bien cómo declarar, asignar y usar variables en C# te va a ayudar a entender todo lo que viene después: condicionales, bucles, funciones y clases.