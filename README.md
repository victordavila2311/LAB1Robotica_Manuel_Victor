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

Luego de realizar la impresion se introdujo el marcador junto con una esponja con el fin de permitir un cierto grado de elasticidad para no dañar la herramienta en un posible punto mas profundo de lo esperado
<div>
<p style = 'text-align:center;' align="center">
<img src="" width="300px">
  TODO poner la imagen de la herramienta con el marcador
</p>
</div>

## Generación de trayectorias

Para realizar las trayectorias primero se realizó en inventor el modelo de las letras a escribir, generando un texto y extruyendolo.
<div>
<p style = 'text-align:center;' align="center">
<img src="" width="300px">
  TODO poner el link de la imagen del modelo cad de las letras y el plano
</p>
</div>



El modelo se importó al RobotStudio y desde ahí se definió el sistema de coordenadas en el mismo sentido en el que está la herramienta, luego realizaron puntos sobre el contorno de las letras y los puntos elevados para la transición de una letra a otra, posteriormente se crearon las trayectorias correspondientes a una velocidad de 100. Cabe recalcar que en la rutina también se incluyo el movimiento desde el "home" del robot hacia las letras.


<div>
<p style = 'text-align:center;' align="center">
<img src="" width="300px">
  TODO poner imagen de las trayectorias del cad en robot studio
</p>
</div>


El código RAPID utilizado para los dos ejercicios de escritura se encuentran dentro del repositorio, [plano sin inclinar](TODO poner el link al codigo de rapid plano) y [plano inclinado](TODO poner el link al codigo de rapid inclinado).

## Video, simulación e implementación

## Conclusiones
