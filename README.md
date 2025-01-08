# Cursos-C-
Este Repositorio es para los curos trabajados en la materia de Desarrollo de Software I IDS340-01

# Conceptos básicos de Visual Studio Code

Visual Studio Code (VS Code) es un editor de código fuente desarrollado por Microsoft. Es ligero, potente y extensible, lo que lo convierte en una herramienta popular entre los desarrolladores. A continuación, se presentan algunos conceptos básicos para comenzar a usar VS Code.

## Instalación

1. Descarga VS Code desde [la página oficial](https://code.visualstudio.com/).
2. Sigue las instrucciones de instalación para tu sistema operativo.

## Interfaz de Usuario

La interfaz de VS Code se compone de varios elementos clave:

- **Barra de Actividad**: Ubicada en el lado izquierdo, permite acceder a diferentes vistas como el explorador de archivos, búsqueda, control de versiones, depuración y extensiones.
- **Explorador de Archivos**: Muestra la estructura de archivos y carpetas de tu proyecto.
- **Editor de Código**: Área principal donde se edita el código.
- **Terminal Integrada**: Permite ejecutar comandos de la línea de comandos directamente desde VS Code.
- **Barra de Estado**: Muestra información sobre el archivo actual y el estado del editor.

## Atajos de Teclado

Algunos atajos de teclado útiles en VS Code:

- `Ctrl + P`: Abrir rápidamente un archivo.
- `Ctrl + Shift + P`: Abrir la paleta de comandos.
- `Ctrl + ` (acento grave): Abrir/ocultar la terminal integrada.
- `Ctrl + B`: Mostrar/ocultar el panel lateral.

## Extensiones

VS Code es altamente extensible mediante extensiones. Puedes encontrar y gestionar extensiones desde la vista de extensiones en la barra de actividad. Algunas extensiones populares incluyen:

- **C#**: Soporte para desarrollo en C#.
- **Python**: Soporte para desarrollo en Python.
- **Prettier**: Formateador de código.
- **ESLint**: Herramienta de análisis de código para JavaScript y TypeScript.

## Configuración

La configuración de VS Code se puede personalizar mediante el archivo `settings.json`. Puedes acceder a la configuración desde `Archivo > Preferencias > Configuración` o usando el atajo `Ctrl + ,`.

Ejemplo de configuración en `settings.json`:


# Para comprender mejor la gramática de C# en un alto nivel, vuelva al programa que acabamos de crear para separar cada una de las palabras clave y los símbolos.

Gracias por enviar la imagen nuevamente. Aquí está el análisis del programa, con las palabras clave y los símbolos desglosados y revisados:

### **Código original:**
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World");
            Console.ReadLine();
        }
    }
}
```

### **Análisis de palabras clave y símbolos:**
1. **`using`**: Palabra clave para incluir bibliotecas (o namespaces) necesarias.
2. **`System`**: Namespace que contiene clases como `Console`, utilizadas para entrada y salida en consola.
3. **`;`**: Símbolo que indica el fin de una declaración.
4. **`namespace`**: Palabra clave que define un espacio de nombres para organizar el código.
5. **`HelloWorld`**: Nombre del espacio de nombres definido por el usuario.
6. **`class`**: Palabra clave para declarar una clase.
7. **`Program`**: Nombre de la clase.
8. **`{` y `}`**: Delimitadores de bloques de código.
9. **`static`**: Modificador que indica que el método pertenece a la clase y no a una instancia de la clase.
10. **`void`**: Tipo de retorno del método que indica que no devuelve ningún valor.
11. **`Main`**: Método principal, punto de entrada de la aplicación.
12. **`string[] args`**: Parámetros que el método puede recibir (en este caso, un arreglo de cadenas).
13. **`Console.WriteLine`**: Método que imprime un mensaje en la consola.
14. **`"Hello World"`**: String literal que será mostrado en la consola.
15. **`Console.ReadLine`**: Método que pausa la ejecución hasta que el usuario presiona Enter.

### **Errores potenciales:**
El código está bien estructurado y no presenta errores de sintaxis. Sin embargo, podríamos hacer un pequeño ajuste estético o de funcionalidad:
- Añadir un punto al mensaje "Hello World." para completar la frase.

### **Código revisado y limpio:**
```csharp
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World.");
            Console.ReadLine();
        }
    }
}
```

# Obtenga información sobre cómo crear una aplicación sencilla y obtener una explicación de las soluciones comunes a diferentes problemas que podría surgir al empezar a escribir y compilar código C#

Para crear una aplicación sencilla en C# y abordar problemas comunes que podrían surgir al comenzar a escribir y compilar código, aquí tienes una guía paso a paso:

---

### **Crear una aplicación sencilla en C#**
1. **Instala Visual Studio:**
   - Descarga e instala Visual Studio desde [https://visualstudio.microsoft.com/](https://visualstudio.microsoft.com/).
   - Durante la instalación, selecciona la carga de trabajo **.NET Desktop Development**.

2. **Crea un nuevo proyecto:**
   - Abre Visual Studio.
   - Selecciona **Create a new project**.
   - Elige **Console App (.NET Core)** o **Console App (.NET Framework)**.
   - Especifica un nombre para tu proyecto (por ejemplo, "MiPrimeraApp") y selecciona una ubicación.

3. **Escribe tu primer código:**
   - Por defecto, Visual Studio genera un archivo llamado `Program.cs`.
   - Reemplaza el contenido con el siguiente código simple:
     ```csharp
     using System;

     namespace MiPrimeraApp
     {
         class Program
         {
             static void Main(string[] args)
             {
                 Console.WriteLine("Hola, mundo!");
                 Console.ReadLine();
             }
         }
     }
     ```
   - Este código imprime "Hola, mundo!" en la consola y espera a que el usuario presione Enter.

4. **Ejecuta el programa:**
   - Presiona **F5** o haz clic en el botón **Start** para compilar y ejecutar tu programa.

---

### **Soluciones comunes a problemas iniciales**

1. **Error: No se encuentra el SDK o framework .NET**
   - Asegúrate de haber instalado el **.NET SDK** durante la instalación de Visual Studio.
   - Actualiza Visual Studio si es necesario.

2. **Error: No se reconoce `Console.WriteLine`**
   - Asegúrate de haber incluido el espacio de nombres `using System;` al comienzo de tu archivo.

3. **El programa compila pero no se ejecuta correctamente**
   - Revisa la lógica del código. A menudo, los problemas están relacionados con errores en la sintaxis o lógica.
   - Usa el depurador (tecla **F10** o **F11**) para ejecutar el código línea por línea.

4. **Errores de compilación:**
   - Revisa los mensajes de error en la ventana **Error List** de Visual Studio.
   - Asegúrate de cerrar correctamente los bloques de código con `{}` y de terminar cada declaración con `;`.

5. **El programa se cierra inmediatamente después de ejecutar**
   - Añade `Console.ReadLine();` al final del método `Main` para mantener la consola abierta.

6. **Error al ejecutar un proyecto antiguo en .NET Framework**
   - Si trabajas en un proyecto que utiliza `.NET Framework` pero no está instalado en tu sistema, instala la versión necesaria desde el [sitio oficial de .NET](https://dotnet.microsoft.com/).

7. **Errores relacionados con permisos de archivos**
   - Si estás leyendo/escribiendo archivos, asegúrate de que tu aplicación tiene los permisos necesarios o ejecuta Visual Studio como administrador.

---

### **Próximos pasos para aprender más**
- Aprende a usar estructuras de control como `if`, `while`, y `for`.
- Crea clases y métodos personalizados.
- Explora cómo manejar excepciones usando `try-catch`.
- Experimenta con la creación de aplicaciones gráficas usando **Windows Forms** o **WPF**.

# Agregue la sintaxis de C# al vocabulario mediante la exploración de bloques de creación fundamentales: tipos de datos y variables. Además, obtenga información sobre temas básicos, como convenciones de nomenclatura y conversiones de tipos de datos.

En C#, los bloques fundamentales del lenguaje se construyen con tipos de datos y variables. Aquí tienes una guía detallada sobre estos conceptos, incluyendo las convenciones de nomenclatura y conversiones de tipos de datos:

---

### **Tipos de datos en C#**
C# es un lenguaje fuertemente tipado, lo que significa que cada variable debe tener un tipo específico.

#### **Tipos de datos comunes:**
1. **Números enteros:**
   - `int`: Enteros de 32 bits.
   - `long`: Enteros de 64 bits.
   - `short`: Enteros de 16 bits.
   - `byte`: Enteros sin signo de 8 bits.

2. **Números de punto flotante:**
   - `float`: Precisión simple de 32 bits.
   - `double`: Precisión doble de 64 bits.
   - `decimal`: Precisión alta de 128 bits (usado para cálculos financieros).

3. **Booleanos:**
   - `bool`: Representa valores `true` o `false`.

4. **Cadenas de texto y caracteres:**
   - `string`: Texto o cadenas de caracteres.
   - `char`: Representa un único carácter.

5. **Otros tipos:**
   - `object`: Tipo base para todos los tipos en C#.
   - `var`: Determina el tipo automáticamente en tiempo de compilación.
   - `dynamic`: Determina el tipo en tiempo de ejecución.

---

### **Variables en C#**
Las variables son contenedores para almacenar datos. 

#### **Sintaxis básica:**
```csharp
tipo nombreVariable = valor;
```

#### **Ejemplos:**
```csharp
int edad = 25;
float altura = 1.75f;
string nombre = "Juan";
bool esMayorDeEdad = true;
```

---

### **Convenciones de nomenclatura**
1. **CamelCase:** Para variables y argumentos.
   - Ejemplo: `miVariable`, `alturaPersona`.

2. **PascalCase:** Para nombres de clases y métodos.
   - Ejemplo: `ClasePersona`, `CalcularEdad`.

3. **Nombres descriptivos:**
   - Usa nombres que reflejen el propósito de la variable.
   - Evita abreviaturas innecesarias.

4. **Prefijos para constantes:**
   - Usa mayúsculas con guiones bajos (`_`) para constantes.
   - Ejemplo: `const int MAX_VALOR = 100;`.

---

### **Conversiones de tipos de datos**
C# permite dos tipos de conversiones: implícitas y explícitas.

#### **Conversiones implícitas:**
Se realizan automáticamente cuando no hay pérdida de datos.
```csharp
int entero = 10;
double flotante = entero; // Conversión implícita
```

#### **Conversiones explícitas (casting):**
Se realizan manualmente cuando existe riesgo de pérdida de datos.
```csharp
double flotante = 9.8;
int entero = (int)flotante; // Conversión explícita
```

#### **Usar métodos para conversión:**
```csharp
string numeroTexto = "123";
int numero = int.Parse(numeroTexto); // Convierte string a int

