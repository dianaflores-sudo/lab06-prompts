# Bitacora de prompts
 
Laboratorio 06: Fundamentos de Ingenieria de Prompts.
 
Herramienta de IA usada: (Gemini)
 
## Ejercicio 2: Tokens y ventana de contexto
 | Texto | Caracteres | Tokens |
|-------|------------|--------|
| Los estudiantes programan en Java. |7|34|
| The students program in Java. |29|6|
| desafortunadamente |4|18|

Paso 4: Si llego a contestar bien 

Paso 5: Respondio bien ya que guarda los datos anteriores 

## Ejercicio 3: Temperatura
| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|-------------|----------------|---------------------------|
| 0 |100%|BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec|
| 0.5 |65.3%|BiblioTec, BiblioTec, BiblioTec, LibroYa, BiblioTec|
| 1 |44.5%|NubeDeTinta, LibroYa, LibroYa, NubeDeTinta, BiblioTec|
| 1.8 |32.2%|BiblioTec, PrestaLibro, LibroYa, LectoGo, LibroYa|

 
## Ejercicio 4: Prompt vago vs estructurado
 | Criterio | Prompt vago | Prompt estructurado |
|----------|-------------|---------------------|
| Menciona el objetivo del sistema |No|Si|
| Menciona a los usuarios principales |No|Si|
| Tiene exactamente 3 funcionalidades |No|Si|
| Esta en 3 parrafos |No|Si|
| Lo usaria en un informe real |No|Si|

## Ejercicio 5: Anatomia de un prompt
| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol |Crea un programa en Java.|
| Instruccion |Actua como desarrollador Java. Crea un programa en Java.|
| Contexto |Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda.|
| Ejemplo |Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda usando una clase Producto con los atributos codigo, nombre, precio y stock.|
| Formato |Actua como desarrollador Java. Crea un programa en Java para gestionar los productos de una tienda usando una clase Producto con los atributos codigo, nombre, precio y stock. Explica primero la estructura de la clase y luego presenta el codigo Java|

Nivel 1: Al no contar con pautas ni un trasfondo definido, la IA seleccionó de manera autónoma un tema cualquiera y generó la función principal (main).

Nivel 2 (+Rol): Al adoptar la postura de un programador experto en Java, elevó el nivel técnico del programa implementando estructuras de datos dinámicas (ArrayList), modularizando la lógica en métodos específicos y ofreciendo un desglose descriptivo sobre el funcionamiento de bloques clave del código.

Nivel 3 (+Contexto): Al incorporar el entorno de aplicación ("un sistema para el control de inventario en un comercio"), orientó todo el diseño hacia la gestión comercial, estructurando una clase base para los artículos junto con la lógica de negocio asociada, detallando además el propósito de cada entidad del sistema.

Nivel 4 (+Instrucción): Al incluir requerimientos precisos para la clase Producto, sustituyó las propiedades genéricas del nivel previo por atributos bien definidos, implementó su método constructor y añadió los correspondientes métodos de acceso (getters).

Nivel 5 (+Formato +Ejemplo): Al estructurar la presentación de la respuesta ("comienza describiendo las variables privadas") e incluir una síntesis conceptual al cierre detallando las responsabilidades de cada componente.
 
## Ejercicio 6: Del prompt basico al profesional
| Qué revisar | Cumple (Sí / No) |
|------------|--------------------|
| ¿Está escrito en Java y usa Swing? |Si|
| ¿Pide correo y contraseña? |Si|
| ¿Explica el funcionamiento antes o después del código? |Si|
| ¿El código está organizado en clases? |Si|
| ¿Valida los datos que ingresa el usuario? |Si|

```text
(Prompt inicial:
Actua como desarrollador Java. Crea un ejemplo de login para una aplicacion de escritorio utilizando Swing. El usuario debe ingresar correo y contrasena. Explica brevemente el funcionamiento y presenta el codigo organizado por clases.

Prompt de mejora:
Mejora el codigo anterior con estas restricciones: no uses librerias externas, valida que el correo contenga @ y que la contrasena tenga al menos 8 caracteres, y muestra los mensajes con JOptionPane.)
```

