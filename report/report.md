# Proyecto de Cohete Impulsado por Agua   
**Materia: Métodos Numéricos**  
**Universidad Autónoma Metropolitana**  
**Trimestre: [25I]**  
**Autores: [Sergio Felipe Gonzalez Cruz, Miguel Ángel Solares Velázquez, Alejandro Martinez Cortés]**  
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
11. [Modelación computacional en MATLAB](#10-modelación-computacional-en-matlab)  
12. [Comparación de resultados: Tracker vs Simulación](#11-comparación-de-resultados-tracker-vs-simulación)  
13. [Modelación físico-matemática-computacional](#12-modelación-físico-matemática-computacional)  
14. [Resultados alcanzados](#13-resultados-alcanzados)  
15. [Reflexión individual](#14-reflexión-individual)  
16. [Conclusiones generales](#15-conclusiones-generales)  
17. [Conclusiones individuales](#16-conclusiones-individuales)  
18. [Bibliografía](#17-bibliografía)

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
El cohete ha sido diseñado utilizando materiales reciclables, accesibles y ligeros, priorizando la funcionalidad, estabilidad y aerodinámica. La estructura principal está conformada por **dos botellas de plástico PET de 1.75 litros**, unidas por sus bocas para aumentar el volumen total. Esta modificación permite una mayor capacidad de almacenamiento de agua y aire comprimido, optimizando el empuje durante el lanzamiento.

La sección frontal cuenta con una **punta cónica de aluminio**, cuya forma aerodinámica minimiza la resistencia al avance. El cuerpo del cohete está recubierto con **cartulina blanca**, tanto por motivos estéticos como para mejorar su visibilidad en video durante las pruebas experimentales. Para garantizar la estabilidad en vuelo, se han incorporado **tres aletas simétricas** fabricadas con **papel ilustración**, dispuestas equidistantemente en la parte inferior del fuselaje.

<img width="739" height="1600" alt="image" src="https://github.com/user-attachments/assets/10119032-7d70-4a1d-8411-7ccc8b9af9a1" />
> _Título: "Imagen 6. Cohete armado."_  

### Lista de Materiales Utilizados

- 2 botellas plásticas PET de refresco (1.75 L cada una)
- 1 punta cónica de aluminio (para mejorar la aerodinámica)
- Cartulina blanca (recubrimiento externo del cuerpo del cohete)
- Papel ilustración (para la construcción de las aletas estabilizadoras)
- Cinta adhesiva resistente
- Tapón con válvula (para el sistema de presurización)
- Agua (como masa reactiva)
- Bomba de aire manual (para generar presión de lanzamiento)

<img width="723" height="357" alt="image" src="https://github.com/user-attachments/assets/28ae5006-e1dd-4df8-be6e-12e2079228f3" />
> _Título: "Imagen 7. Diagrama del cohete."_  


> **Nota**: El diseño cumple con las especificaciones del concurso: uso exclusivo de botellas no retornables de PET, sin componentes electrónicos ni materiales metálicos en zonas estructurales críticas.

## 8. Pruebas experimentales con Tracker

<img width="1361" height="616" alt="image" src="https://github.com/user-attachments/assets/231c4c72-5190-43b0-8a06-29c4906ca641" />
> _Título: "Imagen 8. Seguimiento del cohete en el software tracker."_


<img width="793" height="515" alt="image" src="https://github.com/user-attachments/assets/ba84e90b-93f5-4068-b58c-a3ec0dc10c1e" />
> _Título: "Imagen 9. Gráfica lineal obtenida en Tracker."_


<img width="794" height="518" alt="image" src="https://github.com/user-attachments/assets/08789c50-4dc2-42b1-b702-49d6f2291b80" />
> _Título: "Imagen 10. Gráfica parabólica obtenida en Tracker."_


<img width="768" height="1033" alt="image" src="https://github.com/user-attachments/assets/8996f049-d3a7-4b02-8e82-3833abd719c6" />
> _Título: "Tabla 5. Tabla de variables obtenida en Tracker."




## 9. Determinación de altura con modelo cinemático
Aplicando la ecuación del movimiento vertical uniformemente acelerado:

<img width="155" height="47" alt="image" src="https://github.com/user-attachments/assets/22de7335-cc56-4e74-bbd8-7b02b05b63d8" />


Con una velocidad inicial vertical de v0= 4.68 m/s (registros de la tabla) obtenemos lo siguiente:

<img width="223" height="54" alt="image" src="https://github.com/user-attachments/assets/cad5cc9a-cff7-4624-9d16-899d921d5d68" />


## 10. Análisis de video con variables físicas

- x(t): Al principio constante, por lo que no hay un movimiento horizontal. Después va a disminuir, ya que el objeto se mueve un poquito a la izquierda (por la toma del vídeo y la gráfica de puntos).
- y(t): En el punto y, definitivamente sube por un tiempo considerable.
- vx(t): Según los datos de la tabla, oscila entre 0 y negativo, por lo que hay un pequeño movimiento horizontal hacia la izquierda.
- vy(t): Comienza primero una subida, a lo que posteriormente, hay un decremento de esta velocidad en el eje.
- ax(t): Hay un ligero cambio de signo, lo que implica pequeños ajustes en aceleración horizontal.
- ay(t): Se mantiene cerca de valores negativos (de entre -7 a -15 m/s²), más altos de lo que en promedio se estaría esperando.
- K(t) (Energía cinética): Aumenta hasta un pico (cuando sube), luego disminuye cuando el objeto se detiene.
- Ug (Energía potencial gravitatoria): Aquí esta energía va disminuyendo con el paso del tiempo, ya que está depende de la altura alcanzada en el eje y. 

## 11. Modelación computacional en MATLAB

<img width="934" height="3136" alt="image" src="https://github.com/user-attachments/assets/7c02e3ab-e9d8-4f85-a566-fc93567b2044" />
> _Título: "Imagen 11. Valores obtenidos del modelado en Matlab."_

<img width="524" height="389" alt="image" src="https://github.com/user-attachments/assets/a7f03801-b7ba-45fb-9105-c5069049c449" />
> _Título: "Imagen 12. Gráficas obtenidas en Matlab."_



## 12. Comparación de resultados: Tracker vs Simulación

Al comparar los gráficos obtenidos con el programa Tracker y los producidos a través de la simulación en MATLAB, se notó una gran coincidencia en los resultados. En el gráfico que muestra la altura frente al tiempo, ambas fuentes presentan el mismo comportamiento parabólico hacia abajo, lo que indica que el cohete comienza a caer desde una altura máxima de aproximadamente 3. 2 metros. Los gráficos de velocidad también son coherentes, mostrando valores negativos que representan la caída del cohete, y MATLAB reproduce con precisión las variaciones que se ven en Tracker. 
En lo que respecta a la aceleración, ambas gráficas muestran cambios bruscos, debido al ruido que proviene del cálculo numérico de derivadas con datos discretos. Esto indica que la aceleración obtenida directamente de Tracker puede no ser completamente confiable, por lo que sería aconsejable usar un modelo ideal con aceleración constante para obtener análisis más precisos. 
Por último, los gráficos de energía cinética, potencial y total evidencian una buena conservación de energía en ambas plataformas. La energía potencial disminuye cuando el cohete desciende, mientras que la energía cinética aumenta; la energía mecánica total permanece bastante constante, con pequeñas oscilaciones que se pueden atribuir a errores en el experimento o a leves pérdidas no modeladas.

## 13. Modelación fisicomatemática-computacional

Esto se basa en el estudio del movimiento rectilíneo con aceleración constante bajo la gravedad, después de que el empuje inicial ha terminado. En este punto del vuelo, el cohete no recibe más fuerza de impulso, y su movimiento está determinado por la ecuación cinemática vertical:

<img width="180" height="53" alt="image" src="https://github.com/user-attachments/assets/70b78b3c-8c16-4513-b1ef-e50244f9cb43" />

donde y0 es la altura inicial, v0 es la velocidad vertical inicial (extraída de los datos de Tracker), g es la aceleración debida a la gravedad en el lugar (aproximadamente 9. 81 m/s^2), y t es el tiempo que ha pasado. 
Con la ayuda de MATLAB, se aplicó esta ecuación para imitar el movimiento del cohete en su etapa de descenso. Además, se calcularon y representaron gráficamente variables importantes como posición, velocidad, aceleración y las energías cinética y potencial, combinando así los principios de la física con los datos obtenidos experimentalmente en un modelo computarizado. Esta simulación permitió comprobar los resultados obtenidos con Tracker, ayudando a entender el comportamiento del sistema físico desde un enfoque tanto teórico como numérico.

<img width="441" height="382" alt="image" src="https://github.com/user-attachments/assets/e42d7f61-30dc-4419-880b-60cff819d5ea" />

<img width="690" height="1432" alt="image" src="https://github.com/user-attachments/assets/2062537a-bfd9-413b-8efb-83995b2fb5b6" />




## 14. Resultados alcanzados

Se determina que el cohete alcanzó una altura máxima cercana a 4.09 metros, siendo superior que la calculada analíticamente, comenzando con una fase de aceleración intensa que muestra que hubo un empuje activo (en este caso, por la presión). El análisis indica un comportamiento que se asemeja al movimiento parabólico, con una transición clara entre la subida impulsada y la caída libre. Las alteraciones en la aceleración sugieren que fuerzas variables actuaron durante el vuelo, posiblemente debido a la calidad del medio de video, considerando que se realiza una aproximación. La simulación en MATLAB logró reproducir la trayectoria observada en Tracker, lo que confirma tanto la recolección de datos como el modelo físico planteado. En general, los resultados demuestran una descripción precisa del movimiento y ayudan a entender las diferentes fases del vuelo del cohete.

## 15. Reflexión individual

[Sergio Felipe Gonzalez Cruz]

Como estudiante de Ingeniería Electrónica, este proyecto representó un desafío enriquecedor fuera de mi zona de especialidad. A pesar de no tener formación en diseño aeronáutico o mecánico, me vi obligado a integrar conocimientos de física, dinámica de fluidos, modelación matemática y análisis computacional. Pude comprender mejor cómo los principios abstractos que estudiamos en clase se manifiestan de forma tangible en un sistema real como un cohete de agua.
El uso del software Tracker y MATLAB me permitió fortalecer mi competencia en herramientas de análisis experimental y simulación, áreas fundamentales para cualquier ingeniero moderno. Además, el trabajo en equipo, la organización del repositorio en GitHub y la documentación técnica en Markdown me brindaron la oportunidad de aplicar buenas prácticas de ingeniería en un entorno colaborativo.
Este proyecto no solo reforzó mis habilidades técnicas, sino que también alimentó mi interés por la interdisciplinariedad entre la ingeniería mecánica, la electrónica y la simulación numérica, lo que sin duda enriquecerá mi formación profesional.


[Miguel Angel Solares Velazquez]

La presente actividad facilitó la comprensión práctica de los principios físicos involucrados, especialmente la tercera ley de Newton, en un sistema dinámico real como lo es un cohete propulsado por agua. A través de esta experiencia, fue posible integrar conocimientos de física, diseño técnico y análisis computacional para el desarrollo de un prototipo funcional. El empleo de herramientas especializadas como Tracker y MATLAB permitió visualizar y modelar el movimiento del cohete, fortaleciendo así la comprensión de conceptos fundamentales de cinemática y dinámica, los cuales previamente se habían abordado de manera exclusivamente teórica. Ademas esta actividad contribuyó al desarrollo de habilidades precisas en la recolección de datos y en el diseño estructural, competencias esenciales para la ejecución de proyectos en el ámbito científico y de ingeniería.

[Alejandro Martinez Cortés]

En lo personal, la actividad me dio la oportunidad de entender de manera práctica cómo se utiliza la física para analizar movimientos reales, en particular el movimiento vertical con aceleración variable. Aprendí a usar Tracker para recoger datos experimentales y compararlos con un modelo en MATLAB, lo que me ayudó a reforzar ideas como velocidad, aceleración, energía cinética y trayectoria. También me quedó claro que los modelos teóricos pueden coincidir bastante con la realidad, pero siempre hay elementos como errores de medición o fuerzas no consideradas (como la resistencia del aire o la calidad del vídeo a analizar) que influyen en los resultados.

## 16. Conclusiones generales

La realización de este proyecto permitió aplicar de manera integrada diversos conocimientos adquiridos en el área de métodos numéricos, física y modelación matemática. Desde el diseño y construcción del cohete, hasta la recolección de datos experimentales y su posterior análisis computacional, se logró una experiencia formativa completa que fomentó tanto el pensamiento analítico como la creatividad.
El uso de herramientas como Tracker y MATLAB facilitó la validación empírica del modelo físico propuesto, permitiendo identificar desviaciones, errores sistemáticos y limitaciones del experimento. Además, el proceso de documentación técnica y trabajo en equipo contribuyó a reforzar habilidades profesionales clave en la ingeniería actual.
En síntesis, el proyecto del cohete impulsado por agua no solo cumplió con los objetivos académicos, sino que se convirtió en una oportunidad valiosa para desarrollar habilidades transversales que serán de utilidad en futuros desafíos profesionales.

## 17. Conclusiones individuales

[Sergio Felipe Gonzalez Cruz]
- Aprendí a traducir principios físicos y matemáticos en modelos computacionales que pueden ser contrastados con datos experimentales reales.
- Mejoré mi capacidad para documentar proyectos de forma clara y profesional utilizando herramientas como Markdown y GitHub.
- Reafirmé la importancia de considerar restricciones prácticas y normativas de diseño al proponer soluciones técnicas.
- Comprendí que el pensamiento interdisciplinario es esencial para abordar problemas complejos incluso fuera de mi campo directo de estudio.

[Miguel Angel Solares Velazquez]

La construcción y el análisis del cohete impulsado por chorro de agua no solo consolidaron los conocimientos teóricos de física y modelación computacional, sino que también promovieron el desarrollo de la creatividad, la capacidad para la resolución sistemática de problemas y el trabajo metódico. La integración de teoría, práctica y tecnología en esta actividad generó una experiencia educativa integral, evidenciando cómo el aprendizaje experimental constituye una herramienta eficaz para profundizar en la comprensión de fenómenos físicos.

[Alejandro Martinez Cortés]

Finalmente, considero que esta actividad fue muy valiosa porque me mostró que la física va más allá de las ecuaciones, pudiendo ser utilizada para comprender cosas de la vida real, que no únicamente se quedan en la parte teórica. Asimismo, el uso de programas como Tracker y MATLAB me ayudó no solo al dominio de software (importante para mi carrera), sino para hacer una documentación correcta, algo que en trabajos de investigación continuaré haciendo. 

## 18. Bibliografía

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