double flotante = Convert.ToDouble(numeroTexto); // Usa Convert para diferentes tipos
```

---

### **Ejemplo práctico:**
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Declaración de variables
        int edad = 30;
        double salario = 45000.75;
        string nombre = "Ana";

        // Mostrar datos
        Console.WriteLine($"Nombre: {nombre}");
        Console.WriteLine($"Edad: {edad}");
        Console.WriteLine($"Salario: ${salario}");

        // Conversión explícita
        int salarioEntero = (int)salario;
        Console.WriteLine($"Salario redondeado: ${salarioEntero}");

        // Conversión de string a int
        string textoNumero = "25";
        int numeroConvertido = int.Parse(textoNumero);
        Console.WriteLine($"Número convertido: {numeroConvertido}");
    }
}
```

# Obtenga una introducción a la instrucción if Decision, junto con el operador condicional. Descubra cómo refactorizar el código para que sea más compacto y menos probable que genere errores.

En C#, las estructuras condicionales como la instrucción `if` y el operador condicional (`?:`) son esenciales para tomar decisiones basadas en condiciones específicas. Aquí te presento una introducción, junto con cómo refactorizar el código para hacerlo más compacto y menos propenso a errores.

---

### **Instrucción `if`**
La instrucción `if` permite ejecutar un bloque de código solo si se cumple una condición.

#### **Sintaxis básica:**
```csharp
if (condición)
{
    // Código a ejecutar si la condición es verdadera
}
else
{
    // Código a ejecutar si la condición es falsa (opcional)
}
```

#### **Ejemplo:**
```csharp
int edad = 20;

if (edad >= 18)
{
    Console.WriteLine("Eres mayor de edad.");
}
else
{
    Console.WriteLine("Eres menor de edad.");
}
```

---

### **Operador condicional (`?:`)**
El operador condicional es una forma compacta de escribir un `if-else`. Evalúa una condición y devuelve un valor dependiendo de si la condición es verdadera o falsa.

#### **Sintaxis:**
```csharp
variable = (condición) ? valor_si_verdadero : valor_si_falso;
```

#### **Ejemplo:**
```csharp
int edad = 20;
string mensaje = (edad >= 18) ? "Eres mayor de edad." : "Eres menor de edad.";
Console.WriteLine(mensaje);
```

---

### **Refactorización para código más compacto**
Refactorizar significa simplificar el código manteniendo su funcionalidad. Aquí hay algunas estrategias:

1. **Usar el operador condicional en lugar de `if-else` simples:**
   ```csharp
   // Antes
   if (edad >= 18)
   {
       mensaje = "Eres mayor de edad.";
   }
   else
   {
       mensaje = "Eres menor de edad.";
   }

   // Después
   mensaje = (edad >= 18) ? "Eres mayor de edad." : "Eres menor de edad.";
   ```

2. **Eliminar bloques innecesarios:**
   Si solo tienes una línea de código dentro de un bloque `if` o `else`, puedes omitir las llaves `{}`.
   ```csharp
   // Antes
   if (edad >= 18)
   {
       Console.WriteLine("Eres mayor de edad.");
   }

   // Después
   if (edad >= 18) Console.WriteLine("Eres mayor de edad.");
   ```

3. **Usar el operador `&&` y `||` para combinar condiciones:**
   En lugar de anidar múltiples `if`, combina condiciones.
   ```csharp
   // Antes
   if (edad >= 18)
   {
       if (esEstudiante)
       {
           Console.WriteLine("Eres un estudiante mayor de edad.");
       }
   }

   // Después
   if (edad >= 18 && esEstudiante)
   {
       Console.WriteLine("Eres un estudiante mayor de edad.");
   }
   ```

---

### **Ejemplo práctico refactorizado**
Aquí hay un ejemplo de cómo aplicar estas ideas para simplificar el código:

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        int edad = 22;
        bool esEstudiante = true;

        // Usando el operador condicional
        string mensaje = (edad >= 18) ? "Mayor de edad" : "Menor de edad";
        Console.WriteLine(mensaje);

        // Usando operadores lógicos
        if (edad >= 18 && esEstudiante)
            Console.WriteLine("Eres un estudiante mayor de edad.");
        else if (edad < 18 && esEstudiante)
            Console.WriteLine("Eres un estudiante menor de edad.");
        else
            Console.WriteLine("No eres estudiante.");
    }
}
```

---

### **Errores comunes al usar `if` y el operador condicional**
1. **Olvidar las llaves `{}` en bloques con múltiples líneas:**
   - Esto puede causar errores de lógica inesperados.
2. **Confundir `=` con `==`:**
   - `=` es una asignación; `==` es una comparación.
   - Ejemplo incorrecto:
     ```csharp
     if (edad = 18) // Error
     ```
     Ejemplo correcto:
     ```csharp
     if (edad == 18)
     ```
3. **No manejar todos los casos posibles:**
   - Siempre asegúrate de cubrir todas las posibles condiciones (por ejemplo, con un `else`).

---

# Examine varios tipos diferentes de instrucciones de iteración, cómo usar fragmentos de código para ayudarle a recordar la sintaxis de esta instrucción compleja y la depuración en acción.

En C#, las instrucciones de iteración permiten ejecutar un bloque de código varias veces, dependiendo de una condición o un rango de valores. Aquí tienes una guía para explorar los tipos de instrucciones de iteración, cómo usar fragmentos de código y consejos sobre depuración.

---

### **1. Tipos de instrucciones de iteración en C#**

#### **a) `for`:**
Se usa cuando conoces de antemano cuántas veces necesitas iterar.

**Sintaxis:**
```csharp
for (inicialización; condición; incremento/decremento)
{
    // Código a ejecutar
}
```

**Ejemplo:**
```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine($"Iteración {i}");
}
```

---

#### **b) `while`:**
Se usa cuando no sabes cuántas veces iterarás, pero tienes una condición para detener la iteración.

**Sintaxis:**
```csharp
while (condición)
{
    // Código a ejecutar
}
```

**Ejemplo:**
```csharp
int contador = 0;
while (contador < 5)
{
    Console.WriteLine($"Contador: {contador}");
    contador++;
}
```

---

#### **c) `do-while`:**
Similar a `while`, pero siempre ejecuta el bloque de código al menos una vez.

**Sintaxis:**
```csharp
do
{
    // Código a ejecutar
} while (condición);
```

**Ejemplo:**
```csharp
int contador = 0;
do
{
    Console.WriteLine($"Contador: {contador}");
    contador++;
} while (contador < 5);
```

---

#### **d) `foreach`:**
Se usa para iterar sobre colecciones (como arreglos o listas).

**Sintaxis:**
```csharp
foreach (var elemento in colección)
{
    // Código a ejecutar
}
```

**Ejemplo:**
```csharp
string[] frutas = { "Manzana", "Plátano", "Naranja" };
foreach (string fruta in frutas)
{
    Console.WriteLine(fruta);
}
```

---

### **2. Uso de fragmentos de código**
Visual Studio proporciona fragmentos de código para ayudarte a recordar la sintaxis de las instrucciones de iteración.

#### **Cómo usar fragmentos de código:**
1. Escribe el inicio del bucle (por ejemplo, `for`) y presiona **Tab** dos veces.
2. El IDE generará automáticamente el fragmento de código con la sintaxis básica.
3. Completa los valores necesarios (como la inicialización, la condición y el incremento).

#### **Ejemplo de fragmento de código para `for`:**
1. Escribe `for` en Visual Studio.
2. Presiona **Tab** dos veces.
3. Resultado:
   ```csharp
   for (int i = 0; i < length; i++)
   {
       // Código
   }
   ```

---

### **3. Depuración en acción**
La depuración es crucial para entender cómo se comportan los bucles en tiempo de ejecución.

#### **Pasos para depurar un bucle:**
1. **Coloca un punto de interrupción:**
   - Haz clic en la barra izquierda del editor al lado de la línea donde comienza el bucle.
2. **Ejecuta el programa en modo de depuración:**
   - Presiona **F5** para iniciar la depuración.
3. **Avanza línea por línea:**
   - Usa **F10** para ejecutar cada línea y observar cómo cambian las variables en cada iteración.
4. **Inspecciona las variables:**
   - Usa la ventana **Watch** o pasa el mouse sobre las variables para ver sus valores actuales.

#### **Errores comunes al depurar bucles:**
- **Bucle infinito:** Ocurre si la condición nunca se evalúa como falsa.
  - Ejemplo:
    ```csharp
    int i = 0;
    while (i < 5)
    {
        Console.WriteLine(i);
        // Falta incrementar 'i', causando un bucle infinito
    }
    ```
- **Acceso fuera de rango:** En un `for`, asegúrate de no acceder a índices fuera del rango de un arreglo.

---

### **Ejemplo práctico:**
Un programa que utiliza diferentes bucles:
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Bucle for
        for (int i = 1; i <= 5; i++)
        {
            Console.WriteLine($"for: Iteración {i}");
        }

        // Bucle while
        int contador = 1;
        while (contador <= 5)
        {
            Console.WriteLine($"while: Iteración {contador}");
            contador++;
        }

        // Bucle do-while
        int numero = 1;
        do
        {
            Console.WriteLine($"do-while: Iteración {numero}");
            numero++;
        } while (numero <= 5);

        // Bucle foreach
        string[] colores = { "Rojo", "Verde", "Azul" };
        foreach (string color in colores)
        {
            Console.WriteLine($"foreach: Color {color}");
        }
    }
}
```

