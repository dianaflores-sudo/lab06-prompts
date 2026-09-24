# Tarea: Mi prompt profesional
 
## Funcionalidad elegida
 Sistema de Gestion de Estudiante.

## Version 1: prompt basico
```text
Hazme un programa para registrar estudiantes.
```
Qué cambió / Por qué / Mejora: Es la primera interacción. Resulta muy general, genera un código simple con una estructura de datos incompleta.

## Version 2
```text
 Actua como desarrollador Java. Crea un programa con interfaz grafica Swing para registrar estudiantes con nombre, carrera y edad.
```
-Qué cambió: Se agregó un Rol y un Contexto técnico (uso de Java Swing y campos específicos).

-Mejora: La respuesta ahora entrega una interfaz funcional básica, aunque el código está en una sola clase mixta y carece de validaciones.

## Version 3: prompt final
```text
Actua como desarrollador senior Java. Crea una aplicacion de escritorio en Java Swing para registrar estudiantes. 

El sistema debe solicitar: Nombre completo, Carrera y Edad.

Ejemplo de formato de metodos en el modelo:
getNombre(), setNombre(String nombre)

Presenta el resultado estructurado en arquitectura MVC (Modelo, Vista, Controlador). Explica brevemente la estructura antes del codigo.

Restricciones: No uses librerias externas. Valida que el nombre no este vacio y que la edad sea un numero mayor a 17. Muestra las alertas con JOptionPane.
 ```

-Qué cambió: Se incluyeron Ejemplos de formato, organización clara (MVC), explicación previa y Restricciones explícitas (sin librerías externas y validaciones con JOptionPane).

-Mejora: Se obtiene un código limpio, mantenible, seguro con validaciones y profesionalmente estructurado.

## Componentes del prompt final
 | Componente | Texto de mi prompt |
|------------|--------------------|
| Rol |Actua como desarrollador senior Java.|
| Instruccion |Crea una aplicacion de escritorio en Java Swing para registrar estudiantes... Restricciones: No uses librerias externas. Valida que el nombre no este vacio y que la edad sea un numero mayor a 17. Muestra las alertas con JOptionPane.|
| Contexto |El sistema debe solicitar: Nombre completo, Carrera y Edad.|
| Ejemplo |Ejemplo de formato de metodos en el modelo: getNombre(), setNombre(String nombre)|
| Formato |Presenta el resultado estructurado en arquitectura MVC (Modelo, Vista, Controlador). Explica brevemente la estructura antes del codigo.|

```text
Restricciones: No uses librerias externas. Valida que el nombre no este vacio y que la edad sea un numero mayor a 17. 
```

## Evaluacion del resultado
  | Criterio | Cumple (Sí / No) |
|----------|-------------|
| Usa Java Swing sin librerías externas |Si|
| Aplica arquitectura MVC |SI|
| Valida correctamente edad y nombre |Si|
| Despliega mensajes con JOptionPane |Si|



## Errores que evite
```text
-Ser demasiado general: En la V1 el prompt no especificaba la tecnología ni la estructura. Lo evité definiendo claramente Java Swing, campos necesarios y arquitectura MVC en la V3.

-No indicar restricciones ni formato: Inicialmente no se acotaban las validaciones. Lo evité agregando reglas estrictas (edad > 17, no campos vacíos) e indicando el uso exclusivo de JOptionPane y la explicación previa al código.
```