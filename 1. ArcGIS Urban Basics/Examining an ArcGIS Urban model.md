## ArcGIS Urban requerimientos de licenciamiento

ArcGIS Urban tiene tres usuarios principales: el viewer, el editor y el administrador.

![[Pasted image 20230523110413.png|250]]

##### Viewer

El viewer tiene acceso para ver los planes y proyectos de un modelo. Este usuario puede ser del público o de dentro de su organización.

![[Pasted image 20230523110434.png | 300]]

##### Editor

El editor está dentro de una organización y puede editar planes y proyectos, administrar datos y crear nuevos indicadores.
![[Pasted image 20230523110501.png | 300]]

##### Administrador

El administrador también está dentro de la organización y puede crear nuevos modelos, planes y proyectos.

![[Pasted image 20230523110533.png |250]]      ![[Pasted image 20230523110602.png | 250]]

#### Software necesario

Para acceder a Urban, una organización debe comprar el paquete de aplicaciones ArcGIS Urban Suite. Este paquete de aplicaciones incluye ArcGIS Urban y ArcGIS CityEngine.

Después de que se compra el paquete de aplicaciones ArcGIS Urban Suite, las licencias adicionales están disponibles bajo su organización. Un administrador de la organización o un miembro con privilegios de licencia puede asignar las licencias a usuarios individuales.

![[Pasted image 20230523111018.png | 200]]

Dependiendo de los flujos de trabajo en los que un usuario participará, el usuario debe tener suficientes privilegios otorgados a través de su rol asignado en ArcGIS Online.

Entender estos requisitos de licencia es una parte importante para configurar con éxito su organización para usar ArcGIS Urban para sus necesidades de planificación.

## Componentes de ArcGIS Urban

Las iniciativas y flujos de trabajo de planificación vienen en diferentes tamaños. Algunas son desarrollos individuales que tardan uno o dos años en completarse. Otros son proyectos más complejos que incluyen diferentes edificios y zonificación, como escuelas, restaurantes, negocios y apartamentos, y tardan décadas en construirse. ArcGIS Urban está diseñado para respaldar la planificación y el análisis de estas actividades de desarrollo utilizando un modelo urbano.

### Modelo Urbano 

Un modelo urbano consta de dos bases de datos. Una base de datos es la base de trabajo que contiene los datos de tipos, capas, proyectos, planes e indicadores. La otra base de datos es una copia sincronizada de la base de trabajo que no se puede editar pero se comparte con todos. Las capas representan datos como zonificación, uso de suelo, superposiciones y parcelas. Los datos de tipos se unen con las capas para proporcionar información adicional.

![[Pasted image 20230523112557.png | 400]]

### Proyecto Urbano 

ArcGIS Urban organiza los procesos de planificación a corto plazo a nivel de parcela en proyectos. Por ejemplo, se pueden agregar múltiples propuestas de construcción a un solo proyecto como escenarios individuales. Cada proyecto puede mostrar un modelo detallado de información de los edificios. Para ayudar en la toma de decisiones, el público y los interesados pueden revisar cada escenario dentro del contexto de la condición actual del área del proyecto.

![[Pasted image 20230523112719.png]]

### Planes Urbanos 

ArcGIS Urban utiliza planes para actividades de planificación a largo plazo y proporciona el conjunto de herramientas para comparar y analizar diferentes escenarios. Los planes ayudan a cuantificar y comprender cómo los cambios propuestos, basados en los escenarios, pueden contribuir a los objetivos estimados en general, como las demandas de vivienda y el crecimiento de la población dentro de una ciudad. Los planes también permiten aplicar las regulaciones de zonificación de manera digital y ajustarlas según los escenarios. Urban se puede utilizar para crear escenarios dentro del plan y examinar cómo diversos cambios afectan la capacidad de vivienda y la disponibilidad de empleo.

![[Pasted image 20230523112748.png]]

### Indicadores Urbanos 

Los indicadores añaden información adicional y análisis a tus planes y proyectos urbanos en ArcGIS Urban. Se pueden agregar tres tipos de indicadores:

1. **Indicadores de capacidad:** Analizan la capacidad de población, hogares y empleo en el plan y a nivel de parcela. La condición existente o la capacidad de un proyecto y los valores de capacidad objetivo se introducen manualmente en el modelo. ArcGIS Urban combina los valores de capacidad con los escenarios de diseño para predecir las nuevas condiciones de un proyecto.

2. **Indicadores personalizados:** Son escenas web y paneles de operaciones que se utilizan en ArcGIS Urban. Cualquier dato SIG, como los resultados de análisis espaciales, que se pueda mostrar en un mapa o en una escena se puede utilizar en un indicador personalizado.

3. **Indicadores de ArcGIS Living Atlas of the World:** Son un conjunto preseleccionado de indicadores disponibles dentro de ArcGIS Urban. Estos indicadores están disponibles automáticamente en función de tu ubicación.

![[Pasted image 20230523112835.png]]