---

# Obtenga información sobre las matrices y vea cómo declarar y usar matrices. Vea demostraciones en un par de métodos integrados eficaces que proporcionan características agregadas a matrices.

En C#, una **matriz** (array) es una estructura de datos que almacena elementos del mismo tipo en ubicaciones contiguas de memoria. Aquí tienes una guía detallada sobre cómo declarar, usar y trabajar con matrices, junto con algunos métodos integrados útiles:

---

### **1. Declaración y uso de matrices**

#### **a) Declarar una matriz:**
```csharp
int[] numeros = new int[5]; // Matriz de tamaño 5
```

#### **b) Inicializar una matriz:**
```csharp
int[] numeros = { 1, 2, 3, 4, 5 }; // Inicialización implícita
```

#### **c) Acceder a los elementos:**
```csharp
Console.WriteLine(numeros[0]); // Accede al primer elemento (1)
numeros[1] = 10;               // Modifica el segundo elemento
```

#### **d) Recorrer una matriz con un bucle:**
```csharp
for (int i = 0; i < numeros.Length; i++)
{
    Console.WriteLine(numeros[i]);
}
```

#### **e) Uso de `foreach`:**
```csharp
foreach (int numero in numeros)
{
    Console.WriteLine(numero);
}
```

---

### **2. Tipos de matrices**

#### **a) Matriz unidimensional:**
```csharp
string[] frutas = { "Manzana", "Plátano", "Naranja" };
```

#### **b) Matriz multidimensional:**
```csharp
int[,] matriz = new int[2, 3]; // 2 filas, 3 columnas
matriz[0, 0] = 1;
matriz[1, 2] = 5;
```

#### **c) Matriz jagged (dentada):**
Es una matriz de matrices.
```csharp
int[][] jaggedArray = new int[2][];
jaggedArray[0] = new int[] { 1, 2, 3 };
jaggedArray[1] = new int[] { 4, 5 };
```

---

### **3. Métodos integrados útiles**

C# ofrece varios métodos para trabajar con matrices, especialmente a través de la clase `Array`.

#### **a) `Array.Sort`: Ordenar elementos**
```csharp
int[] numeros = { 3, 1, 4, 1, 5 };
Array.Sort(numeros);
```

#### **b) `Array.Reverse`: Invertir el orden**
```csharp
Array.Reverse(numeros);
```

#### **c) `Array.IndexOf`: Encontrar el índice de un elemento**
```csharp
int index = Array.IndexOf(numeros, 4); // Devuelve 2 si el 4 está en la posición 2
```

#### **d) `Array.Resize`: Cambiar el tamaño**
```csharp
Array.Resize(ref numeros, 10); // Cambia el tamaño de la matriz a 10
```

---

### **4. Ejemplo práctico**

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Declaración e inicialización
        int[] numeros = { 10, 20, 30, 40, 50 };

        // Recorrer y mostrar elementos
        Console.WriteLine("Elementos en la matriz:");
        foreach (int numero in numeros)
        {
            Console.WriteLine(numero);
        }

        // Ordenar la matriz
        Array.Sort(numeros);
        Console.WriteLine("\nMatriz ordenada:");
        foreach (int numero in numeros)
        {
            Console.WriteLine(numero);
        }

        // Invertir la matriz
        Array.Reverse(numeros);
        Console.WriteLine("\nMatriz invertida:");
        foreach (int numero in numeros)
        {
            Console.WriteLine(numero);
        }

        // Encontrar un elemento
        int indice = Array.IndexOf(numeros, 30);
        Console.WriteLine($"\nEl índice del 30 es: {indice}");
    }
}
```

---

### **5. Consejos para trabajar con matrices**
1. **Validar índices:**
   - Asegúrate de no acceder fuera del rango (`IndexOutOfRangeException`).
   ```csharp
   if (index >= 0 && index < numeros.Length)
   {
       Console.WriteLine(numeros[index]);
   }
   ```

2. **Matrices grandes:**
   - Para conjuntos de datos grandes, considera estructuras como `List<T>` o `ArrayList`.

3. **Uso de `LINQ`:**
   - LINQ ofrece operaciones como `Where`, `Select` y `Sum` para trabajar con matrices de manera más declarativa.
   ```csharp
   int suma = numeros.Sum();
   ```

---

# Cree un método auxiliar, cree y llame a métodos para recuperar un valor, crear y usar parámetros de entrada, obtener información sobre el formato de cadena y crear métodos sobrecargados.

Aquí tienes una guía completa sobre cómo trabajar con métodos en C#, incluyendo la creación de métodos auxiliares, uso de parámetros, sobrecarga de métodos y formateo de cadenas:

---

### **1. Crear un método auxiliar**

Un **método auxiliar** es una función diseñada para realizar una tarea específica que puede ser reutilizada en el código.

#### **Ejemplo básico:**
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Llamar al método auxiliar
        MostrarMensaje();
    }

    static void MostrarMensaje()
    {
        Console.WriteLine("Este es un método auxiliar.");
    }
}
```

---

### **2. Crear y llamar métodos para recuperar un valor**

Un método puede devolver un valor utilizando la palabra clave `return`.

#### **Ejemplo:**
```csharp
static int Sumar(int a, int b)
{
    return a + b; // Devuelve la suma de los números
}

static void Main(string[] args)
{
    int resultado = Sumar(5, 3);
    Console.WriteLine($"El resultado es: {resultado}");
}
```

---

### **3. Crear y usar parámetros de entrada**

Los parámetros permiten pasar información a los métodos.

#### **Ejemplo:**
```csharp
static void Saludar(string nombre)
{
    Console.WriteLine($"Hola, {nombre}!");
}

static void Main(string[] args)
{
    Saludar("Ana");
}
```

#### **Parámetros opcionales:**
Puedes definir valores predeterminados para los parámetros.
```csharp
static void Saludar(string nombre = "Invitado")
{
    Console.WriteLine($"Hola, {nombre}!");
}
```

---

### **4. Formateo de cadenas**

C# permite interpolar cadenas para incluir variables y expresiones dentro de textos.

#### **Ejemplo básico:**
```csharp
string nombre = "Carlos";
int edad = 30;

Console.WriteLine($"Hola, mi nombre es {nombre} y tengo {edad} años.");
```

#### **Formato numérico:**
```csharp
double precio = 1234.5678;
Console.WriteLine($"Precio: {precio:F2}"); // Formato con 2 decimales
```

#### **Alineación y ancho fijo:**
```csharp
Console.WriteLine($"{"Producto",-10} {"Precio",10}");
Console.WriteLine($"{"Manzana",-10} {1.25,10:C}");
```

---

### **5. Crear métodos sobrecargados**

La **sobrecarga** permite definir múltiples métodos con el mismo nombre pero diferentes firmas (número o tipo de parámetros).

#### **Ejemplo:**
```csharp
static void MostrarInformacion(string mensaje)
{
    Console.WriteLine($"Mensaje: {mensaje}");
}

static void MostrarInformacion(int numero)
{
    Console.WriteLine($"Número: {numero}");
}

static void Main(string[] args)
{
    MostrarInformacion("Hola mundo");
    MostrarInformacion(42);
}
```

---

### **6. Ejemplo práctico con todo lo anterior**

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Llamar a un método auxiliar
        MostrarMensaje();

        // Usar un método con parámetros y devolver un valor
        int suma = Sumar(10, 20);
        Console.WriteLine($"La suma es: {suma}");

        // Formateo de cadenas
        string resultadoFormateado = FormatearResultado("Suma", suma);
        Console.WriteLine(resultadoFormateado);

        // Llamar a métodos sobrecargados
        MostrarResultado("Este es un mensaje personalizado.");
        MostrarResultado(42);
    }

    static void MostrarMensaje()
    {
        Console.WriteLine("¡Bienvenido a nuestro programa!");
    }

    static int Sumar(int a, int b)
    {
        return a + b;
    }

    static string FormatearResultado(string operacion, int resultado)
    {
        return $"{operacion}: {resultado}";
    }

    static void MostrarResultado(string mensaje)
    {
        Console.WriteLine($"Mensaje: {mensaje}");
    }

    static void MostrarResultado(int numero)
    {
        Console.WriteLine($"Número: {numero}");
    }
}
```

---

# Trabajar con fechas y horas en C# es fundamental para muchas aplicaciones. Aquí tienes una guía sobre cómo usar la clase `DateTime`, trabajar con instancias, agregar tiempos y dar formato a los datos, además de explorar la clase `TimeSpan`.

---

### **1. Clase `DateTime`**
La clase `DateTime` se utiliza para representar fechas y horas.

#### **a) Crear nuevas instancias:**
```csharp
// Fecha y hora actual
DateTime ahora = DateTime.Now;

