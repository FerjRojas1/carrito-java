# 🛒 Carrito de Compras — Java MVC

Aplicación web dinámica desarrollada como trabajo práctico grupal para la **Universidad Nacional de Lomas de Zamora — Facultad de Ingeniería**.

El proyecto implementa un sistema de carrito de compras utilizando **Java, Servlets y JSP**, siguiendo el patrón arquitectónico **MVC (Modelo-Vista-Controlador)** y utilizando sesiones HTTP para la gestión del estado de la aplicación.

---

## 🎯 Descripción

**Carrito de Compras** es una aplicación web desarrollada en Java que permite simular un proceso de compra mediante:

* Autenticación de usuarios.
* Gestión de usuarios mediante roles.
* Visualización y gestión de productos.
* Agregado de productos al carrito.
* Modificación de cantidades.
* Eliminación de productos.
* Cálculo automático del total de la compra.
* Simulación del proceso de checkout.
* Gestión del estado mediante sesiones HTTP.

La aplicación utiliza el patrón **MVC** para separar la lógica de negocio, el acceso a los datos y la presentación.

Los datos del carrito se mantienen durante la sesión HTTP, por lo que **no requiere una base de datos para su ejecución**.

---

## 🔐 Autenticación y roles

El sistema cuenta con autenticación de usuarios y dos roles:

### 👨‍💼 Empleado

El usuario con rol **Empleado** tiene acceso a las funcionalidades relacionadas con la gestión de productos.

**Credenciales de prueba:**

```text
Usuario: Carlos
Contraseña: 1234
Rol: Empleado
```

### 🛒 Cliente

El usuario con rol **Cliente** puede acceder al carrito y realizar el flujo de compra.

**Credenciales de prueba:**

```text
Usuario: Manuel
Contraseña: 1234
Rol: Cliente
```

> Estas credenciales se encuentran incluidas en la aplicación con fines demostrativos y permiten probar los diferentes flujos según el rol del usuario.

---

## 🏗️ Arquitectura

El proyecto está organizado siguiendo el patrón **Modelo-Vista-Controlador (MVC)**:

```text
Controller
    ↓
Repository
    ↓
Model
    ↓
View (JSP)
```

El proyecto también implementa conceptos y patrones como:

* Patrón **MVC**
* Patrón **Singleton**
* Patrón **Repository**
* Autenticación y autorización basada en roles
* Gestión de sesiones HTTP
* Separación de responsabilidades
* Servlets y JSP

---

## ⚙️ Tecnologías

| Tecnología          | Uso                       |
| ------------------- | ------------------------- |
| **Java 17**         | Lenguaje principal        |
| **Servlets & JSP**  | Desarrollo web            |
| **Apache Tomcat 9** | Servidor de aplicaciones  |
| **HTML5**           | Estructura de la interfaz |
| **CSS3**            | Estilos                   |
| **JavaScript**      | Interactividad            |
| **Eclipse IDE**     | Entorno de desarrollo     |
| **Git & GitHub**    | Control de versiones      |

---

## 🚀 Cómo ejecutar el proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/FerJRojas1/carrito-java.git
cd carrito-java
```

### 2. Importar el proyecto en Eclipse

Importar el proyecto en **Eclipse IDE** y configurarlo como aplicación web Java.

Verificar que el proyecto utilice:

* Java 17
* Apache Tomcat 9
* Servlet API compatible con `javax.servlet`

### 3. Configurar Apache Tomcat

Agregar **Tomcat 9** como servidor dentro de Eclipse y asociar el proyecto al servidor.

Luego ejecutar:

```text
Run on Server
```

### 4. Acceder a la aplicación

Una vez iniciado Tomcat, acceder desde el navegador:

```text
http://localhost:8080/carrito-java/
```

---

## 🧪 Usuarios de prueba

Para probar los diferentes flujos de la aplicación se pueden utilizar las siguientes credenciales:

| Rol            | Usuario  | Contraseña |
| -------------- | -------- | ---------- |
| 👨‍💼 Empleado | `Carlos` | `1234`     |
| 🛒 Cliente     | `Manuel` | `1234`     |

Se recomienda probar ambos perfiles para visualizar las funcionalidades disponibles según cada rol.

---

## 💾 Persistencia de datos

La aplicación **no requiere una base de datos**.

El estado del carrito se administra mediante **sesiones HTTP**, por lo que los datos permanecen disponibles mientras la sesión del usuario se encuentre activa.

> Al reiniciar el servidor o finalizar la sesión, los datos almacenados en memoria se pierden.

---

## 👥 Integrantes

* Christian Fidelio
* Tadeo Bodetto
* Fernando Rojas

---

## 🎓 Contexto académico

Proyecto desarrollado como **trabajo práctico grupal** para la **Universidad Nacional de Lomas de Zamora — Facultad de Ingeniería**, con el objetivo de aplicar conceptos de desarrollo web utilizando Java, arquitectura MVC, Servlets, JSP, autenticación, manejo de roles y gestión de sesiones HTTP.