## Navegación en ArcGIS Urban 

Claro, aquí está el texto formateado en Markdown con las palabras clave resaltadas:

**ArcGIS Urban** proporciona **herramientas de navegación** para cambiar la vista del modelo. Estas herramientas son accesibles usando los botones del ratón, atajos de teclado, teclas de flecha y la **barra de herramientas de vista**.

El primer conjunto de **herramientas de navegación** de **ArcGIS Urban** utiliza el ratón. Para **desplazar** la vista, arrastra el ratón.

Para **rotar** o **inclinar** la vista, haz clic derecho en la vista y arrastra en la dirección que quieres ir.

Para **acercar**, gira el botón de la rueda.

Finalmente, para acercar a un solo punto dentro de la vista, haz **doble clic**.

Los **atajos de teclado** también se pueden usar para navegar en tu vista de **ArcGIS Urban**. Presiona la tecla **N** para orientar la vista hacia el norte.

Para establecer la vista perpendicular al suelo, presiona la tecla **P**.

Para mover la vista más cerca del suelo, presiona la tecla **J**, y presiona la tecla **U** para alejarte del suelo.

Otras herramientas de navegación con el teclado son las **teclas de flecha**. Usa estas teclas para mover la vista hacia arriba, abajo, izquierda y derecha.

El conjunto final de **herramientas de navegación** son accesibles desde la **barra de herramientas de vista**, que se encuentra en la esquina inferior derecha de la vista.

Desde esta barra de herramientas, puedes hacer clic en el botón **2D** o **3D** para inclinar la vista.

Para orientar la vista de nuevo al norte, simplemente haz clic en la **flecha del norte**.

A medida que trabajes con **ArcGIS Urban**, descubrirás que estas sencillas **herramientas de navegación** facilitan la visualización de los detalles de tus **planes y proyectos urbanos** de manera más fácil y eficiente.

## Explorar los componentes del modelo de ArcGIS Urban

Ahora que comprendes los componentes del modelo urbano y cómo navegar en un modelo, ampliarás esta base aprendiendo los conceptos básicos de la aplicación. En este ejercicio, utilizarás una ciudad de ejemplo para explorar y navegar por ArcGIS Urban y sus principales componentes.

Tiempo estimado de finalización: 25 minutos

Para completar los ejercicios, necesitarás lo siguiente:

-   Una cuenta de Organización de ArcGIS Online
-   Un rol de Editor o equivalente
-   ArcGIS Urban

Nota: La organización de ArcGIS Online que se utilice para completar los ejercicios debe tener habilitado ArcGIS Urban. La cuenta de usuario debe tener asignada la licencia de Urban y tener el rol de Editor en ArcGIS Online.

**Proceso de exploración de componentes** 

Para comenzar, iniciarás sesión en tu cuenta organizativa de ArcGIS Online. Al iniciar sesión, podrás abrir el modelo urbano de ejemplo.

