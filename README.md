# Lab-GSR
1. Introducción

La respuesta galvánica cutánea (GSR) es una señal fisiológica que mide los cambios en la conductancia eléctrica de la piel. Estos cambios están relacionados con la actividad del sistema nervioso simpático, el cual se activa en situaciones de estrés, concentración o emoción.
 
Cuando una persona experimenta estrés o realiza una tarea que requiere esfuerzo mental, aumenta la actividad de las glándulas sudoríparas. Esto provoca que la piel conduzca mejor la electricidad, lo que se refleja en un aumento de la señal GSR.

En esta práctica se diseñó e implementó un dispositivo vestible para medir la GSR en tiempo real y estimar el nivel de estrés durante la realización de tareas cognitivas.

2. Objetivos
   
2.1 Objetivo General

- Desarrollar un sistema vestible que permita medir el nivel de estrés a partir de la respuesta galvánica cutánea.

2.2 Objetivos Específicos

- Identificar las partes principales de la señal GSR (nivel basal y respuestas rápidas).

- Diseñar un circuito seguro para medir la señal en una persona.

- Visualizar la señal en tiempo real.

- Implementar transmisión inalámbrica.

- Evaluar la señal durante tareas que requieran concentración.

  

3. Procedimiento

   
3.1 Parte A 


- Revisión teórica

Se investigó qué es la actividad electrodérmica y cómo se relaciona con el estrés. Se encontró que la señal GSR tiene dos componentes:

Componente tónica: nivel basal o promedio de la señal.

Componente fásica: aumentos rápidos ante estímulos.

Se confirmó que la GSR es un indicador indirecto de la activación del sistema nervioso simpático.

- Seguridad eléctrica

Para garantizar la seguridad del sujeto, se limitó la corriente a menos de 1 mA.

Se utilizó una fuente de 5 V y una resistencia de 68 kΩ.

Aplicando la Ley de Ohm:

I = V / R
I = 5V / 68000Ω
I = 73.5 µA

Este valor es mucho menor a 1 mA, por lo que el sistema es seguro.

-  Diseño del dispositivo

El sistema estuvo compuesto por:

Dos laminas de aluminio

Una resistencia de 68 kΩ.

Un condensador de 1 µF.

ESP para leer la señal.

Computador.

Los electrodos se colocaron en los dedos porque allí hay mayor cantidad de glándulas sudoríparas, lo que mejora la medición.

<img width="1150" height="677" alt="image" src="https://github.com/user-attachments/assets/672b7770-1bad-4fec-a070-8e0260bcdbd5" />


3.2 Parte B 



-  Medición en tiempo real

Se armó el circuito en protoboard y se visualizó la señal usando el Serial Plotter.
Se probó el sistema en diferentes situaciones: En reposo, caminando y escribiendo
Se observó que el movimiento genera ruido en la señal.

- Prueba de respiración profunda

El sujeto realizó una inspiración profunda y luego exhaló lentamente.

Donde se observó: Un aumento rápido en la señal, un regreso lento al valor inicial.

Con los valores máximos y mínimos se definieron tres niveles: Estrés bajo, estrés moderado, estrés alto

- Transmisión inalámbrica

Se utilizo el wifi para enviar los datos de forma inalámbrica.
En esta etapa, el sistema mostraba la señal completa y un mensaje indicando el nivel de estrés según los umbrales definidos.


3.3 Parte C 

Se pidió al sujeto que resolviera un pequeño examen mientras usaba el dispositivo.

Durante la prueba se observó: Aumento del nivel basal, más respuestas rápidas en la señal, clasificación frecuente en estrés moderado y alto.

Esto demuestra que la carga mental influye en la activación del sistema nervioso simpático.

<img width="1600" height="800" alt="image" src="https://github.com/user-attachments/assets/68487fb2-d5a7-4f97-80b6-3115d9b1a8ec" />

4. Análisis de Resultados

   
-  Respiración en reposo vs tarea cognitiva

En reposo:

Señal estable.

Pocas variaciones.

Nivel basal constante.

Durante la tarea:

Mayor variación en la señal.

Más respuestas rápidas.

Incremento del nivel promedio.

Esto confirma que la concentración y el esfuerzo mental aumentan la activación simpática.


5. Preguntas de Discusión
Pregunta 1: ¿Por qué una inspiración profunda aumenta la GSR?

Porque activa el sistema nervioso simpático, lo que aumenta la actividad de las glándulas sudoríparas. Esto hace que la piel conduzca mejor la electricidad y la señal aumente.

Pregunta 2: Ventajas y desventajas de usar la GSR como indicador de estrés

Ventajas

Fácil de medir.

No invasiva.

Económica.

Sensible a cambios fisiológicos.

Desventajas

No mide directamente el estrés psicológico.

Puede verse afectada por factores externos.

Varía entre personas.

6. Conclusión

En esta práctica se logró diseñar e implementar un sistema vestible para medir la respuesta galvánica cutánea y estimar el nivel de estrés. Se comprobó que tanto la respiración profunda como las tareas cognitivas generan aumentos en la señal, lo que confirma la relación entre GSR y activación simpática.

Aunque la GSR es una herramienta útil para monitoreo continuo, no debe considerarse un indicador absoluto de estrés, ya que puede verse influenciada por diferentes factores externos.

