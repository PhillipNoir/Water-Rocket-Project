# Proyecto de Cohete Impulsado por Agua   
**Materia: Métodos Numéricos**  
**Universidad Autónoma Metropolitana**  
**Trimestre: [25I]**  
**Autores: [Sergio Felipe Gonzalez Cruz]**  
**Profesor: [José Luis Nava Sanchez]**  
**Fecha: [26 de junio de 2025]**

---

## Índice

1. [Resumen](#1-Resumen)
2. [Introducción](#2-Introducción)
3. [Objetivos](#3-Objetivos)
4. [Investigación sobre cohetes y aplicaciones modernas](#2-investigación-sobre-cohetes-y-aplicaciones-modernas)  
5. [Funcionamiento de un cohete de agua y elementos requeridos](#3-funcionamiento-de-un-cohete-de-agua-y-elementos-requeridos)  
6. [Principios físicos involucrados](#4-principios-físicos-involucrados)  
7. [Propuesta de construcción y lista de materiales](#5-propuesta-de-construcción-y-lista-de-materiales)  
8. [Pruebas experimentales con Tracker](#6-pruebas-experimentales-con-tracker)  
9. [Determinación de altura con modelo cinemático](#7-determinación-de-altura-con-modelo-cinemático)  
10. [Análisis de video con variables físicas](#8-análisis-de-video-con-variables-físicas)  
11. [Gráficas obtenidas con Tracker](#9-gráficas-obtenidas-con-tracker)  
12. [Modelación computacional en MATLAB](#10-modelación-computacional-en-matlab)  
13. [Comparación de resultados: Tracker vs Simulación](#11-comparación-de-resultados-tracker-vs-simulación)  
14. [Modelación físico-matemática-computacional](#12-modelación-físico-matemática-computacional)  
15. [Resultados alcanzados](#13-resultados-alcanzados)  
16. [Reflexión individual](#14-reflexión-individual)  
17. [Conclusiones generales](#15-conclusiones-generales)  
18. [Conclusiones individuales](#16-conclusiones-individuales)  
19. [Bibliografía](#17-bibliografía)

---

## 1. Resumen

El presente documento expone el desarrollo completo de un proyecto de diseño, construcción, lanzamiento y análisis de un cohete impulsado por agua. Este tipo de sistema representa una versión simplificada, segura y funcional de un cohete real, permitiendo explorar principios fundamentales de la física como la ley de acción y reacción, la conservación de la cantidad de movimiento, la dinámica de fluidos, y el análisis energético del movimiento.

La estructura del cohete fue construida a partir de una botella plástica presurizada con aire, conteniendo un volumen de agua que, al ser expulsado, genera el empuje necesario para el despegue. Se realizaron pruebas experimentales de lanzamiento, registradas en video para su posterior análisis mediante el software Tracker. A partir de estos datos se extrajeron variables cinemáticas clave (posición, velocidad, aceleración, energía cinética, energía potencial gravitatoria y energía mecánica total) que permitieron describir cuantitativamente la trayectoria del cohete.

Se construyó un modelo físico-matemático del sistema, considerando las fuerzas actuantes durante las diferentes fases del vuelo, y se implementó una simulación computacional en MATLAB para comparar los resultados teóricos con los experimentales. Este enfoque permitió validar el modelo propuesto, identificar fuentes de error y obtener un marco integral del comportamiento dinámico del cohete.

El proyecto se desarrolló con fines educativos, permitiendo a los estudiantes aplicar conceptos de física y métodos numéricos en un contexto experimental real. Además, fomenta competencias de análisis crítico, trabajo en equipo, documentación técnica y uso de herramientas de simulación, contribuyendo al desarrollo profesional en el ámbito de la ingeniería.

**Palabras clave**: Cohete de agua, tercera ley de Newton, análisis cinemático, Tracker, MATLAB, modelación computacional.

## 2. Introducción

El estudio del movimiento de cuerpos propulsados constituye una base fundamental en diversas ramas de la ingeniería y la física aplicada. Dentro de este marco, los cohetes representan sistemas dinámicos complejos cuya comprensión implica el dominio de múltiples disciplinas: mecánica clásica, dinámica de fluidos, termodinámica y métodos numéricos (Tipler & Mosca, 2008).

En este contexto, el cohete impulsado por agua se posiciona como una herramienta pedagógica eficaz para modelar y analizar fenómenos físicos reales mediante recursos accesibles y seguros. Este tipo de cohete opera bajo el principio de acción y reacción enunciado por la tercera ley de Newton, donde el fluido expulsado genera una fuerza neta que impulsa el sistema en dirección opuesta (Serway & Jewett, 2013).

El presente proyecto consiste en el diseño, construcción, lanzamiento y análisis de un cohete propulsado por un chorro de agua a presión, empleando una botella plástica como estructura principal. A nivel experimental, el análisis cinemático del vuelo será realizado mediante el software Tracker, el cual permite obtener variables como posición, velocidad y aceleración en función del tiempo a partir de registros de video (Brown, 2023).

Posteriormente, se desarrollará un modelo físico-matemático del sistema, que será implementado computacionalmente en MATLAB para simular el comportamiento del cohete, permitiendo una comparación entre los datos experimentales y los resultados obtenidos numéricamente (MathWorks, 2023).

Desde el punto de vista educativo, esta actividad busca consolidar la aplicación de los métodos numéricos en la resolución de problemas físicos reales, fomentar el trabajo colaborativo, y desarrollar competencias en la modelación y análisis de sistemas dinámicos.

## 3. Objetivos del Proyecto

### Objetivo General

Diseñar, construir, lanzar y analizar experimentalmente un cohete impulsado por agua, integrando herramientas de medición cinemática y modelación computacional para comprender su comportamiento físico-dinámico, validando los resultados obtenidos mediante simulación numérica con MATLAB y análisis experimental con Tracker.

### Objetivos Específicos

- Investigar los fundamentos históricos, científicos y tecnológicos relacionados con los cohetes, incluyendo sus aplicaciones en la era moderna.
- Comprender y explicar los principios físicos involucrados en el funcionamiento de un cohete impulsado por agua, incluyendo las leyes de Newton, el principio de conservación de la cantidad de movimiento, la presión de fluidos y el análisis energético.
- Proponer y construir un modelo físico funcional de un cohete de agua utilizando materiales accesibles y seguros.
- Registrar lanzamientos experimentales del cohete mediante video para su posterior análisis cinemático utilizando el software Tracker.
- Determinar experimentalmente variables de movimiento como posición, velocidad, aceleración y energía mecánica en función del tiempo.
- Desarrollar un modelo físico-matemático del movimiento del cohete y simularlo en MATLAB para comparar los resultados con los obtenidos empíricamente.
- Evaluar y discutir las diferencias entre los modelos teóricos y experimentales, identificando fuentes de error y limitaciones del sistema.
- Documentar el proceso completo del proyecto de forma técnica y estructurada, integrando conocimientos de física, métodos numéricos y herramientas de análisis computacional.


## 4. Investigación sobre cohetes y aplicaciones modernas
...

## 5. Funcionamiento de un cohete de agua y elementos requeridos
...

## 6. Principios físicos involucrados
...

## 7. Propuesta de construcción y lista de materiales
...

## 8. Pruebas experimentales con Tracker
...

## 9. Determinación de altura con modelo cinemático
...

## 10. Análisis de video con variables físicas
- Posición: `x`, `y`
- Velocidad: `vx`, `vy`
- Aceleración: `ax`, `ay`
- Energía cinética: `K`
- Energía potencial gravitacional: `Ug`

## 11. Gráficas obtenidas con Tracker
...

## 12. Modelación computacional en MATLAB
...

## 13. Comparación de resultados: Tracker vs Simulación
...

## 14. Modelación físico-matemática-computacional
...

## 15. Resultados alcanzados
...

## 16. Reflexión individual
...

## 17. Conclusiones generales
...

## 18. Conclusiones individuales
...

## 19. Bibliografía

Brown, D. (2023). *Tracker Video Analysis and Modeling Tool* (Versión 6.1.5) [Software]. Open Source Physics. https://physlets.org/tracker/

MathWorks. (2023). *MATLAB (R2023a)* [Software]. https://www.mathworks.com/products/matlab.html

Serway, R. A., & Jewett, J. W. (2013). *Physics for Scientists and Engineers* (9th ed.). Cengage Learning.

Tipler, P. A., & Mosca, G. (2008). *Physics for Scientists and Engineers* (6th ed.). W. H. Freeman.

