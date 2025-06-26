---
layout: post
title: "¿Qué son las constantes en C#?"
date: 2025-06-23
author: Juan De Dios
categories: [CSharp, Fundamentos]
tags: [constantes, csharp, programacion-basica]
---

En programación, hay momentos donde necesitás guardar valores que **no deben cambiar nunca** durante la ejecución del programa. En C#, para eso usamos las **constantes**.

Hoy vamos a ver qué son, cómo se declaran y por qué son tan útiles cuando querés que tu código sea claro y confiable.



## ¿Qué es una constante?

Una **constante** es como una variable… pero que **no puede cambiar su valor** una vez que ha sido definida.

En otras palabras, si algo debe mantenerse igual durante toda la ejecución de tu programa (como el número pi, el IVA o una URL base), **usá una constante en vez de una variable**.



## ¿Cómo se declara una constante en C#?

La sintaxis es muy simple. Usás la palabra clave `const`, seguida del tipo, el nombre y el valor:

```csharp
const tipo nombre = valor;
```

Ejemplo:
```csharp
const double Pi = 3.14159;
const int EdadMinima = 18;
const string Mensaje = "Bienvenido al sistema";
```
**Importante**: El valor de una constante debe ser conocido en tiempo de compilación. No podés usar expresiones que se calculen en tiempo de ejecución.


## ¿Cuándo usar constantes?
Usá constantes cuando:

- El valor no cambiará nunca (como el número de días en una semana).

- Querés evitar repetir valores “mágicos” en el código (por ejemplo: 60, 3.14, "admin").

- Necesitás mejorar la legibilidad del código.


Mirá este ejemplo mal hecho:
```csharp
if (edad >= 18)
{
    Console.WriteLine("Es mayor de edad");
}
```

Y ahora, mejor con constante:
```csharp
const int EdadMinima = 18;

if (edad >= EdadMinima)
{
    Console.WriteLine("Es mayor de edad");
}
```

## Conclusión
Las constantes son una herramienta simple pero poderosa. Te ayudan a:

- Escribir código más claro y entendible.

- Evitar errores por valores mal escritos o cambiados por accidente.

- Centralizar valores fijos en un solo lugar.

Usalas siempre que puedas. Tu yo del futuro (y otros programadores) te lo van a agradecer.
