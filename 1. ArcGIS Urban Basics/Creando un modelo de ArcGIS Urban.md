
## Flujo de trabajo con ArcGIS Urban

ArcGIS Urban proporciona muchos beneficios que ayudan en el proceso de planificación. Puedes comenzar a implementar estos beneficios siguiendo un flujo de trabajo sencillo para crear un modelo de ArcGIS Urban.

![[Pasted image 20230523120756.png]]

Antes de poder crear un modelo de ArcGIS Urban, debes iniciar sesión en ArcGIS Online utilizando una cuenta con la licencia de Urban. Después de iniciar sesión, desde la página de Urban, puedes crear tu modelo. Una vez creado el modelo, gestionas la configuración del modelo. A continuación, importas tus datos de planificación, como datos de tipos y capas, al modelo. Después de agregar los datos, creas escenarios de diseño urbano utilizando planes y proyectos. Por último, puedes compartir y colaborar con otros usuarios utilizando el modelo.

## Opciones del modelo de ArcGIS Urban

Cuando empiezas con ArcGIS Urban, tienes dos opciones principales: abrir una ciudad de ejemplo o crea
r un nuevo modelo. Comprender estas opciones te ayudará a determinar cuál es la mejor para crear tu nuevo modelo.

![[Pasted image 20230523121005.png]]

### Ciudad de ejemplo

Boston, Massachusetts, tiene una población de aproximadamente 700,000 habitantes y está trabajando para gestionar su crecimiento mientras preserva su historia. La ciudad de ejemplo de Boston tiene diferentes capas que puedes explorar, incluyendo varios proyectos, planes e indicadores. Aunque puedes explorar los planes existentes, también puedes crear una copia de los planes para examinar más a fondo la zonificación, los tipos de construcción, el uso del espacio y las métricas.

### Plantillas

Hay tres opciones de plantillas:

1.  **Plantilla vacía:** No contiene planes, proyectos, indicadores, tipos o capas. Puedes utilizar esta plantilla como punto de partida antes de cargar tus datos en el modelo.
    
2.  **Plantilla predeterminada de EE. UU.:** No contiene planes ni proyectos, pero incluye uso del espacio predefinido, tipos de construcción y zonificación, y datos de ArcGIS Living Atlas.
    
3.  **Plantilla de geodatabase de archivos:** Te permite configurar un modelo urbano basado en una geodatabase de archivos exportada desde otro modelo.

### Crear el modelo de ArcGIS Urban

Imagina que eres un analista de planificación y te han pedido que crees un nuevo modelo de Urban utilizando una geodatabase de archivos que un colega ha exportado desde un modelo existente. Con una comprensión del flujo de trabajo de Urban y los componentes del modelo, puedes crear tu propio modelo. En este ejercicio, seguirás el flujo de trabajo para crear un nuevo modelo utilizando una geodatabase de archivos.

Tiempo estimado de finalización: 30 minutos

Para completar este ejercicio, necesitarás:

-   ArcGIS Pro 2.7 (Advanced) con la extensión ArcGIS Urban.
-   Una cuenta organizativa de ArcGIS Online con el rol de Editor o equivalente.
-   La geodatabase de archivos que contiene el modelo de Urban exportado.

Nota: Asegúrate de que la geodatabase de archivos sea accesible y contenga los datos necesarios para tu nuevo modelo.

### Pasos:

1.  Inicia ArcGIS Pro en tu computadora.
    
2.  Crea un proyecto nuevo o abre un proyecto existente donde desees crear el nuevo modelo de Urban.
    
3.  En el panel de Catálogo, navega hasta la ubicación donde se encuentra la geodatabase de archivos.
    
4.  Haz clic derecho en la geodatabase de archivos y selecciona **Importar** > **Geodatabase (Múltiple)**.
    
5.  En el cuadro de diálogo **Importar Geodatabase**, elige la configuración adecuada para importar la geodatabase, como la carpeta de destino, las opciones de importación y el filtro de conjuntos de datos. Haz clic en **Aceptar** para iniciar el proceso de importación.
    
6.  Una vez que se complete la importación, verás los conjuntos de datos importados en el panel de Catálogo.
    
7.  En el panel de **Catálogo**, expande la geodatabase importada y navega hasta el conjunto de datos del modelo de Urban.
    
8.  Haz clic derecho en el conjunto de datos del modelo de Urban y selecciona **Crear modelo de Urban**.
    
9.  En el cuadro de diálogo **Crear modelo de Urban**, proporciona un nombre y una descripción para tu nuevo modelo. Opcionalmente, puedes establecer el sistema de coordenadas y ajustar otras configuraciones según sea necesario. Haz clic en **Aceptar** para crear el nuevo modelo de Urban.
    
10.  El nuevo modelo de Urban se creará y se agregará a tu proyecto. Ahora puedes comenzar a configurar y personalizar el modelo según tus requisitos de planificación.
    
11.  Configura el modelo definiendo los componentes como proyectos, planes, indicadores, tipos y capas. Configura los parámetros y atributos necesarios para cada componente según tus necesidades de planificación.
    
12.  Importa datos adicionales, si es necesario, para mejorar tu modelo. Esto puede incluir capas adicionales, datos demográficos, regulaciones de zonificación u otros conjuntos de datos relevantes.
    
13.  Crea escenarios de diseño urbano utilizando planes y proyectos dentro de tu modelo. Explora diferentes opciones de desarrollo, analiza sus impactos y compara los resultados.
    
14.  Comparte y colabora con otros interesados publicando tu modelo en ArcGIS Online. Esto permitirá que otros accedan y revisen el modelo, proporcionen comentarios y participen en el proceso de planificación.
    
15.  Itera y perfecciona tu modelo según sea necesario, en función de los comentarios y los requisitos de planificación en evolución