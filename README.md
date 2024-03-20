# IntroducciónACMasMas

**_Para comenzar..._**

## Qué es un lenguaje de programación en C++?

- **_C++ es un lenguaje compilado que fue desarrollado en 1980 por el ingeniero escandinavo Bjarne Stroustroup en los laboratorios At&T como una extensión orientada a objetos del lenguaje C._**

- **_También dicho lenguaje de programación mencionado anteriormente significaría incremento de C, aprovechando que dicho lenguaje tiene el operador ++ con ese nombre._**

- **_En ese sentido, desde el punto de vista de los lenguajes orientados a objetos, C++ es un lenguaje híbrido._**

  ![image](https://github.com/Autinfit/Introducci-nACMasMas/assets/155406623/1cdd1a57-ad29-421d-9232-d7fe17f0a79c)


- **_Posteriormente se añadieron facilidades de programación genérica, que se sumaron a los paradigmas de programación estructurada y programación orientada a objetos._**

- **_Por esto se suele decir que el C++ es un lenguaje de programación multiparadigma._**

- **_Actualmente existe un estándar, denominado ISO C++, al que se han adherido la mayoría de los fabricantes de compiladores más modernos._**

- **_Existen también algunos intérpretes, tales como ROOT._**

- **_El nombre "C++" fue propuesto por Rick Mascitti en el año 1983, cuando el lenguaje fue utilizado por primera vez fuera de un laboratorio científico._**

- **_Antes se había usado el nombre "C con clases"._**

- **_En C++, la expresión "C++" significa "incremento de C" y se refiere a que C++ es una extensión de C._**

![image](https://github.com/Autinfit/Introducci-nACMasMas/assets/155406623/7dde6dd7-cd13-406a-b09d-8d8e070e89c2)

## Características de C++

- **_Su sintaxis es heredada del lenguaje C._**

- **_Programa orientado a objetos (POO)._**

- **_Permite la agrupación de instrucciones._**

- **_Es portátil y tiene un gran número de compiladores en diferentes plataformas y sistemas operativos._**

- **_Permite la separación de un programa en módulos que admiten compilación independiente._**

- **_Es un lenguaje de alto nivel._**

## Ejemplos

**_A continuación se cita un programa de ejemplo Hola mundo escrito en C++:_**

```
#include <iostream>

Diapositiva 1: Título
Título: "Introducción a C++"
Diapositiva 2: ¿Qué es C++?
Título: "¿Qué es C++?"
Contenido:
C++ es un lenguaje de programación de alto nivel y general.
Desarrollado como una extensión del lenguaje C.
Ampliamente utilizado en desarrollo de software, sistemas operativos, videojuegos y más.
Diapositiva 3: Estructura Básica de C++
Título: "Estructura Básica de C++"
Contenido:
Encabezado:
cpp
Copy code
#include <iostream>
using namespace std;
Función Principal:
cpp
Copy code
int main() {
    // Código principal aquí
    return 0;
}
Diapositiva 4: ¿Cómo funciona el "if" en C++?
Título: "Estructuras Condicionales: if"
Contenido:
Sintaxis:
cpp
Copy code
if (condición) {
    // Código si la condición es verdadera
} else {
    // Código si la condición es falsa
}
Ejemplo:
cpp
Copy code
int edad = 18;
if (edad >= 18) {
    cout << "Eres mayor de edad." << endl;
} else {
    cout << "Eres menor de edad." << endl;
}
Diapositiva 5: Tipos de Variables en C++
Título: "Tipos de Variables en C++"
Contenido:
Enteros:
cpp
Copy code
int entero = 42;
Decimales:
cpp
Copy code
double decimal = 3.14;
Caracteres:
cpp
Copy code
char caracter = 'A';
Cadenas de Texto:
cpp
Copy code
string texto = "Hola, mundo!";
Diapositiva 6: Resumen
Título: "Resumen"
Contenido:
Revisamos la estructura básica de C++.
Exploramos la estructura condicional "if" con un ejemplo.
Conocimos diferentes tipos de variables en C++.
Diapositiva 7: Preguntas
Título: "¿Preguntas?"
Contenido:
Invita a la audiencia a hacer preguntas y proporciona tus detalles de contacto si es necesario.
```

### Breve explicación del código:

**_Al usar la directiva ```#include``` se le dice al compilador que busque e interprete todos los elementos definidos en el archivo que acompaña la directiva (en este caso, ```iostream```). Para evitar sobrescribir los elementos ya definidos al ponerles igual nombre, se crearon los espacios de nombres o ```namespace``` del singular en inglés. En este caso hay un espacio de nombres llamado ```std```, que es donde se incluyen las definiciones de todas las funciones y clases que conforman la biblioteca estándar de C++. Al incluir la sentencia ```using namespace std``` le estamos diciendo al compilador que usaremos el espacio de nombres ```std``` por lo que no tendremos que incluirlo cuando usemos elementos de este espacio de nombres, como pueden ser los objetos ```cout``` y ```cin```, que representan el flujo de salida estándar (típicamente la pantalla o una ventana de texto) y el flujo de entrada estándar (típicamente el teclado)._**

**_La definición de funciones es igual que en C, salvo por la característica de que si ```main``` no va a recoger argumentos, no tenemos por qué ponérselos, a diferencia de C, donde había que ponerlos explícitamente, aunque no se fueran a usar. Queda solo comentar que el símbolo ```<<``` se conoce como operador de inserción, y grosso modo está enviando a ```cout``` lo que queremos mostrar por pantalla para que lo pinte, en este caso la cadena ```"Hola mundo"```. El mismo operador << se puede usar varias veces en la misma sentencia, de forma que gracias a esta característica podremos concatenar el objeto endl al final, cuyo resultado será imprimir un retorno de línea._**

## Tipos de datos

**_C++ tiene los siguientes tipos fundamentales:_**

 - **_Caracteres: ```char``` (también es un entero),_** ```wchar_t```
 - **_Enteros:_** ```short```, ```int```, ```long```, ```long long```
 - **_Números en coma flotante:_** ```float```, ```double```, ```long double```
 - **_Booleanos:_** ```bool```
 - **_Vacío:_** ```void```

**_El modificador ```unsigned``` se puede aplicar a enteros para obtener números sin signo (por omisión los enteros contienen signo), con lo que se consigue un rango mayor de números naturales._**

## Tamaños asociados

- **_Según la máquina y el compilador que se utilice los tipos primitivos pueden ocupar un determinado tamaño en memoria. La siguiente lista ilustra el número de bits que ocupan los distintos tipos primitivos en la arquitectura x86._**

- **_Otras arquitecturas pueden requerir distintos tamaños de tipos de datos primitivos. C++ no dice nada acerca de cuál es el número de bits en un byte, ni del tamaño de estos tipos; más bien, ofrece solamente las siguientes "garantías de tipos":_**

   - **_De acuerdo al estándar C99, un tipo ```char``` debe ocupar exactamente un 'byte' compuesto de un mínimo de 8 'bits' independientemente de la arquitectura de la máquina._**
   - **_El tamaño reconocido de ```char``` es de 1. Es decir, ```sizeof(char)``` siempre devuelve 1._**
   - **_Un tipo ```short``` tiene al menos el mismo tamaño que un tipo ```char```._**
   - **_Un tipo ```long``` tiene al menos el doble tamaño en bytes que un tipo ```short```._**
   - **_Un tipo ```int``` tiene un tamaño entre el de ```short``` y el de long, ambos incluidos, preferentemente el tamaño de un apuntador de memoria de la máquina. Su valor máximo es 2147483647, usando 32 bits._**