// Solo fecha de hoy
DateTime hoy = DateTime.Today;

// Fecha específica
DateTime fechaEspecifica = new DateTime(2024, 12, 21); // Año, mes, día
```

---

#### **b) Acceder a propiedades:**
```csharp
Console.WriteLine(ahora.Year);  // Año
Console.WriteLine(ahora.Month); // Mes
Console.WriteLine(ahora.Day);   // Día
Console.WriteLine(ahora.Hour);  // Hora
Console.WriteLine(ahora.Minute); // Minutos
Console.WriteLine(ahora.Second); // Segundos
```

---

### **2. Agregar tiempo a una fecha**
Puedes modificar instancias de `DateTime` agregando o restando valores.

#### **Ejemplo:**
```csharp
DateTime ahora = DateTime.Now;

// Agregar días
DateTime enUnaSemana = ahora.AddDays(7);

// Restar horas
DateTime haceDosHoras = ahora.AddHours(-2);

// Agregar meses
DateTime proximoMes = ahora.AddMonths(1);
```

---

### **3. Dar formato a fechas**
C# permite dar formato a fechas usando cadenas de formato.

#### **Ejemplos de formato estándar:**
```csharp
DateTime ahora = DateTime.Now;

// Formato corto
Console.WriteLine(ahora.ToShortDateString()); // Ejemplo: 12/21/2024

// Formato largo
Console.WriteLine(ahora.ToLongDateString()); // Ejemplo: Saturday, December 21, 2024

// Formato de hora
Console.WriteLine(ahora.ToShortTimeString()); // Ejemplo: 10:30 PM
Console.WriteLine(ahora.ToLongTimeString());  // Ejemplo: 10:30:45 PM
```

#### **Formatos personalizados:**
```csharp
Console.WriteLine(ahora.ToString("yyyy-MM-dd")); // 2024-12-21
Console.WriteLine(ahora.ToString("dd/MM/yyyy HH:mm:ss")); // 21/12/2024 22:30:45
Console.WriteLine(ahora.ToString("MMMM dd, yyyy")); // December 21, 2024
```

---

### **4. Clase `TimeSpan`**
La clase `TimeSpan` se usa para representar diferencias entre fechas y tiempos.

#### **a) Crear una instancia de `TimeSpan`:**
```csharp
// Intervalo de tiempo de 1 hora, 30 minutos y 15 segundos
TimeSpan intervalo = new TimeSpan(1, 30, 15);

// Diferencia entre dos fechas
DateTime inicio = new DateTime(2024, 12, 21, 10, 0, 0);
DateTime fin = new DateTime(2024, 12, 21, 12, 30, 0);
TimeSpan duracion = fin - inicio;

Console.WriteLine(duracion); // 02:30:00
```

#### **b) Propiedades de `TimeSpan`:**
```csharp
Console.WriteLine(duracion.Hours);   // Horas: 2
Console.WriteLine(duracion.Minutes); // Minutos: 30
Console.WriteLine(duracion.Seconds); // Segundos: 0
Console.WriteLine(duracion.TotalMinutes); // Total en minutos: 150
```

#### **c) Operaciones con `TimeSpan`:**
```csharp
TimeSpan intervalo = new TimeSpan(1, 30, 0); // 1 hora, 30 minutos

// Sumar intervalos
TimeSpan suma = intervalo + TimeSpan.FromMinutes(15);

// Restar intervalos
TimeSpan resta = intervalo - TimeSpan.FromMinutes(30);

Console.WriteLine(suma); // 01:45:00
Console.WriteLine(resta); // 01:00:00
```

---

### **Ejemplo práctico**
```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        // Fecha y hora actuales
        DateTime ahora = DateTime.Now;
        Console.WriteLine($"Fecha y hora actual: {ahora}");

        // Agregar tiempo
        DateTime mañana = ahora.AddDays(1);
        Console.WriteLine($"Mañana será: {mañana.ToShortDateString()}");

        // Formatear la fecha
        Console.WriteLine($"Fecha formateada: {ahora.ToString("dd/MM/yyyy HH:mm")}");

        // Usar TimeSpan
        TimeSpan intervalo = new TimeSpan(2, 15, 30); // 2 horas, 15 minutos, 30 segundos
        Console.WriteLine($"Intervalo: {intervalo}");

        // Diferencia entre fechas
        DateTime inicio = new DateTime(2024, 12, 20, 10, 0, 0);
        DateTime fin = new DateTime(2024, 12, 21, 15, 30, 0);
        TimeSpan duracion = fin - inicio;
        Console.WriteLine($"Duración entre fechas: {duracion.TotalHours} horas");
    }
}
```

---

# Examine los métodos string integrados para manipular el contenido dentro de una cadena literal y en la clase StringBuilder para concatenar muchas cadenas juntas de forma fácil de usar memoria y recursos.

En C#, puedes manipular cadenas utilizando los métodos integrados de la clase `String` y la clase `StringBuilder` para operaciones más eficientes cuando trabajas con grandes volúmenes de concatenación. Aquí te explico ambas formas:

---

### **1. Métodos de la clase `String`**

La clase `String` proporciona una variedad de métodos para trabajar con cadenas. Aquí tienes algunos de los más comunes:

#### **a) Concatenación:**
Combina dos o más cadenas.
```csharp
string saludo = "Hola";
string nombre = "Juan";
string mensaje = string.Concat(saludo, ", ", nombre, "!");
Console.WriteLine(mensaje); // Salida: Hola, Juan!
```

#### **b) Subcadenas (`Substring`):**
Obtiene una parte de la cadena.
```csharp
string texto = "Bienvenido a C#";
string parte = texto.Substring(11); // Desde el índice 11 hasta el final
Console.WriteLine(parte); // Salida: C#
```

#### **c) Buscar texto (`Contains`, `IndexOf`):**
```csharp
string texto = "Aprendiendo C#";
bool contiene = texto.Contains("C#"); // Devuelve true
int indice = texto.IndexOf("C#");     // Devuelve 11
```

#### **d) Reemplazar texto (`Replace`):**
```csharp
string texto = "Hola Mundo";
string nuevoTexto = texto.Replace("Mundo", "C#");
Console.WriteLine(nuevoTexto); // Salida: Hola C#
```

#### **e) Cambiar mayúsculas y minúsculas:**
```csharp
string texto = "Csharp";
Console.WriteLine(texto.ToUpper()); // CSHARP
Console.WriteLine(texto.ToLower()); // csharp
```

#### **f) Dividir cadenas (`Split`) y unirlas (`Join`):**
```csharp
string texto = "uno,dos,tres";
string[] partes = texto.Split(','); // Divide en ["uno", "dos", "tres"]
string unido = string.Join("-", partes); // Une con "-"
Console.WriteLine(unido); // uno-dos-tres
```

---

### **2. Clase `StringBuilder`**

La clase `StringBuilder` es más eficiente que `String` para concatenar muchas cadenas porque no crea nuevas instancias en cada operación.

#### **a) Crear una instancia de `StringBuilder`:**
```csharp
using System.Text;

StringBuilder sb = new StringBuilder("Hola");
sb.Append(", Juan"); // Agrega texto al final
Console.WriteLine(sb.ToString()); // Salida: Hola, Juan
```

#### **b) Insertar texto:**
```csharp
sb.Insert(5, " Mundo");
Console.WriteLine(sb.ToString()); // Salida: Hola Mundo, Juan
```

#### **c) Reemplazar texto:**
```csharp
sb.Replace("Juan", "María");
Console.WriteLine(sb.ToString()); // Salida: Hola Mundo, María
```

#### **d) Eliminar texto:**
```csharp
sb.Remove(5, 6); // Elimina 6 caracteres desde el índice 5
Console.WriteLine(sb.ToString()); // Salida: Hola, María
```

#### **e) Capacidad y longitud:**
```csharp
Console.WriteLine(sb.Capacity); // Capacidad inicial
Console.WriteLine(sb.Length);   // Longitud del contenido actual
```

---

### **3. Comparativa `String` vs `StringBuilder`**

| **Criterio**         | **String**                            | **StringBuilder**                      |
|----------------------|---------------------------------------|---------------------------------------|
| **Mutabilidad**      | Inmutable (cada cambio crea una nueva instancia). | Mutable (se modifica en la misma instancia). |
| **Rendimiento**      | Menos eficiente para múltiples operaciones.  | Más eficiente para muchas concatenaciones.  |
| **Uso común**        | Operaciones simples con cadenas pequeñas. | Concatenación masiva o repetitiva.        |

---

### **4. Ejemplo práctico**

#### **Usando métodos de `String` y `StringBuilder`:**
```csharp
using System;
using System.Text;

class Program
{
    static void Main(string[] args)
    {
        // Usando String
        string texto = "Aprender C# es divertido";
        Console.WriteLine(texto.ToUpper()); // APR...
        Console.WriteLine(texto.Replace("divertido", "interesante")); // Aprender...

        // Usando StringBuilder
        StringBuilder sb = new StringBuilder("Hola");
        sb.Append(" Mundo");
        sb.AppendLine("!");
        sb.Replace("Mundo", "C#");
        Console.WriteLine(sb.ToString()); // Hola C#...
    }
}
```

---

# Obtenga información sobre cómo se definen las clases y se crean nuevas instancias, cómo definir propiedades y cómo establecer valores y obtener valores para una instancia determinada de la clase.

En C#, las clases son el componente fundamental de la programación orientada a objetos. Aquí tienes una guía completa para definir clases, crear instancias y trabajar con propiedades para establecer y obtener valores.

---

### **1. Definir una clase**

Una **clase** es una plantilla que define las propiedades y métodos de un objeto.

#### **Sintaxis básica:**
```csharp
class NombreClase
{
    // Campos
    private int campoPrivado;

