# Bitacora de prompts

Laboratorio 06: Fundamentos de Ingenieria de Prompts.

Herramienta de IA usada: ChatGPT

## Ejercicio 2: Tokens y ventana de contexto
| Texto | Caracteres | Tokens |
|-------|------------|--------|
| Los estudiantes programan en Java. | 34 | 7 |
| The students program in Java. | 30 | 6 |
| desafortunadamente | 18 | 4 |

En el mismo chat, ChatGPT recordó correctamente que mi aplicación se llama TiendaTec y utiliza Java Swing.

En el chat nuevo, también respondió correctamente. Esto ocurrio porque la función de memoria de ChatGPT está activada.

## Ejercicio 3: Temperatura
| Prueba | Nombres generados |
|--------|-------------------|
| 1 | BiblioUni, UniBook, BookCampus |
| 2 | BiblioTec, UniBook, BookCampus |
| 3 | BiblioTec, UniLibro, BookCampus |
### Resultados del simulador Java

| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|-------------|----------------|---------------------------|
| 0 | 100.0% | BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec |
| 0.5 | 65.3% | BiblioTec, BiblioTec, BiblioTec, LibroYa, LibroYa |
| 1.0 | 44.5% | LibroYa, BiblioTec, BiblioTec, PaginaLibre, PrestaLibro |
| 1.8 | 32.2% | LibroYa, PrestaLibro, NubeDeTinta, BiblioTec, PrestaLibro |

### Segunda prueba con temperatura 1.8

Los cinco intentos fueron: PaginaLibre, BiblioTec, BiblioTec, BiblioTec y LectoGo.

### Observacion

Al aumentar la temperatura, la probabilidad se distribuye entre más opciones y aumenta la variedad de nombres generados. Con temperatura 0, siempre se selecciona la opción con mayor puntaje.

El simulador solo puede elegir entre los nombres definidos en el arreglo opciones, por lo que no puede generar nombres nuevos.

- **Nivel 4:** La IA incorporó la clase Producto con los cuatro atributos solicitados (codigo, nombre, precio y stock) y utilizó encapsulamiento mediante atributos privados y métodos getters.

## Ejercicio 4: Prompt vago vs estructurado

### Prompt vago

Hazme una aplicación de biblioteca.

**Resultado:**

ChatGPT propuso funcionalidades generales como registrar libros, estudiantes, préstamos y devoluciones. También preguntó qué tecnología quería utilizar.

### Prompt estructurado

Actua como analista de sistemas. Redacta una descripcion breve de un sistema web para gestionar prestamos de libros en una biblioteca. Incluye objetivo, usuarios principales y 3 funcionalidades clave. Utiliza un lenguaje claro y profesional y presenta el resultado en 3 parrafos.

**Resultado:**

El sistema web para gestionar préstamos de libros en una biblioteca tiene como objetivo facilitar y optimizar el control de los libros disponibles, los préstamos y las devoluciones. Su propósito es agilizar los procesos de atención, reducir los errores en los registros y mantener la información organizada y actualizada.

Los principales usuarios del sistema son los bibliotecarios, encargados de administrar los libros y controlar los préstamos, y los estudiantes o lectores, quienes podrán consultar el catálogo y solicitar préstamos de libros. Cada usuario tendrá acceso a las opciones correspondientes según su función dentro de la biblioteca.

El sistema contará con tres funcionalidades clave: gestión de libros, que permitirá registrar, modificar y consultar los libros disponibles; gestión de préstamos y devoluciones, que facilitará el registro y seguimiento de los libros prestados y sus fechas de devolución; y consulta del catálogo, que permitirá a los usuarios buscar libros por título, autor o categoría y conocer su disponibilidad.

### Comparación

| Criterio | Prompt vago | Prompt estructurado |
|----------|-------------|---------------------|
| Menciona el objetivo del sistema | No | Sí |
| Menciona a los usuarios principales | No | Sí |
| Tiene exactamente 3 funcionalidades | Sí | Sí |
| Está en 3 párrafos | No | Sí |
| Lo usaría en un informe real | No | Sí |


## Ejercicio 5: Anatomia de un prompt