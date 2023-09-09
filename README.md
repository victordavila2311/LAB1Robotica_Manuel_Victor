## Laboratorio No. 1 - Robótica Industrial
### Integrantes: 
- Victor Manuel Dávila Castañeda.
- Manuel Felipe Carranza Montenegro.
## Descripción de la solución planteada
## Diseño de la herramienta:
Para el diseño de la herramienta porta marcador se tuvo en cuenta que, esta no se encontrará alineada con la articulación No. 6.

<div>
<p style = 'text-align:center;' align="center">
<img src="" width="300px" >
 https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/assets/82252851/e05677f4-f09e-418d-89ed-2f166d151d77
 TODO aca toca poner el link de la herramienta
</p>
</div>

Se planteó hacer la herramienta a través de impresion 3D, por lo que se procedió a diseñar el modelo en inventor para obtener los planos y el modelo STL que se exportó a Robot Studio.
<div>
<p style = 'text-align:center;' align="center">
<img src="" width="300px">
  TODO poner la imagen de la herramienta importada en el robot studio
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
