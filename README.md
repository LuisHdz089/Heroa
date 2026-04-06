# Proyecto: Compilador Heroa (Lenguajes y Autómatas I)

Este proyecto consiste en el diseño e implementación de un **Analizador Léxico y Sintáctico** desarrollado para la carrera de **Ingeniería en Sistemas Computacionales**.

## 📊 Caracterización de la Asignatura
El desarrollo de este sistema se basa en los siguientes pilares académicos:
* **Modelado:** Aplicación de conceptos, técnicas y herramientas orientadas al modelado de soluciones computacionales.
* **Eficiencia:** Desarrollo de aplicaciones eficientes en el uso de recursos y restricciones de desempeño.
* **Formalidad:** Uso de representaciones formales para el procesamiento e implementación de lenguajes.

## 🚀 Competencias Desarrolladas
* **Análisis Léxico:** Identificación de componentes léxicos, patrones y lexemas.
* **Análisis Sintáctico:** Implementación de gramáticas libres de contexto y árboles de derivación.
* **Uso de Estándares:** Implementación sujeta a estándares de desarrollo de software para incentivar la productividad.

## 🛠️ Especificaciones del Lenguaje
El compilador es capaz de procesar las siguientes estructuras de **Declaración de Variables**:

1. **Declaración Simple:** `variable <tipo> <id>;`
2. **Declaración con Asignación:** `variable <tipo> <id> = <valor>;`
3. **Declaración Múltiple:** Permite declarar 2 o más variables en una sola línea: `variable <tipo> <id1>, <id2>;`

### Tipos de Datos Soportados
* `entero`, `decimal`, `caracter`, `booleano`, `cadena`.

## 💻 Instrucciones de Uso

### Requisitos
* JDK (Java Development Kit).
* JavaCC (Java Compiler Compiler).

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