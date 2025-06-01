---
layout: post
title: "Cómo instalar SQL Server y SSMS paso a paso"
date: 2025-06-01
categories: [SQLServer, Instalación]
tags: [sql-server, ssms, tutorial, instalación]
author: JuanD
---

¡Hola, comunidad! 👋 Hoy quiero compartir un tema esencial para cualquiera que esté comenzando en el mundo del desarrollo backend o la administración de bases de datos: **la instalación de SQL Server y SQL Server Management Studio (SSMS)**.

Si estás aprendiendo .NET o simplemente quieres tener un entorno robusto para practicar tus consultas SQL, este tutorial es para ti.

---

## 🧩 ¿Qué es SQL Server y por qué instalarlo?

**SQL Server** es un sistema de gestión de bases de datos relacional desarrollado por Microsoft. Es ampliamente utilizado en entornos empresariales por su potencia, seguridad y excelente integración con el ecosistema .NET.

**SSMS (SQL Server Management Studio)** es la herramienta gráfica oficial para conectarte a tus bases de datos, ejecutando consultas, creando tablas, usuarios, respaldos, etc. Podríamos decir que es como el "IDE" de las bases de datos SQL Server.

---

## 🚀 Requisitos previos

Antes de comenzar, asegúrate de cumplir con lo siguiente:

- Un PC con Windows 10/11 (64 bits).
- Al menos 4 GB de RAM (recomendado 8 GB).
- Espacio en disco: mínimo 6 GB disponibles.
- Conexión a internet (para descargar los instaladores).

---

## 🛠️ Paso 1: Descargar el instalador de SQL Server

1. Visita la página oficial de descargas:  
   👉 [https://www.microsoft.com/en-us/sql-server/sql-server-downloads](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

2. Descarga la **edición Developer** (es gratuita y con todas las características para desarrollo).

![Descargar SQL Server Developer](../assets/img/sql-server-descarga-developer.png)

---

## 🧙 Paso 2: Ejecutar el instalador de SQL Server

1. Abre el archivo `.exe` descargado.
2. Selecciona la opción **Basic** (instalación rápida) o **Custom** para personalizar.

3. Acepta los términos de licencia y espera a que se descarguen e instalen los componentes.

![Instalación básica de SQL Server](../assets/img/sql-server-instalador-basico.png)

---

## 🧾 Paso 3: Configurar la instancia (si elegiste "Custom")

- Elige una instancia con nombre o deja `MSSQLSERVER` como predeterminado.
- Selecciona el modo de autenticación: **mixto (SQL y Windows)**.
- Crea una contraseña para el usuario `sa`.
- Añade tu usuario de Windows como administrador.

![Configuración de autenticación](../assets/img/sql-server-autenticacion.png)

---

## 🧪 Paso 4: Verificar la instalación

1. Abre "SQL Server Configuration Manager".
2. Revisa que el servicio `SQL Server (MSSQLSERVER)` esté en estado **Running**.

---

## 💻 Paso 5: Instalar SQL Server Management Studio (SSMS)

1. Descarga SSMS desde la página oficial:  
   👉 [https://aka.ms/ssmsfullsetup](https://aka.ms/ssmsfullsetup)

2. Ejecuta el instalador, acepta los términos y continúa con la instalación.

![Instalación de SSMS](../assets/img/ssms-instalacion.png)

---

## 🟢 Paso 6: Conectarte a tu base de datos con SSMS

1. Abre SSMS desde el menú inicio.
2. En "Server name", escribe: .\SQLEXPRESS3. 
3. Selecciona el tipo de autenticación adecuado (SQL o Windows).

![Conexión en SSMS](../assets/img/ssms-conexion.png)

---

## 🧪 Prueba de conexión

Abre una nueva consulta (`Ctrl + N`) y ejecuta el siguiente script:

```sql
SELECT @@VERSION;
```

Si ves la versión del motor en los resultados, ¡todo está funcionando!

---

## Conclusión
Tener SQL Server y SSMS bien instalados es el primer paso para trabajar profesionalmente con bases de datos. A partir de aquí puedes practicar tus scripts SQL, aprender procedimientos almacenados, funciones, índices, y todo lo que necesitas para dominar el backend con .NET y SQL Server.

---

¿Te fue útil esta guía? ¿Tuviste algún problema durante la instalación? Déjamelo en los comentarios del blog o contáctame en mis redes. ¡Nos leemos pronto!
