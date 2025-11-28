--Lenguaje Natural a Ensamblador-- Convertir lenguaje natural a un lenguaje ensamblador basico simplificando las instrucciones de alto nivel a operaciones fundamentales de la CPU.

          Materia: Programacion de Sistemas Base 2
      Institución: Universidad Autonoma de Tamaulipas
        Semestre: Noveno Semestre de 2025 Grupo: J
          Profesor: Muñoz Quintero Dante Adolfo
                  Integrantes del Equipo:
                    Ruiz Gómez Andres
                 Gonzales Flores Juan Diego
                Fornue Rivera Joseph Stefano
                
La organización de los archivos principales es la siguiente: -Traductor.py: Script de pre-procesamiento que convierte el texto libre (Lenguaje Natural) en código intermedio (Ensamblador) utilizando expresiones regulares. -mainEnsamblador.py: Punto de entrada principal. Ejecuta el análisis léxico, sintáctico y semántico sobre el código ensamblador generado. -Ensamblador.g4: Gramática definida en ANTLR4 que establece las reglas léxicas y sintácticas del lenguaje ensamblador. -AnalizadorSemantico.py: Módulo que valida la lógica del programa (etiquetas duplicadas, saltos inválidos, división por cero, registros correctos). -EntradaNatural.txt: Archivo de texto donde el usuario escribe sus algoritmos en español. -EnsambladorGenerado.txt: Archivo de salida que contiene el código traducido, listo para ser analizado. -- Archivos Generados por ANTLR -- -EnsambladorLexer.py -EnsambladorParser.py -EnsambladorListener.py

REQUISITOS Y DEPENDENCIAS

Para ejecutar este proyecto correctamente, es necesario contar con el siguiente software y librerias:

1.- Python 3.8 superior: El proyecto esta desarrollado integramente en Python. 2.- ANTLR4 Python Runtime: Necesaria para que Python pueda interpretar los archivos generados por la gramatica.
pip install antlr4-python3-runtime
3.- Librerias Estandar: Se utiliza re (Expresiones Regulares) y sys, las cuales ya vienen incluidas en Python.

INSTRUCCIONES DE COMPILACION Y EJECUCIÓN

Paso 1: Definir el Algoritmo Edite el archivo EntradaNatural.txt y escriba sus instrucciones en español.

-Ejemplo: "Suma 5 y 3 y guarda el resultado en registro B".
Paso 2: Traducción (Lenguaje Natural --> Ensamblador) Ejecute el traductor para generar el codigo intermedio.

python Traductor.py
