# Caso-Final-Integrador-Tema-4

https://github.com/24MICAELA/Caso-Final-Integrador-Tema-4.git

## Enunciado del Proyecto

Para este proyecto, se te pide que implementes un intérprete "tiny-lisp" basado en la clase Variant y las capacidades de la Standard Template Library (STL) de C++. Deberás trabajar en CLion para este proyecto.

## Requisitos del proyecto

Definir e implementar una clase Variant. Esta clase deberá ser capaz de representar diferentes tipos de datos, incluyendo símbolos, números, listas y procedimientos.

- Implementar un método to_string() para la clase Variant que convierta una instancia de la clase a una cadena de texto.
- Implementar un método to_json_string() para la clase Variant que convierta una instancia de la clase a una representación en formato JSON.
- Implementar un método estático from_json_string() que tome una cadena en formato JSON y la convierta a una instancia de la clase Variant.
- Implementar un método parse_json() que tome una cadena en formato JSON y la convierta a una instancia de la clase Variant.

## Resolución

## Clase Variant

La clase Variant representa distintos tipos de datos en un intérprete "tiny-lisp". Soporta:

Símbolos: Identificadores (variables, funciones).
Números: Valores numéricos.
Listas: Colecciones de Variant.
Funciones: Funciones ejecutables.
Lambdas: Funciones anónimas.
Cadenas: Texto entre comillas.

## Métodos clave

Constructor: Inicializa el tipo de dato (type), y los punteros env y proc a nullptr.

to_string(): Convierte el objeto en una cadena, adaptándose al tipo (símbolo, número, lista, etc.).

to_json_string(): Convierte el objeto en una cadena JSON usando la biblioteca json11.

from_json_string(): Convierte una cadena JSON a un objeto Variant.

parse_json(): Método auxiliar para convertir un objeto JSON en un Variant recursivamente.

## Pruebas

Las pruebas verifican el correcto funcionamiento de los métodos, asegurando que la clase maneje correctamente las conversiones entre tipos y formatos:

to_string(): Verifica la conversión a cadena de distintos tipos (Number, Cadena, List).
to_json_string(): Testea la conversión a JSON.
from_json_string(): Asegura que un JSON válido se convierta correctamente a un Variant.
parse_json(): Valida la conversión recursiva de estructuras JSON complejas.

