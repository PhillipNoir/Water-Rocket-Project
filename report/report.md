# Proyecto de Cohete Impulsado por Agua   
**Materia: Métodos Numéricos**  
**Universidad Autónoma Metropolitana**  
**Trimestre: [25I]**  
**Autores: [Sergio Felipe Gonzalez Cruz, Miguel Ángel Solares Velázquez]**  
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

### Historia Breve de los Cohetes

El concepto de propulsión por reacción tiene raíces profundas en la historia de la humanidad. Aunque los cohetes modernos son productos de la física del siglo XX, sus principios fundamentales se conocen desde hace siglos.

#### Orígenes tempranos

El primer uso documentado de cohetes data del siglo XIII en China, donde se empleaban tubos de bambú rellenos con pólvora negra como armas militares rudimentarias (Sutton y Biblarz, 2017). Estas primeras versiones de cohetes eran esencialmente fuegos artificiales modificados, aprovechando la expansión de gases para generar empuje. Durante los siglos siguientes, el conocimiento sobre estas armas se difundió a través de Oriente Medio y Europa, siendo utilizadas en conflictos como la Guerra de los Cien Años.

![image](https://github.com/user-attachments/assets/ee43714c-b1f2-4463-99b1-b63e438870e7)
> _Título: "Imagen 1. Uso militar temprano de cohetes en la antigua China"_  

#### La era moderna: fundamentos científicos

Fue hasta el siglo XVII que comenzaron a formularse principios científicos que explican el funcionamiento de los cohetes. Isaac Newton enunció sus leyes del movimiento en 1687, estableciendo formalmente la **tercera ley de Newton**, que es el principio fundamental detrás de la propulsión de cohetes: *"a toda acción le corresponde una reacción de igual magnitud y en sentido opuesto" (Newton, 1687).

Sin embargo, el desarrollo práctico de los cohetes como vehículos de propulsión científica no ocurrió sino hasta el siglo XX, con los trabajos pioneros de científicos como:

- **Konstantin Tsiolkovsky** (Rusia), quien enunció en 1903 la ecuación del cohete y teorizó sobre el uso de cohetes para viajes espaciales (Tsiolkovsky, 1903).
- **Robert Goddard** (EE.UU.), considerado el "padre del cohete moderno", quien en 1926 lanzó el primer cohete de combustible líquido exitoso (Goddard, 1926).
- **Hermann Oberth** (Alemania), uno de los primeros en estudiar científicamente el uso de cohetes para alcanzar el espacio.

> _Título: "Tabla 1. Contribuciones clave al desarrollo de la cohetería moderna"_

| Científico             | País       | Aporte principal                            | Año destacado |
|------------------------|------------|----------------------------------------------|---------------|
| Konstantin Tsiolkovsky| Rusia      | Ecuación del cohete, viajes espaciales       | 1903          |
| Robert Goddard         | EE.UU.     | Primer cohete de combustible líquido         | 1926          |
| Hermann Oberth         | Alemania   | Fomento de la astronáutica                   | 1923          |

#### Segunda Guerra Mundial y carrera espacial

Durante la Segunda Guerra Mundial, Alemania desarrolló el **V-2**, el primer cohete balístico de largo alcance y el primero en alcanzar el espacio suborbital (más de 100 km de altitud) (Ordway y Sharpe, 1979). Aunque fue un arma devastadora, sentó las bases para la ingeniería aeroespacial moderna.

Al finalizar la guerra, tanto Estados Unidos como la Unión Soviética reclutaron a científicos alemanes (como Wernher von Braun) para desarrollar sus propios programas espaciales, lo que dio inicio a la **carrera espacial** durante la Guerra Fría.

![image](https://github.com/user-attachments/assets/62188a0d-578b-42c8-a352-14fd623f5e23)
> _Título: "Imagen 2. Cohete V-2: precursor tecnológico del viaje espacial"_

Durante las décadas siguientes, se lograron hitos como:

- **Sputnik I** (1957): primer satélite artificial (URSS)
- **Vostok I** (1961): primer humano en el espacio, Yuri Gagarin (URSS)
- **Apolo 11** (1969): alunizaje del ser humano, Neil Armstrong (EE.UU.)

![image](https://github.com/user-attachments/assets/6b51df62-2b0b-4815-bca8-cb4fc6ec2247)
> _Título: "Imagen 3. Saturno V, uno de los cohetes más potentes jamás construidos"_

#### Era contemporánea

En el siglo XXI, el enfoque se ha desplazado hacia la reutilización, eficiencia y exploración interplanetaria. Empresas como **SpaceX**, **Blue Origin**, **Rocket Lab** y **Arianespace** están redefiniendo la industria espacial, con avances como:

- Cohetes reutilizables (Falcon 9)
- Motores de metano (Raptor)
- Turismo espacial (New Shepard)
- Misiones científicas y comerciales a Marte, la Luna y asteroides.

> _Título: "Tabla 2. Clasificación moderna de cohetes por propósito"_

| Nombre          | Tipo           | Propósito principal     | Reutilizable |
|-----------------|----------------|--------------------------|--------------|
| Falcon 9        | Orbital        | Lanzamiento satelital    | Sí           |
| Ariane 5        | Orbital        | Ciencia/comercial        | No           |
| New Shepard     | Suborbital     | Turismo espacial         | Sí           |
| Electron        | Orbital ligero | Microsatélites           | Parcialmente |


## 5. Funcionamiento de un cohete de agua y elementos requeridos

### Principio de funcionamiento

Un cohete de agua funciona bajo el mismo principio de **acción y reacción** descrito por la tercera ley de Newton. La botella actúa como una cámara de presión parcialmente llena de agua. Al presurizar el aire dentro de la botella y luego liberar su contenido por una boquilla estrecha, el agua es expulsada violentamente, generando un empuje que impulsa la botella en la dirección opuesta (Newton, 1687).

La propulsión es predominantemente **impulsiva** y de **corta duración**, generando una aceleración inicial considerable. Este tipo de cohete se categoriza como un **sistema de propulsión no térmica**, ya que no utiliza combustión, sino compresión neumática y la expulsión de masa líquida.

![image](https://github.com/user-attachments/assets/dba7b430-80cc-41be-8254-a048ed9f8bd4)
> _Título: "Imagen 4. Funcionamiento de un cohete de agua"_  

### Componentes del cohete de agua

A continuación se describen los elementos esenciales para la construcción de un cohete de agua funcional:

| Componente             | Función principal                                            |
|------------------------|--------------------------------------------------------------|
| Botella plástica PET   | Cuerpo del cohete y cámara de presión                        |
| Agua                   | Masa reactiva expulsada para generar empuje                  |
| Aire comprimido        | Fuente de energía almacenada (mediante una bomba manual)     |
| Boquilla (tapa o adaptador) | Controla el flujo de salida del agua, optimizando empuje    |
| Aletas                 | Estabilización durante el vuelo                              |
| Nariz o cono frontal   | Mejora la aerodinámica y reduce el arrastre                  |
| Plataforma de lanzamiento | Sujeta el cohete y permite presurización segura             |
| Sistema de liberación  | Mecanismo para activar el despegue de forma controlada       |

> _Título: "Tabla 3. Componentes y funciones del cohete de agua"_ 
> Fuente: elaboración propia con base en (Schlichting y Truckenbrodt, 2000), (NASA, 2019)

### Ciclo de operación

1. **Carga del agua**: Se llena entre 30%–50% de la capacidad del cuerpo (1-2 L es común).
2. **Presurización**: Se inyecta aire a través de una válvula con bomba manual o compresor.
3. **Lanzamiento**: Se libera el seguro de la plataforma. La presión del aire expulsa el agua.
4. **Ascenso**: El cohete se eleva hasta alcanzar su apogeo (pico de trayectoria).
5. **Caída libre**: El cohete desciende, pudiendo o no incluir paracaídas de recuperación.

![image](https://github.com/user-attachments/assets/4dc6c508-3eca-4b13-bb59-0622ae8b8d65)
> _Título: "Imagen 5. Secuencia operativa típica de un cohete de agua escolar"_  


### Variables críticas en el diseño

- **Relación agua/aire**: Influye directamente en el impulso específico.
- **Tamaño de boquilla**: Controla el caudal de salida; afecta empuje y duración.
- **Masa total y forma**: Determinan aceleración, arrastre y estabilidad.
- **Presión máxima**: Limitada por la resistencia del PET (normalmente <100 psi).

> _Título: "Tabla 4. Influencia de parámetros de diseño sobre el rendimiento"
> _Fuente: adaptación de (Turner, 2008)_

| Parámetro                | Aumento →                 | Disminución →            |
|--------------------------|---------------------------|---------------------------|
| Porcentaje de agua       | Mayor empuje inicial      | Menor tiempo de vuelo     |
| Tamaño de boquilla       | Mayor caudal, menor duración | Menor empuje total    |
| Masa total               | Mayor inercia, menor altura | Mayor aceleración     |
| Presión interna          | Mayor empuje               | Menor rendimiento         |


## 6. Principios físicos involucrados

El funcionamiento de un cohete impulsado por agua se explica mediante diversos principios fundamentales de la física clásica, especialmente de la **mecánica newtoniana**, la **hidrodinámica** y la **termodinámica**.

### Tercera Ley de Newton: Acción y reacción

La base del movimiento del cohete de agua es la **tercera ley de Newton**, que establece que a toda acción corresponde una reacción de igual magnitud y en sentido opuesto. En este caso, la **acción** es la expulsión del agua por la boquilla del cohete y la **reacción** es el impulso que recibe el cohete en dirección contraria (Newton, 1687).

![image](https://github.com/user-attachments/assets/3b1ec471-b427-4f60-88b4-e03e1f1ef15e)


### Conservación de la cantidad de movimiento

Durante la expulsión del fluido, se conserva la **cantidad de movimiento lineal (momento lineal)** del sistema cohete + agua. La expulsión de masa (agua) con una cierta velocidad genera un cambio igual y opuesto en la velocidad del cohete (Halliday, Resnick & Walker, 2014).

![image](https://github.com/user-attachments/assets/2e6cf209-1a76-4d27-a795-193132b8410e)


Este intercambio impulsa el cohete hacia arriba y permite modelar su comportamiento usando ecuaciones de impulso variable.


### Ley de los gases ideales y presión

El cohete se presuriza al inyectar aire comprimido dentro de la botella. Este aire actúa como un gas ideal y, al expandirse, transfiere energía al agua. Según la **ley de los gases ideales**:

![image](https://github.com/user-attachments/assets/f2cbce00-06fd-46db-8a7e-43146dda3cf4)


donde una disminución súbita en volumen (al liberar el agua) provoca un aumento en la presión y, por tanto, en la energía cinética del fluido expulsado (Young & Freedman, 2019).

### Energía cinética y potencial

Durante el ascenso, el cohete convierte parte de la energía liberada en **energía cinética** y, posteriormente, en **energía potencial gravitatoria**:

![image](https://github.com/user-attachments/assets/4bd5051b-1ad8-4665-8584-bbebe9eb04a2)


La altura máxima (apogeo) es alcanzada cuando la velocidad vertical se reduce a cero y toda la energía se encuentra en forma de \( U_g \) (Tipler & Mosca, 2008).


### Resistencia del aire y fuerzas en vuelo

Durante el vuelo, el cohete también está sujeto a **resistencia del aire (arrastre)**, la cual se modela comúnmente como:

![image](https://github.com/user-attachments/assets/731032c2-f0b6-4be9-b7c4-d041fabe3b8a)


Donde:
- C_d = coeficiente de arrastre (≈ 0.75 a 1.0 para cohetes caseros)
- rho = densidad del aire
- A = área frontal del cohete
- v = velocidad del cohete

Este efecto debe considerarse para un modelo computacional más realista (Turner, 2008).


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

Goddard, R. H. (1926). *A Method of Reaching Extreme Altitudes*. Smithsonian Institution.

Halliday, D., Resnick, R., & Walker, J. (2014). *Fundamentals of Physics* (10th ed.). Wiley.

MathWorks. (2023). *MATLAB (R2023a)* [Software]. https://www.mathworks.com/products/matlab.html

Newton, I. (1687). *Philosophiæ Naturalis Principia Mathematica*.

Ordway, F. I., & Sharpe, M. R. (1979). *The Rocket Team*. Thomas Y. Crowell.

Schlichting, H., & Truckenbrodt, E. (2000). *Aerodynamics of the Water Rocket*. Springer.

Serway, R. A., & Jewett, J. W. (2013). *Physics for Scientists and Engineers* (9th ed.). Cengage Learning.

Sutton, G. P., & Biblarz, O. (2017). *Rocket Propulsion Elements* (9th ed.). Wiley.

Tipler, P. A., & Mosca, G. (2008). *Physics for Scientists and Engineers* (6th ed.). W. H. Freeman.

Turner, M. J. (2008). *Rocket and Spacecraft Propulsion: Principles, Practice and New Developments*. Springer.

Tsiolkovsky, K. E. (1903). *The Exploration of Cosmic Space by Means of Reaction Devices*

Young, H. D., & Freedman, R. A. (2019). *University Physics with Modern Physics* (15th ed.). Pearson.