    // Propiedades
    public int MiPropiedad { get; set; }

    // Métodos
    public void MostrarMensaje()
    {
        Console.WriteLine("Hola desde la clase!");
    }
}
```

---

### **2. Crear una instancia de una clase**

Una **instancia** es un objeto creado a partir de una clase.

#### **Ejemplo:**
```csharp
class Persona
{
    public string Nombre { get; set; }
    public int Edad { get; set; }
}

class Program
{
    static void Main(string[] args)
    {
        // Crear una instancia de Persona
        Persona persona = new Persona();
        persona.Nombre = "Ana";
        persona.Edad = 25;

        // Mostrar valores
        Console.WriteLine($"Nombre: {persona.Nombre}, Edad: {persona.Edad}");
    }
}
```

---

### **3. Propiedades en clases**

Las **propiedades** permiten controlar el acceso a los datos del objeto.

#### **a) Propiedades automáticas:**
C# permite definir propiedades con `get` y `set` automáticamente.
```csharp
public class Persona
{
    public string Nombre { get; set; } // Propiedad automática
    public int Edad { get; set; }
}
```

#### **b) Propiedades con lógica personalizada:**
Puedes personalizar el comportamiento de `get` y `set`.
```csharp
public class Persona
{
    private int edad;

    public int Edad
    {
        get { return edad; }
        set
        {
            if (value >= 0) edad = value;
            else throw new ArgumentException("La edad no puede ser negativa.");
        }
    }
}
```

---

### **4. Establecer y obtener valores**

#### **Establecer valores:**
```csharp
persona.Nombre = "Carlos";
persona.Edad = 30;
```

#### **Obtener valores:**
```csharp
Console.WriteLine(persona.Nombre); // Carlos
Console.WriteLine(persona.Edad);   // 30
```

---

### **5. Constructor**

Un **constructor** es un método especial que se ejecuta al crear una instancia de la clase.

#### **Constructor predeterminado:**
```csharp
public class Persona
{
    public string Nombre { get; set; }
    public int Edad { get; set; }

    // Constructor
    public Persona()
    {
        Nombre = "Sin nombre";
        Edad = 0;
    }
}
```

#### **Constructor parametrizado:**
```csharp
public class Persona
{
    public string Nombre { get; set; }
    public int Edad { get; set; }

    public Persona(string nombre, int edad)
    {
        Nombre = nombre;
        Edad = edad;
    }
}

// Usar el constructor
Persona persona = new Persona("Luis", 28);
```

---

### **6. Ejemplo práctico**

Aquí hay un programa que combina todos los conceptos:
```csharp
using System;

class Persona
{
    // Propiedades
    public string Nombre { get; set; }
    public int Edad { get; set; }

    // Constructor
    public Persona(string nombre, int edad)
    {
        Nombre = nombre;
        Edad = edad;
    }

    // Método
    public void Presentarse()
    {
        Console.WriteLine($"Hola, mi nombre es {Nombre} y tengo {Edad} años.");
    }
}

class Program
{
    static void Main(string[] args)
    {
        // Crear una instancia de Persona
        Persona persona = new Persona("María", 30);

        // Llamar al método
        persona.Presentarse();
    }
}
```

---

### **7. Ventajas de las clases**
- Reutilización del código.
- Organización clara del proyecto.
- Encapsulación para proteger los datos.
- Abstracción para ocultar detalles innecesarios.

---

# Explore el ámbito de las variables y cómo la biblioteca de clases de .NET Framework usa los modificadores de accesibilidad para exponer u ocultar la implementación de sus servicios dados a los consumidores de esa clase determinada.

En C#, el **ámbito de las variables** y los **modificadores de accesibilidad** son fundamentales para controlar cómo y dónde se pueden acceder a las variables y métodos en un programa. Además, .NET Framework utiliza estos conceptos para exponer o proteger funcionalidades dentro de clases y servicios.

---

### **1. Ámbito de las variables**

El ámbito define dónde una variable es accesible dentro del código. Hay cuatro niveles principales de ámbito:

#### **a) Ámbito local:**
Las variables declaradas dentro de un método o bloque son locales a ese método o bloque.
```csharp
void Metodo()
{
    int numero = 5; // Variable local
    Console.WriteLine(numero);
}
// 'numero' no está accesible fuera de Metodo.
```

#### **b) Ámbito de clase:**
Las variables declaradas fuera de cualquier método, pero dentro de una clase, son accesibles por todos los métodos de la clase.
```csharp
class MiClase
{
    private int edad = 25; // Ámbito de clase

    void MostrarEdad()
    {
        Console.WriteLine(edad);
    }
}
```

#### **c) Ámbito estático:**
Las variables declaradas con el modificador `static` pertenecen a la clase en lugar de a una instancia específica.
```csharp
class Ejemplo
{
    static int contador = 0;

    public static void Incrementar()
    {
        contador++;
        Console.WriteLine(contador);
    }
}
```

#### **d) Ámbito global:**
En C#, no existe un verdadero "ámbito global", pero las variables estáticas accesibles desde cualquier parte de un programa pueden simularlo.

---

### **2. Modificadores de accesibilidad**

Los **modificadores de accesibilidad** controlan la visibilidad de clases, métodos y variables. En C#, estos son los principales:

#### **a) `public`:**
Accesible desde cualquier lugar.
```csharp
public class MiClase
{
    public int MiPropiedad { get; set; }
}
```

#### **b) `private`:**
Accesible solo dentro de la clase donde se define.
```csharp
class MiClase
{
    private int edad;

    private void MostrarEdad()
    {
        Console.WriteLine(edad);
    }
}
```

#### **c) `protected`:**
Accesible dentro de la clase y sus clases derivadas.
```csharp
class MiClase
{
    protected int edad;

    protected void MostrarEdad()
    {
        Console.WriteLine(edad);
    }
}
```

#### **d) `internal`:**
Accesible solo dentro del mismo ensamblado.
```csharp
internal class MiClase
{
    internal int MiPropiedad { get; set; }
}
```

#### **e) `protected internal`:**
Accesible dentro del mismo ensamblado y también en clases derivadas fuera del ensamblado.
```csharp
protected internal void Metodo()
{
    // Código
}
```

#### **f) `private protected`:**
Accesible solo dentro de la clase y sus derivadas dentro del mismo ensamblado.
```csharp
private protected int MiCampo;
```

---

### **3. Uso de modificadores en .NET Framework**

#### **Exponer funcionalidades públicas:**
Las clases y métodos públicos en .NET permiten a los desarrolladores consumir servicios sin conocer la implementación interna.

**Ejemplo:**
```csharp
public class MathHelper
{
    public static int Sumar(int a, int b)
    {
        return a + b; // Método público expuesto
    }
}
```

#### **Ocultar implementación interna:**
.NET utiliza modificadores como `internal` y `private` para proteger detalles internos de implementación.

**Ejemplo:**
```csharp
internal class InternalHelper
{
    private void HelperMethod()
    {
        Console.WriteLine("Este método no está expuesto.");
    }
}
```

---

### **4. Ejemplo práctico**

Un ejemplo que combina ámbitos y modificadores de accesibilidad:
```csharp
using System;

class Persona
{
    // Campo privado
    private string nombre;

    // Propiedad pública para exponer el campo
    public string Nombre
    {
        get { return nombre; }
        set { nombre = value; }
    }

    // Método protegido (solo accesible por clases derivadas)
    protected void Saludar()
    {
        Console.WriteLine($"Hola, {nombre}");
    }
}

class Empleado : Persona
{
    public void MostrarSaludo()
    {
        Saludar(); // Llamada al método protegido
    }
}

class Program
{
    static void Main(string[] args)
    {
        Empleado empleado = new Empleado();
        empleado.Nombre = "Juan"; // Usando la propiedad pública
        empleado.MostrarSaludo();
    }
}
```

---

### **5. Ventajas de los modificadores de accesibilidad**
1. **Encapsulación:** Protege los datos y métodos internos para evitar acceso directo no deseado.
2. **Modularidad:** Facilita la construcción de clases reutilizables y seguras.
3. **Seguridad:** Minimiza los riesgos de errores al limitar la visibilidad del código.

---

# Profundice en más detalles sobre las clases: cree una nueva instancia, agregue referencias de clase y pase la referencia a un método. Además, revise los métodos sobrecargados, los métodos estáticos frente a los métodos de instancia y los constructores.

Profundicemos en el manejo avanzado de clases en C#. Aquí abordaremos cómo crear instancias, pasar referencias a métodos, usar métodos sobrecargados, distinguir entre métodos estáticos y de instancia, y trabajar con constructores.

---

### **1. Crear una nueva instancia de clase**

Una instancia de clase es un objeto creado a partir de una clase.

#### **Ejemplo básico:**
```csharp
class Persona
{
    public string Nombre { get; set; }
    public int Edad { get; set; }
}

