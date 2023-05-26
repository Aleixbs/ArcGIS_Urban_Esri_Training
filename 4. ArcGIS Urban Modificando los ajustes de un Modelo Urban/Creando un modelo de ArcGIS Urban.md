![[Pasted image 20230524162418.png|250]]

## Describiendo los ajustes/configuraciones de un modelo de ArcGIS Urban 

Después de crear su modelo Urbano, puede administrar las configuraciones del modelo a través del administrador de datos. La gestión de estas configuraciones le permite personalizar la visualización de su ciudad en ArcGIS Urban. La siguiente tabla describe las configuraciones disponibles.

Entiendo. Aquí tienes tu tabla de contenidos con 2 columnas:

|Configuración|Descripción|
|---|---|
|Nombre de la ciudad|Nombre de la ciudad|
|Logo de la ciudad|URL del logotipo de la ciudad|
|Vista predeterminada|Vista del mapa inicial|
|Visualización esquemática|Edificios y árboles existentes, mapa base|
|Visualización realista|Malla de realidad, árboles existentes, mapa base|
|Capa de elevación|Capa para mostrar terreno personalizado|
|Capas base personalizadas|Capas que enriquecen la visión general|
|Imágenes a nivel de calle|Imágenes para comparar futuro y situación actual a nivel de calle|
|Visualización inicial|Visualización predeterminada para edificios existentes|
|Configuración de visualización|Configuración de etiqueta CustomID para parcelas|


## Uso de capas base en un modelo urbano

Ahora que está familiarizado con las opciones de configuración del modelo, explorará cómo se pueden usar las capas base 3D en un modelo de ArcGIS Urban. Las capas base 3D se utilizan para crear un gemelo digital y agregar una visualización del mundo real a su modelo. Puede agregar capas de edificios y árboles para visualizar las condiciones existentes o establecer mapas base personalizados y capas de elevación para aumentar el modelo urbano.

Las capas base tridimensionales ayudan a traer características del mundo real a su modelo urbano. Puede usar capas como edificios existentes, árboles existentes, capas base personalizadas, mapas base personalizados y elevaciones personalizadas. Aunque hay muchas opciones para configurar las capas base 3D, no tiene que configurar una capa para cada elemento. Si no se establecen capas base, el modelo utilizará mapas estándar de ArcGIS Online y el servicio World Elevation Terrain.

## Nota

Las siguientes secciones incluyen escenas web incrustadas que se pueden explorar. Las imágenes pueden tardar un momento en cargarse.

## Capa de edificios existentes

La capa de edificios existentes se utiliza para visualizar los edificios existentes de su ciudad y para propósitos de enmascaramiento. Puede visualizar un escenario de diseño enmascarando los edificios existentes donde no existirían en el escenario o se intersectarían con los edificios del plan o proyecto futuro.

En Urban, puede configurar dos capas de edificios existentes: una para la vista esquemática y otra para la vista realista. Los edificios existentes para la visualización esquemática se representan como edificios esquemáticos blancos con bordes. La capa de edificios existentes para la visualización realista aparece con un mapa base realista. Esta vista trae edificios realistas a su modelo urbano.

![[3DSceneBuildings.gif]]
## Capa de árboles existentes

La capa de árboles existentes se utiliza para visualizar los árboles existentes de su ciudad y para enmascaramiento. Puede visualizar un escenario de diseño enmascarando los árboles existentes donde no existirían en el escenario o se intersectarían con los edificios del plan o proyecto futuro.

![[3DSceneTrees.gif]]
## Capas base personalizadas

Además de los edificios y árboles existentes, puede agregar más capas base a la visión general en ArcGIS Urban. Estas capas deben estar agrupadas en una escena web alojada en ArcGIS Online.

![[3DSceneCustomBaseLayer.gif]]

## Mapas base personalizados

Puede agregar tanto un mapa base esquemático como un mapa base realista a ArcGIS Urban. Una vez agregados, puede usar cualquiera de los mapas base en la visión general.

![[3DSceneCustomBaseMap.gif]]
## Capa de elevación personalizada

ArcGIS Urban utiliza la capa de elevación personalizada para mostrar un terreno dentro de la escena. Cuando agrega edificios futuros a un plan o dibuja objetos en un proyecto, la capa de elevación alinea estas características de construcción con el suelo.

ArcGIS Urban utiliza el servicio World Elevation Terrain si no usa una capa de elevación personalizada.

![[3DSceneCustomElevation.gif]]

#### Verifique su comprensión 

1. Si no se establecen capas base, ¿qué mapas usará su modelo ArcGIS Urban?
  
El modelo utilizará los mapas estándar de ArcGIS Online y el servicio World Elevation Terrain.

2. Además de visualizar los edificios existentes de su ciudad, ¿cómo puede usar su capa de edificios existentes?

La capa de edificios existentes puede ser utilizada para propósitos de enmascaramiento.

3. ¿Qué acción debe tomar para agregar capas base personalizadas a la visión general en ArcGIS Urban?
Debe agrupar las capas en una escena web alojada en ArcGIS Online.

 4. ¿Qué capa base 3D se publica en ArcGIS Online y se utiliza para mostrar el terreno en una escena web?

Capa de elevación personalizada


## Cuestionario

Las pruebas ponen a prueba los conocimientos y habilidades que ha aprendido en cada sección. Debe responder correctamente a 2 de 3 preguntas para aprobar este cuestionario. Debe aprobar todos los cuestionarios de sección para recibir su certificado de finalización del curso.

¿Qué paso en el flujo de trabajo del modelo ArcGIS Urban debe realizar después de crear un nuevo modelo?

Gestionar las configuraciones del modelo

¿Cuáles dos capas pueden usarse para modificar la visibilidad de un modelo urbano?

Elija dos.

Capa de árboles

Capa base personalizada

¿Qué configuración de ArcGIS Urban le permite establecer la visualización predeterminada para los edificios existentes?

Visualización inicial

