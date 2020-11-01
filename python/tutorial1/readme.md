# Tutorial 1 de python
## Prerrequisitos
- [Instalar python](https://www.python.org/downloads/)
- Instalar un entorno de desarrollo o IDE: [Pycharm community](www.jetbrains.com/pycharm/download)
- Si no se lo ha hecho antes, realizar un tutorial básico general de python para entender bucles, condicionales, listas, diccionarios

## Ejercicio
- El teatro Sucre está vendiendo espectáculos teatrales a clientes corporativos. Un cliente típico comprará unas cuantas obras y Teatro Sucre le cobrará sobre la base del tamaño de la audiencia y del tipo de obra ejecutada.  
- Actualmente existen dos tipos de obras: tragedias y comedias

### Las obras se cobran de la siguiente forma
  - Tragedias
    - $ 40.000
    - Si la audiencia supera las 30 personas, se cobra 1.000 por cada persona adicional
  - Comedias
    - $ 30.000 + 300 por cada asistente 
    - Si la audiencia supera las 20 personas, se cobra un fee de $10.000 + 500 por cada persona adicional

Los puntos de lealtad se otorgan por cada obra contratada, sobre la base de la cantidad de púbico de la siguiente forma:
- Un punto de lealtad por cada asistente, siempre y cuando hayan 30 o más asistentes.
- Las comedias generan un punto adicional por cada 10 asistentes

- El sistema debe proveer una factura por las obras contratadas, y además otorgar "puntos de descuento" para próximas obras como mecanismo para asegurar la  lealtad de los clientes 


### Historia de usuario
Como usuario quiero que el sistema me muestre la factura de un cliente, con el precio desglosado de cada obra y al final el monto total y los puntos otorgados. 

### Consejos
- No calcular el IVA y no realizar ningún tipo de interfaz de usuario ni conexión a base de datos
- Los datos de las obras vienen en un diccionario como el siguiente:
{
  "hamlet": {"nombre": "Hamlet", "tipo": "tragedia"},
  "lear": {"nombre": "El Rey Lear", "tipo": "comedia"},
  "othello": {"nombre": "Otelo", "type": "tragedia"}
}
- Los datos de las ventas vienen en una lista anidada de diccionarios como la siguiente:
[
  {"cliente": "La Favorita",
    "espectaculos": [
      {
        "id": "hamlet",
        "audiencia": 55
      },
      {
        "id": "lear",
        "audiencia": 35
      },
      {
        "id": "otelo",
        "audiencia": 40
      }
    ]
  },
  {"cliente": "Ministerio de Cultura",
    "espectaculos": [
    {
        "id": "hamlet",
        "audiencia": 24
      },
      {
        "id": "lear",
        "audiencia": 24
      },
    ]
  }
]

## Pasos
- Intentar programar el script en Python
- Anotar los conceptos sobre los que no se tiene dominio
- Revisar cómo se implementó el mismo programa en Javascript en la página 7 del libro Refactoring: Improving the design of existing code (Fowler)
- "Traducir" la solución del libro de Martin Fowler a Python
## Reflexionar
- Una vez terminado el programa, ¿se lo puede mejorar?
- ¿Qué es refactoring?
- Revisar capítulo 2 del libro Refactoring: Defining refactoring, The two hats, Why should we refactor
- Revisar el video de Robert Martin sobre código limpio:
https://www.youtube.com/watch?v=7EmboKQH8lM
12:21     The current Society works with Software
19:47     Volkswagen case / Introduction to the Ethics of Software Development
24:28     Why are Programmers so slow?
32:13     What is a Clean Code?
40:09     Analyzing some lines of code
43:43     Long code is not Good Code
49:25     Good Code / Refactored Function
52:40     Polite Code / Rules for writing a news paper article
55:25     Shrunk Code / The Rules of Functions