class Program
{
    static void Main(string[] args)
    {
        Persona persona = new Persona();
        persona.Nombre = "Ana";
        persona.Edad = 25;

        Console.WriteLine($"Nombre: {persona.Nombre}, Edad: {persona.Edad}");
    }
}
```

---

### **2. Agregar referencias de clase y pasarlas a un método**

#### **Referencia de clase:**
Cuando pasas un objeto a un método, estás pasando una referencia, no una copia.

#### **Ejemplo:**
```csharp
class Persona
{
    public string Nombre { get; set; }
    public int Edad { get; set; }
}

class Program
{
    static void CambiarNombre(Persona persona, string nuevoNombre)
    {
        persona.Nombre = nuevoNombre; // Cambia directamente el valor en la referencia
    }

    static void Main(string[] args)
    {
        Persona persona = new Persona { Nombre = "Juan", Edad = 30 };

        Console.WriteLine($"Antes: {persona.Nombre}");
        CambiarNombre(persona, "Carlos");
        Console.WriteLine($"Después: {persona.Nombre}");
    }
}
```
- **Resultado:**
  - Antes: Juan
  - Después: Carlos

---

### **3. Métodos sobrecargados**

La **sobrecarga de métodos** permite definir múltiples métodos con el mismo nombre, pero con diferentes parámetros.

#### **Ejemplo:**
```csharp
class Calculadora
{
    public int Sumar(int a, int b) => a + b;

    public double Sumar(double a, double b) => a + b;

    public int Sumar(int a, int b, int c) => a + b + c;
}

class Program
{
    static void Main(string[] args)
    {
        Calculadora calc = new Calculadora();

        Console.WriteLine(calc.Sumar(2, 3));       // Usa Sumar(int, int)
        Console.WriteLine(calc.Sumar(2.5, 3.5)); // Usa Sumar(double, double)
        Console.WriteLine(calc.Sumar(1, 2, 3));   // Usa Sumar(int, int, int)
    }
}
```

---

### **4. Métodos estáticos frente a métodos de instancia**

#### **Métodos de instancia:**
Dependen de una instancia de la clase y pueden acceder a propiedades y métodos no estáticos.
```csharp
class Persona
{
    public string Nombre { get; set; }

    public void Saludar()
    {
        Console.WriteLine($"Hola, soy {Nombre}");
    }
}

class Program
{
    static void Main(string[] args)
    {
        Persona persona = new Persona { Nombre = "Ana" };
        persona.Saludar(); // Llamada al método de instancia
    }
}
```

#### **Métodos estáticos:**
Pertenecen a la clase y no necesitan una instancia para ser llamados.
```csharp
class Calculadora
{
    public static int Sumar(int a, int b) => a + b;
}

class Program
{
    static void Main(string[] args)
    {
        int resultado = Calculadora.Sumar(5, 10); // Llamada al método estático
        Console.WriteLine($"Resultado: {resultado}");
    }
}
```

---

### **5. Constructores**

Un **constructor** es un método especial que inicializa los objetos de una clase.

#### **Constructor predeterminado:**
```csharp
class Persona
{
    public string Nombre { get; set; }

    // Constructor predeterminado
    public Persona()
    {
        Nombre = "Sin nombre";
    }
}

class Program
{
    static void Main(string[] args)
    {
        Persona persona = new Persona();
        Console.WriteLine($"Nombre: {persona.Nombre}");
    }
}
```

#### **Constructor parametrizado:**
```csharp
class Persona
{
    public string Nombre { get; set; }
    public int Edad { get; set; }

    public Persona(string nombre, int edad)
    {
        Nombre = nombre;
        Edad = edad;
    }
}

class Program
{
    static void Main(string[] args)
    {
        Persona persona = new Persona("Carlos", 25);
        Console.WriteLine($"Nombre: {persona.Nombre}, Edad: {persona.Edad}");
    }
}
```

---

### **6. Ejemplo práctico que combina todos los conceptos**

```csharp
using System;

class Persona
{
    public string Nombre { get; set; }
    public int Edad { get; set; }

    // Constructor predeterminado
    public Persona()
    {
        Nombre = "Desconocido";
        Edad = 0;
    }

    // Constructor parametrizado
    public Persona(string nombre, int edad)
    {
        Nombre = nombre;
        Edad = edad;
    }

    // Método de instancia
    public void Presentarse()
    {
        Console.WriteLine($"Hola, soy {Nombre} y tengo {Edad} años.");
    }

    // Método estático
    public static void Despedida()
    {
        Console.WriteLine("Adiós desde la clase Persona.");
    }
}

class Program
{
    static void Main(string[] args)
    {
        // Crear instancia usando el constructor predeterminado
        Persona p1 = new Persona();
        p1.Presentarse();

        // Crear instancia usando el constructor parametrizado
        Persona p2 = new Persona("Ana", 30);
        p2.Presentarse();

        // Llamar a un método estático
        Persona.Despedida();
    }
}
```

---

# Obtenga información sobre los ensamblados de .NET: bibliotecas de código y ejecutables, depuración y versiones de lanzamiento de ensamblados. Además, consulte cómo hacer referencia a ensamblados, usar NuGet y crear referencias a bibliotecas personalizadas.

En C#, los **ensamblados** son bloques fundamentales del .NET Framework, que incluyen bibliotecas de código y ejecutables. Aquí tienes una guía detallada sobre ensamblados, depuración, versiones, referencias y uso de bibliotecas personalizadas.

---

### **1. ¿Qué es un ensamblado?**
Un ensamblado es una unidad compilada de código que .NET usa para ejecutar aplicaciones. Puede ser:
- **Biblioteca de clases (.dll)**: Contiene código reutilizable que otros programas pueden consumir.
- **Ejecutable (.exe)**: Un programa independiente.

Cada ensamblado contiene:
- Código intermedio (IL).
- Metadatos sobre tipos y referencias.
- Un manifiesto que describe el ensamblado.

---

### **2. Crear un ensamblado en C#**

#### **a) Crear una biblioteca de clases:**
1. Abre Visual Studio.
2. Crea un nuevo proyecto y selecciona **Class Library**.
3. Escribe el código deseado.
4. Compila para generar un archivo `.dll`.

**Ejemplo:**
```csharp
namespace MiBiblioteca
{
    public class Calculadora
    {
        public int Sumar(int a, int b) => a + b;
    }
}
```

#### **b) Crear un ejecutable:**
1. Abre Visual Studio.
2. Crea un proyecto de **Aplicación de Consola**.
3. Escribe el código deseado y compila para generar un archivo `.exe`.

---

### **3. Referenciar ensamblados**

#### **a) Referenciar un ensamblado en un proyecto:**
1. Haz clic derecho en **Dependencias** en el Explorador de Soluciones.
2. Selecciona **Agregar referencia**.
3. Navega hasta el ensamblado `.dll` y agrégalo.

#### **b) Usar el ensamblado en código:**
```csharp
using MiBiblioteca;

class Program
{
    static void Main(string[] args)
    {
        Calculadora calc = new Calculadora();
        Console.WriteLine(calc.Sumar(3, 5));
    }
}
```

---

### **4. Usar NuGet para administrar ensamblados**

NuGet es un gestor de paquetes para .NET que permite instalar bibliotecas de terceros.

#### **Pasos:**
1. Haz clic derecho en **Dependencias** > **Administrar paquetes NuGet**.
2. Busca el paquete deseado.
3. Instálalo y confirma.
4. Usa la biblioteca en tu código.

**Ejemplo:**
Para instalar Newtonsoft.Json:
```csharp
// Instalar:
Install-Package Newtonsoft.Json
```

Código:
```csharp
using Newtonsoft.Json;

class Program
{
    static void Main(string[] args)
    {
        var persona = new { Nombre = "Juan", Edad = 30 };
        string json = JsonConvert.SerializeObject(persona);
        Console.WriteLine(json);
    }
}
```

---

### **5. Depuración de ensamblados**

#### **a) Depuración local:**
- Configura puntos de interrupción en tu código.
- Usa **F5** para iniciar la depuración.

#### **b) Depuración de una biblioteca:**
1. Incluye los símbolos de depuración (`.pdb`) en el proyecto.
2. Configura el ensamblado como referencia y habilita la depuración externa.

---

### **6. Versionado de ensamblados**

El manifiesto del ensamblado incluye información sobre su versión. Una versión tiene cuatro partes:
```csharp
[assembly: AssemblyVersion("1.0.0.0")]
```

#### **Convenciones:**
1. **Major**: Cambios importantes.
2. **Minor**: Nuevas características.
3. **Build**: Cambios menores o correcciones.
4. **Revision**: Parche o hotfix.

---

### **7. Crear referencias a bibliotecas personalizadas**

1. Compila tu biblioteca personalizada.
2. Agrega la referencia en otros proyectos.
3. Usa el código de la biblioteca en tu programa principal.

---

### **8. Ejemplo práctico**

#### **Paso 1: Crear biblioteca (MiBiblioteca.dll):**
```csharp
namespace MiBiblioteca
{
    public class Calculadora
    {
        public int Sumar(int a, int b) => a + b;
    }
}
```

#### **Paso 2: Usar la biblioteca en otro proyecto:**
```csharp
using MiBiblioteca;

class Program
{
    static void Main(string[] args)
    {
        Calculadora calc = new Calculadora();
        Console.WriteLine($"Suma: {calc.Sumar(3, 5)}");
    }
}
```

---

# Vea una colección de estilos antigua, junto con varias de las colecciones genéricas más recientes y fuertemente tipadas (List y Dictionary) utilizando la sintaxis genérica.

En C#, las colecciones son herramientas esenciales para almacenar y manipular grupos de datos. Vamos a explorar:

1. **Colecciones antiguas (no genéricas):** Como `ArrayList`.
2. **Colecciones genéricas (más modernas):** Como `List<T>` y `Dictionary<TKey, TValue>`.

---

### **1. Colecciones antiguas: `ArrayList`**

El `ArrayList` es una colección que puede almacenar elementos de cualquier tipo, pero carece de seguridad de tipos.

#### **Ejemplo:**
```csharp
using System;
using System.Collections;

