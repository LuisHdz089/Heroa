# Proyecto: Compilador Heroa (Lenguajes y Autómatas I)

Este proyecto consiste en el diseño e implementación de un **Analizador Léxico y Sintáctico** robusto, desarrollado para la carrera de **Ingeniería en Sistemas Computacionales**. El sistema no solo valida la gramática del lenguaje HEROA, sino que es capaz de recuperarse ante fallos estructurales para continuar el análisis.

## 📊 Caracterización de la Asignatura
El desarrollo de este sistema se basa en los siguientes pilares académicos:
* **Modelado:** Aplicación de conceptos, técnicas y herramientas orientadas al modelado de soluciones computacionales.
* **Eficiencia:** Desarrollo de aplicaciones eficientes en el uso de recursos y procesamiento de texto.
* **Formalidad:** Uso de representaciones formales (BNF) para el procesamiento e implementación de lenguajes.

## 🚀 Competencias y Características Técnicas
* **Análisis Léxico:** Identificación de componentes léxicos y patrones con reporte preciso de **línea y columna** para cada token.
* **Análisis Sintáctico:** Implementación de gramáticas libres de contexto mediante JavaCC.
* **Sincronización Inteligente (Panic Mode Recovery):** El compilador utiliza un sistema de balanceo de llaves y búsqueda de anclas (delimitadores) para recuperarse de errores sintácticos. Esto evita el "Efecto Cascada", permitiendo detectar múltiples errores reales en una sola ejecución.
* **Gestión de Bloques Huérfanos:** Incluye reglas específicas para detectar y reportar estructuras condicionales (`sino`, `sino_si`) que no poseen un bloque `si` previo.

## 🛠️ Especificaciones del Lenguaje
El compilador procesa una gramática completa que incluye:

1. **Declaraciones:**
   - Simple: `variable entero x;`
   - Con Asignación: `variable decimal PI = 3.14;`
   - Múltiple: `variable booleano b1, b2;`
2. **Estructuras de Control:** `si-sino`, `mientras`, `para` y `hacer-mientras`.
3. **Estructuras de Datos:** Soporte para **Arreglos** y **Matrices** bidimensionales.
4. **Tipos de Datos:** `entero`, `decimal`, `caracter`, `booleano`, `cadena`.

## 💻 Instrucciones de Uso

### Requisitos
* **JDK** (Java Development Kit) 8 o superior.
* **JavaCC** (Java Compiler Compiler).

### Compilación y Ejecución
1. Generar el analizador a partir del archivo gramatical:
   ```bash
   javacc analizador.jj
2. Compilar las clases Java generadas:
    ```bash
   javac *. java
3. Ejecutar el programa utilizando un archivo de entrada (**ej. prueba.txt**)
   ```bash
   java Heroa