1.  En un navegador web, ve a ArcGIS Online ([www.arcgis.com](http://www.arcgis.com/)) y haz clic en "Iniciar sesión".
    
2.  Ingresa el nombre de usuario y la contraseña de tu cuenta organizativa, y luego haz clic en "Iniciar sesión".
    

Abre la ciudad de ejemplo

Ahora que has iniciado sesión en tu organización de ArcGIS Online, accederás a ArcGIS Urban para abrir la ciudad de ejemplo.

1.  En la parte superior de la página, haz clic en el botón "Aplicaciones".
    
2.  Selecciona "Urban".
    

Nota: Si no tienes la opción de abrir ArcGIS Urban, verifica que tengas los permisos necesarios dentro de tu organización para ArcGIS Urban.

ArcGIS Urban se abre en una página donde puedes abrir modelos recientes, crear un nuevo modelo urbano o abrir una ciudad de ejemplo.

3.  Haz clic en "Abrir ejemplo".

Navegar por un modelo de ArcGIS Urban

ArcGIS Urban se abre con un modelo de Boston, Massachusetts. En la parte superior izquierda de la pantalla se encuentra el menú Urban, así como el panel lateral de capas, que incluye un campo de búsqueda y botones para los tres componentes principales de Urban: Proyectos, Planes e Indicadores.

Además de las condiciones existentes, se han agregado modelos de edificios de proyectos y se han simbolizado según su estado.

Utiliza las herramientas de navegación para desplazarte y hacer zoom en el mapa hasta el centro de Boston y para navegar por los proyectos en la zona.

Explorar el panel lateral de capas

A continuación, explorarás el panel lateral de capas donde puedes controlar la visibilidad de las capas.

1.  Haz clic en el botón de menú (ícono de hamburguesa) para abrir el panel lateral de capas.
    
2.  En el panel lateral de capas, puedes cambiar el mapa base, activar y desactivar capas y tomar una captura de pantalla.
    
3.  Desde el panel lateral de capas, haz clic en "Tomar una captura de pantalla".
    

Nota: La barra de "Tomar una captura de pantalla" aparecerá en la parte superior de la vista. Puedes dibujar un rectángulo o utilizar toda la ventana para tomar una captura de pantalla.

4.  Dibuja un rectángulo alrededor de una pequeña sección de edificios.
    
5.  Haz clic en "Guardar" en la barra de "Tomar una captura de pantalla".
    

Si aparece un cuadro de diálogo, haz clic en "Aceptar" para guardar la captura de pantalla.

Se guardará un archivo PNG de alta resolución en tu carpeta de Descargas para usarlo en una presentación o documento.

Explorar un proyecto

Los proyectos permiten gestionar desarrollos a corto plazo a nivel de parcela. Ahora, explorarás un proyecto y accederás a sus detalles.

1.  En la parte superior izquierda, haz clic en "Proyectos".
    
2.  Se expandirá una lista que muestra todos los proyectos del modelo. Cada proyecto está marcado con un ícono que indica el estado del proyecto.
    
3.  Haz clic en "Estado" y selecciona "Aprobado por la Junta".
    

La lista de proyectos y la vista del mapa se actualizarán para mostrar solo aquellos proyectos que han sido aprobados por la junta.

4.  Ahora verás el proyecto "815 East Fifth Street", que ya ha sido completado.
    
5.  En el campo de búsqueda, sobre el panel lateral, reemplaza la palabra "Proyectos" por "815 East Fifth Street" y luego presiona Enter.
    

La vista se acerca al proyecto y se indica el edificio propuesto.

6.  En los resultados de búsqueda, haz clic en el proyecto "815 East Fifth Street".

En el panel lateral, aparecerá la tarjeta de detalles del proyecto. La información en esta tarjeta incluye el nombre del proyecto, un enlace a su página web y sus fechas de inicio y finalización.

¿Cuál fue la fecha de inicio del proyecto?

Haz clic en "Existente".

La vista se actualiza para mostrar la condición existente del sitio del proyecto sin el edificio propuesto. Se pueden agregar otros escenarios de construcción al proyecto para que sean fácilmente visualizados por las partes interesadas.

9.  En la parte superior izquierda del encabezado, a la izquierda del nombre del proyecto, haz clic en el botón "Volver a la vista general".

Exploraste el proyecto "815 East Fifth Street" y viste cómo acceder a la información sobre el proyecto.

Explorar un plan

Un plan está compuesto por proyectos individuales a pequeña escala. Ahora, explorarás un plan y verás cómo el escenario propuesto aumenta la población del área.

Nota: Explorarás un plan de ejemplo que tiene funcionalidad limitada. Puedes explorar la funcionalidad completa del plan creando una copia del mismo.

1.  En el panel lateral, haz clic en "Planes" y luego en "South Boston Dot Ave".

Nota: Puede tomar unos momentos para que el plan se cargue.

La vista del mapa se acerca al área del plan, con información sobre el plan en el panel lateral. También se ha agregado una capa de zonificación.

¿Cuántos escenarios tiene este plan?

Haz clic en el botón "Tablero de instrumentos".

Revisa las métricas disponibles para el plan.

Haz clic en los cuatro escenarios para comparar la cantidad de empleos que cada uno crearía.

¿Qué escenario crea la mayor cantidad de empleos para esta área?

Haz clic en el botón "Volver a la vista general".

Examinaste el plan "South Boston Dot Ave" y viste los diferentes escenarios que contiene.

Explorar los indicadores

Un indicador proporciona información adicional y análisis a tus planes y proyectos urbanos. Ahora explorarás los indicadores para ver cómo te ayudan a obtener más información en la planificación urbana.

1.  En el panel lateral, haz clic en "Indicadores".

Aparecerá una lista de indicadores disponibles.

2.  Selecciona el indicador "Riesgo de inundación".

En el panel lateral, la tarjeta de detalles proporciona más información sobre este indicador e incluye una leyenda para ayudarte a interpretarlo.

En la vista del mapa, el mapa se actualiza para mostrar las áreas que se proyecta que estén en riesgo de inundación. Esta información de riesgo de inundación es útil para mostrar qué proyectos podrían verse afectados por inundaciones.

4.  Desplaza el mapa para ver las áreas de la ciudad que están dentro de las zonas de riesgo de inundación.

Haz clic en "Volver a la lista".

Selecciona el indicador "Crimenpersonal (solo EE. UU.)".

5.  Desplaza el mapa para ver la relación del crimen con los proyectos del área.

El mapa se actualiza para mostrar dónde el crimen personal está por encima y por debajo del promedio nacional. Este indicador ayuda a mostrar la relación de los proyectos con el crimen del área.

Cierra la pestaña del navegador web de ArcGIS Urban.

En este ejercicio, exploraste los proyectos, planes e indicadores de ArcGIS Urban. Descubriste cómo estos componentes se pueden utilizar en el proceso de planificación urbana para crear y analizar diferentes escenarios.