class Program
{
    static void Main(string[] args)
    {
        // Crear un ArrayList
        ArrayList lista = new ArrayList();
        
        // Agregar elementos de diferentes tipos
        lista.Add(1);       // Entero
        lista.Add("Hola");  // Cadena
        lista.Add(3.14);    // Doble

        // Recorrer el ArrayList
        foreach (var item in lista)
        {
            Console.WriteLine(item);
        }
    }
}
```

#### **Problemas:**
- No tiene seguridad de tipos (pueden ocurrir errores en tiempo de ejecución).
- Operaciones de conversión pueden ser necesarias.

---

### **2. Colecciones genéricas modernas**

Las colecciones genéricas se introdujeron con .NET 2.0. Ofrecen:
- **Seguridad de tipos**: Solo aceptan elementos del tipo especificado.
- **Mejor rendimiento**: Evitan conversiones innecesarias.

---

#### **a) `List<T>`**

Una lista genérica que almacena elementos de un tipo específico.

##### **Ejemplo:**
```csharp
using System;
using System.Collections.Generic;

class Program
{
    static void Main(string[] args)
    {
        // Crear una lista genérica de enteros
        List<int> numeros = new List<int> { 1, 2, 3 };

        // Agregar elementos
        numeros.Add(4);
        numeros.Add(5);

        // Acceder por índice
        Console.WriteLine($"Primer número: {numeros[0]}");

        // Recorrer la lista
        foreach (int numero in numeros)
        {
            Console.WriteLine(numero);
        }
    }
}
```

##### **Métodos comunes de `List<T>`:**
- `Add`: Agregar un elemento.
- `Remove`: Eliminar un elemento.
- `Contains`: Verificar si existe un elemento.
- `Count`: Obtener el número de elementos.

---

#### **b) `Dictionary<TKey, TValue>`**

Una colección que almacena pares clave-valor. Es útil para búsquedas rápidas.

##### **Ejemplo:**
```csharp
using System;
using System.Collections.Generic;

class Program
{
    static void Main(string[] args)
    {
        // Crear un diccionario
        Dictionary<string, int> edades = new Dictionary<string, int>
        {
            { "Juan", 25 },
            { "Ana", 30 }
        };

        // Agregar elementos
        edades["Luis"] = 35;

        // Acceder a un valor por clave
        Console.WriteLine($"Edad de Juan: {edades["Juan"]}");

        // Recorrer el diccionario
        foreach (var par in edades)
        {
            Console.WriteLine($"{par.Key}: {par.Value}");
        }
    }
}
```

##### **Métodos comunes de `Dictionary<TKey, TValue>`:**
- `Add`: Agregar un par clave-valor.
- `ContainsKey`: Verificar si una clave existe.
- `Remove`: Eliminar un par clave-valor.
- `Count`: Obtener el número de pares en el diccionario.

---

### **3. Comparativa: `ArrayList` vs `List<T>` y `Dictionary<TKey, TValue>`**

| **Característica**          | **ArrayList**             | **List<T>**                | **Dictionary<TKey, TValue>** |
|-----------------------------|---------------------------|----------------------------|-------------------------------|
| **Seguridad de tipos**      | No                       | Sí                         | Sí                            |
| **Uso de memoria**          | Menos eficiente          | Más eficiente              | Más eficiente                 |
| **Acceso por índice**       | Sí                       | Sí                         | No                            |
| **Acceso por clave**        | No                       | No                         | Sí                            |
| **Velocidad de búsqueda**   | Lenta (lineal)           | Lenta (lineal)             | Rápida (hashing)              |

---

### **4. Ejemplo combinado**
Aquí hay un ejemplo que combina `List<T>` y `Dictionary<TKey, TValue>`:

```csharp
using System;
using System.Collections.Generic;

class Program
{
    static void Main(string[] args)
    {
        // Lista de nombres
        List<string> nombres = new List<string> { "Juan", "Ana", "Luis" };
        nombres.Add("María");

        Console.WriteLine("Lista de nombres:");
        foreach (string nombre in nombres)
        {
            Console.WriteLine(nombre);
        }

        // Diccionario de edades
        Dictionary<string, int> edades = new Dictionary<string, int>();
        edades["Juan"] = 25;
        edades["Ana"] = 30;

        Console.WriteLine("\nEdades en el diccionario:");
        foreach (var par in edades)
        {
            Console.WriteLine($"{par.Key}: {par.Value} años");
        }
    }
}
```

---

### **Conclusión**
- **ArrayList** es útil para compatibilidad con versiones anteriores, pero `List<T>` y `Dictionary<TKey, TValue>` son preferibles por su seguridad de tipos y mejor rendimiento.
- Usa `List<T>` para almacenar elementos de un tipo específico en orden.
- Usa `Dictionary<TKey, TValue>` para búsquedas rápidas mediante claves.

# Vea una demostración sobre el uso de Enumeraciones, cree una enumeración personalizada y después úsela en una aplicación sencilla que muestre una tercera instrucción Decision, el modificador.

En C#, una **enumeración** (enum) es una colección de constantes con nombres que representan valores específicos. Son útiles para representar un conjunto limitado de opciones, como días de la semana, estados de un proceso, etc.

Aquí tienes una demostración paso a paso:

---

### **1. Crear una enumeración personalizada**

#### **Ejemplo:**
Creamos una enumeración para representar los días de la semana:
```csharp
public enum DiasSemana
{
    Lunes,
    Martes,
    Miercoles,
    Jueves,
    Viernes,
    Sabado,
    Domingo
}
```
- Por defecto, los valores de la enumeración son enteros empezando desde 0.
- Puedes asignar valores personalizados:
```csharp
public enum DiasSemana
{
    Lunes = 1,
    Martes = 2,
    Miercoles = 3,
    Jueves = 4,
    Viernes = 5,
    Sabado = 6,
    Domingo = 7
}
```

---

### **2. Usar la enumeración en una aplicación sencilla**

Vamos a usar `DiasSemana` en un programa que tome una entrada y realice una acción basada en el valor ingresado.

#### **Ejemplo completo:**
```csharp
using System;

public enum DiasSemana
{
    Lunes = 1,
    Martes,
    Miercoles,
    Jueves,
    Viernes,
    Sabado,
    Domingo
}

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Ingrese un número del 1 al 7 para seleccionar un día de la semana:");
        int opcion = int.Parse(Console.ReadLine());

        // Convertir el número ingresado a la enumeración
        if (Enum.IsDefined(typeof(DiasSemana), opcion))
        {
            DiasSemana diaSeleccionado = (DiasSemana)opcion;

            // Mostrar una decisión basada en la enumeración
            switch (diaSeleccionado)
            {
                case DiasSemana.Lunes:
                    Console.WriteLine("¡Es lunes! Inicio de la semana.");
                    break;
                case DiasSemana.Viernes:
                    Console.WriteLine("¡Es viernes! Fin de la semana laboral.");
                    break;
                case DiasSemana.Sabado:
                case DiasSemana.Domingo:
                    Console.WriteLine("¡Es fin de semana! Hora de descansar.");
                    break;
                default:
                    Console.WriteLine($"Es {diaSeleccionado}, sigue trabajando.");
                    break;
            }
        }
        else
        {
            Console.WriteLine("El número ingresado no es válido.");
        }
    }
}
```

---

### **3. Modificadores: Usar enumeraciones como parámetros o propiedades**

Puedes usar una enumeración como:
1. **Propiedad en una clase:**
```csharp
public class Actividad
{
    public string Nombre { get; set; }
    public DiasSemana Dia { get; set; }
}
```

2. **Parámetro de un método:**
```csharp
public static void MostrarMensaje(DiasSemana dia)
{
    Console.WriteLine($"El día seleccionado es: {dia}");
}

// Llamada al método
MostrarMensaje(DiasSemana.Martes);
```

---

### **4. Ventajas de las enumeraciones**
- **Legibilidad:** Los nombres significativos hacen que el código sea más fácil de entender.
- **Seguridad de tipos:** Evita valores inválidos.
- **Facilidad de mantenimiento:** Cambiar los valores en la enumeración actualiza el código automáticamente.

---

### **5. Resumen del programa**
- Creamos una enumeración `DiasSemana`.
- La usamos en una aplicación para tomar una decisión basada en el valor ingresado.
- Aplicamos la enumeración como propiedad y parámetro.

# Explore Lenguaje de consulta estructurado y la sintaxis LINQ. Consulte una demostración de la proyección de datos en tipos existentes y nuevos tipos anónimos.

En C#, **LINQ** (Language-Integrated Query) es una poderosa herramienta para trabajar con datos de manera declarativa y sencilla. Te permite consultar y manipular colecciones en memoria, bases de datos, XML, y más.

A continuación, exploraremos la **sintaxis LINQ**, cómo proyectar datos en tipos existentes y cómo crear tipos anónimos.

---

### **1. Sintaxis LINQ**

LINQ ofrece dos formas principales de sintaxis:
1. **Sintaxis de consulta** (similar al SQL).
2. **Sintaxis de métodos** (más común).

#### **Ejemplo básico:**
Dado un arreglo de números, seleccionemos los números pares:
```csharp
using System;
using System.Linq;

