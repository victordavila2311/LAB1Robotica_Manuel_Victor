## Laboratorio No. 1 - Robótica Industrial
### Integrantes: 
- Victor Manuel Dávila Castañeda.
- Manuel Felipe Carranza Montenegro.
## Descripción de la solución planteada
## Diseño de la Herramienta (Efector Final):

Para el diseño del efector final, se consideró que no debería alinearse con la articulación número 6 del robot. Esto se hizo con el fin de reducir la probabilidad de ingresar en una singularidad que podría impedir la ejecución adecuada de la rutina, por tal motivo dicha herramienta cuenta con una inlinación de 45°.

Modelado del Efector Final en Autodesk Inventor.

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/assets/82252851/3e54788c-fd73-4fbc-b19a-a6e3236d5a12" width="300px" 
</p>
</div>

Se decidió fabricar la herramienta utilizando impresión 3D, lo que llevó a la creación del modelo en Inventor. A partir de este diseño, se generaron los planos necesarios y se obtuvo el modelo en formato STL, que posteriormente se importó a Robot Studio.

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/assets/82252851/9bc03ca1-a9e2-4eb7-ac9b-6e65cfd7f75d" width="300px" >
</p>
</div>

Después de completar la impresión, se procedió a introducir el marcador en la herramienta, junto con una esponja. Esta elección se hizo con el propósito de proporcionar un grado de elasticidad adicional, con el fin de evitar posibles daños en caso de que el marcador penetre más profundamente de lo previsto.

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/assets/82252851/678d3ef2-2f87-432c-959a-20d94432932a" width="300px" >
</p>
</div>

## Generación de trayectorias

Para crear las trayectorias, inicialmente se diseñó el modelo de las letras que se iban a escribir en Inventor. Esto se logró generando un texto y extruyéndolo.

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/assets/82252851/22d05586-68b4-40e2-84a8-a1abd7f5e610" width="300px" >
</p>
</div>

El modelo se importó a RobotStudio y desde allí se definió el sistema de coordenadas en la misma orientación que la herramienta. Luego, se colocaron puntos a lo largo del contorno de las letras y puntos elevados para facilitar la transición entre una letra y otra. A continuación, se crearon las trayectorias correspondientes, con una velocidad de 100 unidades (por ejemplo, milímetros por segundo). Es importante mencionar que en la rutina también se incluyó el movimiento desde la posición "home" del robot hacia las letras.

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/assets/82252851/fde2e2e1-0896-4848-9a8b-d7463b84b075" width="300px" >
</p>
</div>

El código RAPID utilizado para los dos ejercicios de escritura se encuentran dentro del repositorio, [plano horizontal](https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/blob/main/codigos_RAPID/plano%20horizontal/Module1.mod) y [plano inclinado](https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/blob/main/codigos_RAPID/plano%20inclinado/Module2.mod).

## Video, simulación e implementación (hacer click en las imagenes)

1) Simulación escritura en Plano Horizontal.

<div>
<p style = 'text-align:center;' align="center">
<a href="https://youtu.be/QPYjsCDeQc4" target="_blank"><img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/blob/main/imagenes_simulacion/imagen%20simulacion%20horizontal.png" 
alt="IMAGE ALT TEXT HERE" width="380" height="319.5" border="10" /> </a> 
</p>
</div>

2) Simulación escritura en Plano Inclinado.

<div>
<p style = 'text-align:center;' align="center">
<a href="https://youtu.be/5O8jzoXYNls" target="_blank"><img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/blob/main/imagenes_simulacion/imagen%20simulacion%20vertical.png" 
alt="IMAGE ALT TEXT HERE" width="390" height="319.5" border="10" /> </a>
</p>
</div>

3) Implementación en Plano Horizontal.

<div>
<p style = 'text-align:center;' align="center">
<a href="https://youtu.be/-qRDwdd-Kuo" target="_blank"><img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/blob/main/imagenes_simulacion/imagen%20implementacion.png" 
alt="IMAGE ALT TEXT HERE" width="260" height="319.5" border="10" /></a>
</p>
</div>

El único problema que se experimentó en la implementación fue que al principio no se dispensó suficiente tinta desde el marcador, lo que resultó en que la primera letra no quedara tan clara como se esperaba. Sin embargo, las letras posteriores se visualizaron según lo planeado.

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/blob/main/imagenes_simulacion/resultado%20implementacion.jpeg" width="300px">
</p>
</div>

## Conclusiones
- La posibilidad de utilizar inventor para importar el modelo de las letras facilito de gran manera la generacion de las trayectorias.
- Primero se realizo una prueba en simulacion con una herramienta rect que no dio resultado debido a que esto genera una gran cantidad de singularidades, por lo que se debe intentar en lo posible el usar herramientas cuyos sistemas de coordenadas tengan la menor coincidencia posible con los de los eslabones del robot.
- los Work objects son fundamentales a la hora de realizar las trayectorias ya que aunque al cambiar el angulo del mismo generaba nuevos errores de movimiento, si facilitaba la adaptacion del robot y el codigo a nuevas trayectorias sin tener que empezar todo desde cero
