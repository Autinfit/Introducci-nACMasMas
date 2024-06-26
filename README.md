# IntroducciónACMasMas

**_Para comenzar..._**

## Qué es un lenguaje de programación en C++?

- **_C++ es un lenguaje de alto nivel compilado que fue desarrollado en 1980 por el ingeniero escandinavo Bjarne Stroustroup en los laboratorios At&T como una extensión orientada a objetos del lenguaje C._**

- **_También dicho lenguaje de programación mencionado anteriormente significaría incremento de C, aprovechando que dicho lenguaje tiene el operador ++ con ese  mismo nombre._**

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
   - **_Un tipo ```int``` tiene un tamaño entre el de ```short``` y el de ```long```, ambos incluidos, preferentemente el tamaño de un apuntador de memoria de la máquina. Su valor máximo es 2147483647, usando 32 bits._**
   - **_Un tipo ```unsigned``` tiene el mismo tamaño que su versión ```signed```._**
 
### Wchar_t

**_Para la versión del estándar que se publicó en 1998, se decidió añadir el tipo de dato wchar_t, que permite el uso de caracteres UNICODE, a diferencia del tradicional ```char```, que contempla simplemente al código de caracteres ASCII extendido. A su vez, se ha definido para la mayoría de las funciones y clases, tanto de C como de C++, una versión para trabajar con ```wchar_t```, donde usualmente se prefija el carácter w al nombre de la función (en ocasiones el carácter es un infijo). Por ejemplo:_**

 - ```strcpy - wstrcpy```
 - ```std::string - std::wstring```
 - ```std::cout - std::wcout```

**_Cabe resaltar que en C se define ```wchar_t``` como:_**

```typedef unsigned short wchar_t;```

**_Mientras que en C++ es en sí mismo un tipo de dato._**

### La palabra reservada "void"

**_La palabra reservada ```void``` define en C++ el concepto de no existencia o no atribución de un tipo en una variable o declaración. Es decir, una función declarada como ```void``` no devolverá ningún valor. Esta palabra reservada también puede usarse para indicar que una función no recibe parámetros, como en la siguiente declaración:_**

```int funcion (void);```

**_Aunque la tendencia actual es la de no colocar la palabra "void"._**

**_Además se utiliza para determinar que una función no retorna un valor, como en:_**

```void funcion (int parametro);```

**_Cabe destacar que ```void``` no es un tipo. Una función como la declarada anteriormente no puede retornar un valor por medio de return: la palabra clave va sola. No es posible una declaración del tipo:_**

```void t; //Está mal```

**_En este sentido, ```void``` se comporta de forma ligeramente diferente a como lo hace en C, especialmente en cuanto a su significado en declaraciones y prototipos de funciones._**

**_Sin embargo, la forma especial ```void *``` indica que el tipo de datos es un puntero. Por ejemplo:_**

```void *memoria;```

**_Indica que ```memoria``` es un puntero a "alguna parte", donde se guarda información de algún tipo. El programador es responsable de definir estos "algún", eliminando toda ambigüedad. Una ventaja de la declaración "void *" es que puede representar a la vez varios tipos de datos, dependiendo de la operación de cast escogida. La memoria que hemos apuntado en alguna parte, en el ejemplo anterior, bien podría almacenar un entero, un flotante, una cadena de texto o un programa, o combinaciones de estos. Es responsabilidad del programador recordar qué tipo de datos hay y garantizar el acceso adecuado._**

### La palabra "NULL"

**_Además de los valores que pueden tomar los tipos anteriormente mencionados, existe un valor llamado NULL, sea el caso numérico para los enteros, carácter para el tipo char, cadena de texto para el tipo string, etc. El valor NULL, expresa, por lo regular, la representación de una Macro, asignada al valor "0"._**

**_Tenemos entonces que:_**

```
void* puntero = NULL;
int entero = NULL;
bool boleana = NULL;
char caracter = NULL;
```

**_El valor de las variables anteriores nos daría 0. A diferencia de la variable "caracter", que nos daría el equivalente a NULL, '\0', para caracteres._**

**_Para evitar ambigüedad en funciones sobrecargadas, puede emplearse la palabra clave nullptr. Esta palabra clave siempre representa un puntero. Por ejemplo:_**

```
void f(int a);
void f(foo *a);

int main(int argc, char** argv) {
        f(NULL); // Se ejecuta f(int a)
        f(nullptr); // Se ejecuta f(foo *a)
        return 0;
}
```