class Program
{
    static void Main(string[] args)
    {
        int[] numeros = { 1, 2, 3, 4, 5, 6 };

        // Sintaxis de consulta
        var paresConsulta = from n in numeros
                            where n % 2 == 0
                            select n;

        // Sintaxis de métodos
        var paresMetodo = numeros.Where(n => n % 2 == 0);

        Console.WriteLine("Números pares:");
        foreach (var numero in paresMetodo)
        {
            Console.WriteLine(numero);
        }
    }
}
```

---

### **2. Proyección de datos en tipos existentes**

La **proyección** transforma los datos de una colección en otra estructura. Si los datos se proyectan en un tipo existente, se usan constructores o inicializadores de objetos.

#### **Ejemplo: Proyección en una clase existente**
```csharp
using System;
using System.Linq;
using System.Collections.Generic;

public class Producto
{
    public string Nombre { get; set; }
    public decimal Precio { get; set; }
}

public class ProductoConDescuento
{
    public string Nombre { get; set; }
    public decimal PrecioConDescuento { get; set; }
}

class Program
{
    static void Main(string[] args)
    {
        List<Producto> productos = new List<Producto>
        {
            new Producto { Nombre = "Camisa", Precio = 500 },
            new Producto { Nombre = "Pantalón", Precio = 700 },
            new Producto { Nombre = "Zapatos", Precio = 1200 }
        };

        // Proyectar a un nuevo tipo
        var productosConDescuento = productos
            .Select(p => new ProductoConDescuento
            {
                Nombre = p.Nombre,
                PrecioConDescuento = p.Precio * 0.9m // 10% de descuento
            });

        Console.WriteLine("Productos con descuento:");
        foreach (var producto in productosConDescuento)
        {
            Console.WriteLine($"{producto.Nombre}: ${producto.PrecioConDescuento}");
        }
    }
}
```

---

### **3. Proyección en tipos anónimos**

Los **tipos anónimos** permiten crear estructuras temporales sin definir una clase explícita.

#### **Ejemplo: Proyección en un tipo anónimo**
```csharp
using System;
using System.Linq;
using System.Collections.Generic;

class Program
{
    static void Main(string[] args)
    {
        List<Producto> productos = new List<Producto>
        {
            new Producto { Nombre = "Camisa", Precio = 500 },
            new Producto { Nombre = "Pantalón", Precio = 700 },
            new Producto { Nombre = "Zapatos", Precio = 1200 }
        };

        // Proyección en un tipo anónimo
        var productosConDescuento = productos
            .Select(p => new
            {
                p.Nombre,
                PrecioConDescuento = p.Precio * 0.9m
            });

        Console.WriteLine("Productos con descuento (tipo anónimo):");
        foreach (var producto in productosConDescuento)
        {
            Console.WriteLine($"{producto.Nombre}: ${producto.PrecioConDescuento}");
        }
    }
}

public class Producto
{
    public string Nombre { get; set; }
    public decimal Precio { get; set; }
}
```

---

### **4. Consultas avanzadas**

#### **a) Proyección múltiple con `join`:**
Combina dos colecciones relacionadas.
```csharp
var empleados = new List<Empleado>
{
    new Empleado { Id = 1, Nombre = "Juan" },
    new Empleado { Id = 2, Nombre = "Ana" }
};

var departamentos = new List<Departamento>
{
    new Departamento { EmpleadoId = 1, Nombre = "IT" },
    new Departamento { EmpleadoId = 2, Nombre = "RRHH" }
};

// Sintaxis de consulta
var consulta = from e in empleados
               join d in departamentos on e.Id equals d.EmpleadoId
               select new { e.Nombre, Departamento = d.Nombre };

foreach (var resultado in consulta)
{
    Console.WriteLine($"{resultado.Nombre} trabaja en {resultado.Departamento}");
}
```

#### **b) Métodos de agregación:**
Calcula valores como suma, promedio, máximo y mínimo.
```csharp
var precios = new[] { 100m, 200m, 300m };

decimal total = precios.Sum();
decimal promedio = precios.Average();

Console.WriteLine($"Total: {total}, Promedio: {promedio}");
```

---

### **5. Ventajas de LINQ**
1. **Legibilidad:** Sintaxis clara y declarativa.
2. **Versatilidad:** Compatible con bases de datos, colecciones en memoria, XML, y más.
3. **Seguridad de tipos:** Los errores se detectan en tiempo de compilación.
4. **Reutilización:** Es posible encadenar operaciones complejas fácilmente.

---

# En C#, **LINQ** (Language-Integrated Query) es una poderosa herramienta para trabajar con datos de manera declarativa y sencilla. Te permite consultar y manipular colecciones en memoria, bases de datos, XML, y más.

A continuación, exploraremos la **sintaxis LINQ**, cómo proyectar datos en tipos existentes y cómo crear tipos anónimos.

---

### **1. Sintaxis LINQ**

LINQ ofrece dos formas principales de sintaxis:
1. **Sintaxis de consulta** (similar al SQL).
2. **Sintaxis de métodos** (más común).

#### **Ejemplo básico:**
Dado un arreglo de números, seleccionemos los números pares:
```csharp
using System;
using System.Linq;

class Program
{
    static void Main(string[] args)
    {
        int[] numeros = { 1, 2, 3, 4, 5, 6 };

        // Sintaxis de consulta
        var paresConsulta = from n in numeros
                            where n % 2 == 0
                            select n;

        // Sintaxis de métodos
        var paresMetodo = numeros.Where(n => n % 2 == 0);

        Console.WriteLine("Números pares:");
        foreach (var numero in paresMetodo)
        {
            Console.WriteLine(numero);
        }
    }
}
```

---

### **2. Proyección de datos en tipos existentes**

La **proyección** transforma los datos de una colección en otra estructura. Si los datos se proyectan en un tipo existente, se usan constructores o inicializadores de objetos.

#### **Ejemplo: Proyección en una clase existente**
```csharp
using System;
using System.Linq;
using System.Collections.Generic;

public class Producto
{
    public string Nombre { get; set; }
    public decimal Precio { get; set; }
}

public class ProductoConDescuento
{
    public string Nombre { get; set; }
    public decimal PrecioConDescuento { get; set; }
}

class Program
{
    static void Main(string[] args)
    {
        List<Producto> productos = new List<Producto>
        {
            new Producto { Nombre = "Camisa", Precio = 500 },
            new Producto { Nombre = "Pantalón", Precio = 700 },
            new Producto { Nombre = "Zapatos", Precio = 1200 }
        };

        // Proyectar a un nuevo tipo
        var productosConDescuento = productos
            .Select(p => new ProductoConDescuento
            {
                Nombre = p.Nombre,
                PrecioConDescuento = p.Precio * 0.9m // 10% de descuento
            });

        Console.WriteLine("Productos con descuento:");
        foreach (var producto in productosConDescuento)
        {
            Console.WriteLine($"{producto.Nombre}: ${producto.PrecioConDescuento}");
        }
    }
}
```

---

### **3. Proyección en tipos anónimos**

Los **tipos anónimos** permiten crear estructuras temporales sin definir una clase explícita.

#### **Ejemplo: Proyección en un tipo anónimo**
```csharp
using System;
using System.Linq;
using System.Collections.Generic;

class Program
{
    static void Main(string[] args)
    {
        List<Producto> productos = new List<Producto>
        {
            new Producto { Nombre = "Camisa", Precio = 500 },
            new Producto { Nombre = "Pantalón", Precio = 700 },
            new Producto { Nombre = "Zapatos", Precio = 1200 }
        };

        // Proyección en un tipo anónimo
        var productosConDescuento = productos
            .Select(p => new
            {
                p.Nombre,
                PrecioConDescuento = p.Precio * 0.9m
            });

        Console.WriteLine("Productos con descuento (tipo anónimo):");
        foreach (var producto in productosConDescuento)
        {
            Console.WriteLine($"{producto.Nombre}: ${producto.PrecioConDescuento}");
        }
    }
}

public class Producto
{
    public string Nombre { get; set; }
    public decimal Precio { get; set; }
}
```

---

### **4. Consultas avanzadas**

#### **a) Proyección múltiple con `join`:**
Combina dos colecciones relacionadas.
```csharp
var empleados = new List<Empleado>
{
    new Empleado { Id = 1, Nombre = "Juan" },
    new Empleado { Id = 2, Nombre = "Ana" }
};

var departamentos = new List<Departamento>
{
    new Departamento { EmpleadoId = 1, Nombre = "IT" },
    new Departamento { EmpleadoId = 2, Nombre = "RRHH" }
};

// Sintaxis de consulta
var consulta = from e in empleados
               join d in departamentos on e.Id equals d.EmpleadoId
               select new { e.Nombre, Departamento = d.Nombre };

foreach (var resultado in consulta)
{
    Console.WriteLine($"{resultado.Nombre} trabaja en {resultado.Departamento}");
}
```

#### **b) Métodos de agregación:**
Calcula valores como suma, promedio, máximo y mínimo.
```csharp
var precios = new[] { 100m, 200m, 300m };

decimal total = precios.Sum();
decimal promedio = precios.Average();

Console.WriteLine($"Total: {total}, Promedio: {promedio}");
```

---

### **5. Ventajas de LINQ**
1. **Legibilidad:** Sintaxis clara y declarativa.
2. **Versatilidad:** Compatible con bases de datos, colecciones en memoria, XML, y más.
3. **Seguridad de tipos:** Los errores se detectan en tiempo de compilación.
4. **Reutilización:** Es posible encadenar operaciones complejas fácilmente.

---
