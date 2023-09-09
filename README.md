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

El modelo se importó al RobotStudio y desde ahí se definió el sistema de coordenadas en el mismo sentido en el que está la herramienta, luego realizaron puntos sobre el contorno de las letras y los puntos elevados para la transición de una letra a otra, posteriormente se crearon las trayectorias correspondientes a una velocidad de 100. Cabe recalcar que en la rutina también se incluyo el movimiento desde el "home" del robot hacia las letras.


<div>
<p style = 'text-align:center;' align="center">
<img src="" width="300px">
  TODO poner imagen de las trayectorias del cad en robot studio
</p>
</div>


El código RAPID utilizado para los dos ejercicios de escritura se encuentran dentro del repositorio, [plano sin inclinar](TODO poner el link al codigo de rapid plano) y [plano inclinado](TODO poner el link al codigo de rapid inclinado).

## Video, simulación e implementación

1)simulacion escritura en plano horizontal.

<a href="" target="_blank"><img src="" 
alt="IMAGE ALT TEXT HERE" width="260" height="319.5" border="10" /> </a> TODO incluir el video de youtube de la implementacion horizontal

2)simulacion escritura en plano inclinado.

<a href="" target="_blank"><img src="" 
alt="IMAGE ALT TEXT HERE" width="260" height="319.5" border="10" /> </a> TODO incluir el video de youtube de la implementacion inclinada

3)implementacion en plano horizontal.

<a href="https://youtu.be/-qRDwdd-Kuo" target="_blank"><img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/blob/main/imagenes_simulacion/imagen%20implementacion.png" 
alt="IMAGE ALT TEXT HERE" width="260" height="319.5" border="10" /></a>


resultado del video 


El unico problema en el resultado de la implementacion fue que en el comienzo no salia la suficiente tinta en el marcador

<div>
<p style = 'text-align:center;' align="center">
<img src="https://github.com/victordavila2311/LAB1Robotica_Manuel_Victor/blob/main/imagenes_simulacion/resultado%20implementacion.jpeg" width="300px">
</p>
</div>

## Conclusiones
