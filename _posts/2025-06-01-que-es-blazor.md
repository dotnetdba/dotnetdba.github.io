---
layout: post
title: "¿Qué es Blazor y cómo se relaciona con .NET?"
date: 2025-06-01
categories: [Blazor, .NET]
tags: [blazor, dotnet, web, csharp, frontend]
author: Juan De Dios
---

¡Hola! 👋 Hoy quiero hablarte de un tema que cada vez suena más fuerte entre los desarrolladores .NET: **Blazor**. Tal vez ya lo escuchaste nombrar, o incluso viste alguna demo en algún evento de Microsoft, pero no terminás de entender bien qué es o por qué deberías prestarle atención. Bueno, hoy lo aclaramos.

---

## ☁️ Entonces… ¿Qué es Blazor?

Blazor es un **framework de desarrollo web** creado por Microsoft que permite crear aplicaciones web interactivas **usando C# en lugar de JavaScript**.

Sí, leíste bien. Con Blazor podés escribir todo tu código del lado del cliente (lo que normalmente harías con JS, React, Angular, etc.) usando solamente C# y Razor. Es parte del ecosistema de **ASP.NET Core**, así que si ya estás familiarizado con .NET, te vas a sentir como en casa.

---

## 🧠 ¿De dónde viene el nombre “Blazor”?

El nombre viene de una combinación entre:

- **BLA** = Browser + Razor  
- **ZOR** = Sonaba bien… 😅

El punto es que une Razor (el motor de plantillas que usamos en ASP.NET) con la ejecución en el navegador, lo que lo convierte en una experiencia web muy completa sin salir de .NET.

---

## 🧩 ¿Cómo funciona Blazor?

Blazor tiene **dos modelos de ejecución principales**:

### 1. Blazor Server

- El código C# se ejecuta en el servidor.
- El navegador se comunica con el servidor a través de una conexión en tiempo real usando SignalR.
- Cada vez que interactuás con la app (un clic, un scroll, etc.), se envía un evento al servidor, se procesa y se actualiza la UI.

✅ Ventajas:
- El tamaño de descarga es muy bajo.
- Compatible con todos los navegadores modernos.

🚫 Desventajas:
- Depende 100% de la conexión con el servidor.
- Cada usuario consume recursos del servidor constantemente.

---

### 2. Blazor WebAssembly (Blazor WASM)

- El código C# se ejecuta directamente en el navegador gracias a **WebAssembly**.
- Se descarga un pequeño runtime de .NET junto con tu app.
- No necesita conexión permanente al servidor.

✅ Ventajas:
- Totalmente cliente, sin conexión en tiempo real.
- Ideal para aplicaciones PWA o que deben funcionar offline.

🚫 Desventajas:
- El tamaño inicial de descarga es mayor.
- Algunas limitaciones en el acceso a recursos del sistema.

---

## 🧵 ¿Cómo se relaciona con .NET?

Blazor **forma parte del ecosistema .NET** desde la versión .NET Core 3.0 y ha crecido muchísimo con .NET 5, 6, 7 y ahora .NET 8/9.

Podés usar:
- Las clases y librerías de .NET como en cualquier otra app.
- Inyección de dependencias.
- Entity Framework para conectarte a bases de datos.
- Integración con APIs REST, gRPC, servicios de Azure, etc.

En resumen: **Blazor no es algo aparte. Es parte de .NET**. Si ya sabés .NET, solo estás aprendiendo una nueva forma de presentar tus datos.

---

## ✨ ¿Por qué usar Blazor?

Depende de tus necesidades, pero algunas razones muy válidas son:

- Querés desarrollar con C# en el frontend sin tocar JavaScript.
- Tu equipo ya trabaja con .NET y no querés agregar otro stack.
- Necesitás compartir código entre el frontend y backend.
- Querés una app moderna pero no querés aprender un framework JS más.

---

## 🔥 ¿Y qué se puede hacer con Blazor?

¡Mucho! Algunas ideas:

- Dashboards empresariales.
- Aplicaciones internas para empresas.
- Páginas SPA modernas.
- Aplicaciones PWA que funcionan sin conexión.
- Prototipos rápidos si ya dominás C#.

Además, podés integrar componentes de librerías como Bootstrap, Material o incluso usar Blazor con MAUI para apps móviles.

---

## 🧪 ¿Y el rendimiento?

Blazor Server es súper rápido en apps con pocos usuarios concurrentes. Ideal para sistemas internos o administrativos.

Blazor WebAssembly ha mejorado muchísimo y hoy es perfectamente usable para apps públicas. Obviamente no va a tener el mismo rendimiento inicial que una app React optimizada, pero **la experiencia es más que aceptable** y sigue mejorando con cada versión de .NET.

---

## 🛠️ ¿Cómo empiezo?

Solo necesitás tener instalado:

- El SDK de .NET más reciente: [https://dotnet.microsoft.com/download](https://dotnet.microsoft.com/download)
- Visual Studio (versión Community o superior) o Visual Studio Code.
- Y ganas de probar algo nuevo. 😉

```bash
dotnet new blazorwasm -o MiPrimeraAppBlazor
cd MiPrimeraAppBlazor
dotnet run
```

¡Y ya tenés una app Blazor corriendo!

## Conclusión
Blazor es una propuesta muy interesante si venís del mundo .NET. Te permite crear aplicaciones web modernas sin tener que salir de tu stack de confianza. ¿Va a reemplazar a React o Angular? No necesariamente. Pero es una alternativa real, estable y muy bien integrada con el resto del ecosistema de Microsoft.

En lo personal, me parece una de las tecnologías más emocionantes que ha sacado Microsoft en los últimos años.

Nos leemos en el próximo post ✌️
