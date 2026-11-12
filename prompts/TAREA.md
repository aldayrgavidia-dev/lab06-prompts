
# Tarea: Mi prompt profesional

## Funcionalidad elegida

Elegí desarrollar un sistema de registro de productos para una tienda utilizando Java. El programa permitirá registrar productos y mostrar sus datos, como código, nombre, precio y stock.

## Version 1: prompt básico

**Prompt v1:**

```text
Crea un programa en Java para registrar productos de una tienda.
```

**Qué cambié:** En esta primera versión solamente indiqué la funcionalidad general.

**Por qué:** Quería observar qué respuesta generaba la IA con una instrucción sencilla.

**Qué mejoró en la respuesta:** La IA propuso una solución inicial, pero faltaban detalles sobre los atributos, la estructura y el funcionamiento del programa.

## Version 2: prompt mejorado

**Prompt v2:**

```text
Crea un programa en Java para registrar productos de una tienda.
Utiliza una clase Producto con los atributos codigo, nombre,
precio y stock. Incluye métodos para mostrar los datos
de cada producto.
```

**Qué cambié:** Agregué los atributos que debía tener la clase Producto y solicité un método para mostrar sus datos.

**Por qué:** La primera versión era demasiado general y dejaba muchas decisiones a la IA.

**Qué mejoró en la respuesta:** La IA presentó una estructura más organizada, con una clase Producto y los atributos solicitados.

## Version 3: prompt final

**Prompt v3:**

```text
ROL:
Actúa como un desarrollador Java especializado en
programación orientada a objetos.

INSTRUCCIÓN:
Crea un programa de consola para registrar y consultar
productos de una tienda.

CONTEXTO:
El programa será utilizado por un estudiante de primer ciclo
de Desarrollo de Software. Debe ser sencillo y utilizar
programación orientada a objetos. La clase Producto debe
contener los atributos codigo, nombre, precio y stock.

EJEMPLO:
Un producto registrado puede tener los siguientes datos:
codigo: P001
nombre: Teclado
precio: 85.50
stock: 10

FORMATO:
Presenta el código completo separado por clases.
Explica brevemente la función de cada clase y muestra
un ejemplo de ejecución en consola.

RESTRICCIÓN:
No utilices librerías externas ni bases de datos.
Utiliza únicamente Java y sus funcionalidades estándar.
```

**Qué cambié:** Incorporé los cinco componentes de un prompt: rol, instrucción, contexto, ejemplos y formato. También agregué una restricción.

**Por qué:** Necesitaba que la IA entendiera mejor el objetivo, las características del programa y la manera en que debía presentar la solución.

**Qué mejoró en la respuesta:** La respuesta fue más completa y organizada. La IA tuvo información suficiente para generar una solución relacionada con lo solicitado y respetar las condiciones indicadas.

## Componentes del prompt final

| Componente | Identificación en el prompt |
|---|---|
| Rol | Desarrollador Java especializado en POO. |
| Instrucción | Crear un programa para registrar y consultar productos. |
| Contexto | Programa para un estudiante de primer ciclo con una clase Producto. |
| Ejemplos | Producto P001, Teclado, 85.50 y stock 10. |
| Formato | Código separado por clases y ejemplo de ejecución. |

## Evaluación del resultado

| Criterio | Resultado |
|---|---|
| Utiliza Java | Sí |
| Incluye la clase Producto | Sí |
| Contiene los cuatro atributos solicitados | Sí |
| Presenta el código organizado por clases | Sí |
| Incluye un ejemplo de ejecución | Sí |
| Respeta la restricción de no utilizar librerías externas | Sí |

## Errores que evité

| Error frecuente | Cómo lo evité |
|---|---|
| Ser demasiado general | Agregué los atributos, las funciones y el objetivo específico del programa. |
| No indicar el formato | Solicité el código separado por clases, una explicación y un ejemplo de ejecución. |

