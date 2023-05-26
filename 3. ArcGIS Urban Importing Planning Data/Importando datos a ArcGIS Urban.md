## Introducción

Después de crear un modelo de ArcGIS Urban y gestionar la configuración del modelo, el siguiente paso es importar datos de planificación en el modelo. Un modelo de Urban admite datos de planificación para flujos de trabajo como el uso del espacio, el uso del suelo y la zonificación. Es esencial comprender el tipo de datos, el esquema de datos y la conexión de datos de cada tipo de datos de planificación. En este curso, aprenderás cómo configurar los datos de tipos y las capas de entidades en un modelo de ArcGIS Urban.

## Objetivos del curso

-   Configurar los datos de tipos en ArcGIS Urban.
-   Configurar las capas en ArcGIS Urban.

## Requisitos de software

Para completar los ejercicios, necesitarás lo siguiente:

-   Una cuenta organizativa de ArcGIS Online.
-   Rol de Editor o equivalente.
-   ArcGIS Urban.
-   Microsoft Excel 2007 o posterior.

## Datos

Haz clic en "Descargar Datos" para descargar los datos.

[Descargar Datos](https://chat.openai.com/UrbanImportPlanData.zip)

Tamaño del archivo: 79.5 KB

Para instalar los datos, debes extraerlos del archivo ZIP en la carpeta C:\EsriTraining.

## Flujo de trabajo con ArcGIS Urban

ArcGIS Urban proporciona muchos beneficios que ayudan en el proceso de planificación. Puedes comenzar a implementar estos beneficios siguiendo un flujo de trabajo sencillo para crear un modelo de ArcGIS Urban.

![[Pasted image 20230523120756.png]]

Antes de poder crear un modelo de ArcGIS Urban, debes iniciar sesión en ArcGIS Online utilizando una cuenta con la licencia de Urban. Después de iniciar sesión, desde la página de Urban, puedes crear tu modelo. Una vez creado el modelo, gestionas la configuración del modelo. A continuación, importas tus datos de planificación, como datos de tipos y capas, al modelo. Después de agregar los datos, creas escenarios de diseño urbano utilizando planes y proyectos. Por último, puedes compartir y colaborar con otros usuarios utilizando el modelo.

## Datos de tipos en Urban

Después de haber creado un modelo de Urban y haber gestionado la configuración del modelo, puedes comenzar a configurar los datos dentro del modelo. Dentro del sistema de registro, se pueden configurar seis tipos diferentes. En la mayoría de los casos, los datos de tipos deben configurarse primero antes de configurar las capas de entidades. Algunos tipos requieren que otros datos de tipos ya estén definidos, como los tipos de zonificación que requieren que los tipos de uso del espacio ya estén asignados.

### Tipos de zonificación en Urban

Los tipos de zonificación (Zoning types) describen una combinación de restricciones de códigos de zonificación. Los tipos de zonificación no tienen geometría; en su lugar, se vinculan a una capa de zonificación basada en un ID de unión. Debes tener tipos de uso del espacio disponibles en el modelo antes de poder configurar los tipos de zonificación. Los tipos de zonificación imponen restricciones como la altura máxima construible, la cobertura máxima de la parcela o los usos del espacio permitidos.

![[Pasted image 20230523161931.png]]

### Tipos de superposición en Urban

Los tipos de superposición (Overlay types) no tienen geometría y se hacen referencia a través de límites de superposición. Los límites de superposición definen la extensión espacial de las restricciones del código de zonificación. Los tipos de superposición agrupan límites de superposición individuales para que todos puedan visualizarse utilizando la misma simbología. Los tipos de superposición solo pueden definirse en planes de zonificación y no en planes de uso de suelo.

![[Pasted image 20230523161952.png]]

### Tipos de uso de suelo en Urban

Los tipos de uso de suelo describen una combinación de restricciones del código de zonificación. Los tipos de uso de suelo no tienen geometría; en su lugar, se vinculan a una capa de uso de suelo basada en un ID de unión. Debes tener tipos de uso del espacio disponibles en el modelo antes de poder configurar los tipos de uso de suelo. Los tipos de uso de suelo imponen restricciones como la altura máxima construible, la cobertura máxima de la parcela o los usos del espacio permitidos.

![[Pasted image 20230523162030.png]]

### Tipos de uso del espacio en Urban

Los tipos de uso del espacio describen el propósito de un espacio dentro de un edificio, típicamente un piso. Los pisos y las partes de los edificios pueden tener asignado un uso del espacio para restringir su uso. También puedes agregar métricas de capacidad para ayudar en el análisis de tu plan.

![[Pasted image 20230523162106.png]]

###   Tipos de edificios en Urban

Los tipos de edificios definen el uso de los edificios basándose en uno o más tipos de uso del espacio, que representan el uso de los edificios. Los tipos de edificios están compuestos por uno o más tipos de uso del espacio y actúan como plantillas para visualizar diferentes escenarios de edificios respetando el código de zonificación, que obtiene su información de los tipos de zonificación y los tipos de uso del suelo.

![[Pasted image 20230523162128.png]]

### Tipos de estado de proyecto en Urban

Los tipos de estado de proyecto describen la etapa actual de un proyecto de desarrollo urbano. Cuando un planificador filtra un proyecto por tipo de estado de proyecto, la escena se actualiza para mostrar solo aquellos proyectos que cumplen con los requisitos del filtro utilizando el icono del tipo de estado. Los tipos de estado de proyecto contienen un nombre, un icono y una descripción.

![[Pasted image 20230523162211.png]]

## Capas de entidades en Urban

Después de configurar los datos de tipos, puedes comenzar a agregar y configurar tus capas dentro del sistema de registro. Hay cuatro tipos de capas: zonificación, uso de suelo, superposiciones y parcelas. Puedes agregar capas de zonificación y uso de suelo después de configurar los tipos de zonificación y uso de suelo. Estas capas de entidades deben ser capas de entidades alojadas dentro de tu organización de ArcGIS Online.

### Capa de zonificación en Urban

Una capa de zonificación está compuesta por polígonos de geometría que definen un conjunto de regulaciones para nuevos desarrollos. Debes agregar tipos de zonificación antes de agregar una capa de zonificación, a menos que agregues la capa de zonificación durante el proceso de creación del modelo. Una capa de zonificación se vincula a los tipos de zonificación basados en un ID de unión. Solo puedes agregar una capa de zonificación a un modelo de Urban.

![[Pasted image 20230523162302.png]]

### Capa de uso de suelo en Urban

Una capa de uso de suelo está compuesta por polígonos de geometría que definen la funcionalidad del terreno. Debes agregar tipos de uso de suelo antes de agregar una capa de uso de suelo. Una capa de uso de suelo se vincula a los tipos de uso de suelo basados en un ID de unión. Solo puedes agregar una capa de uso de suelo existente y una capa de uso de suelo futuro a un modelo de Urban.

![[Pasted image 20230523162330.png]]

### Capas de superposición en Urban

Las capas de superposición te permiten anular uno o más parámetros de un tipo de zonificación. Por ejemplo, podrías usar una capa de superposición para anular el parámetro de altura máxima de un edificio. Puedes agregar múltiples capas de superposición a un modelo de Urban. Antes de agregar los límites de superposición, primero debes crear los datos de tipos de superposición y configurar los parámetros. Luego, puedes importar los límites desde una capa de entidades en tu organización de ArcGIS Online.


![[Pasted image 20230523162357.png]]

## Capa de parcelas en Urban

Una capa de parcelas está compuesta por geometrías de polígonos que definen un área de terreno para fines de propiedad y tributarios. Puedes agregar esta capa desde una capa de entidades en tu organización de ArcGIS Online. Solo puedes agregar una capa de parcelas a un modelo de Urban.

![[Pasted image 20230523162444.png]]


## Importando datos de Planificación 

Puedes importar datos de tipos en un modelo urbano utilizando varios métodos. Comprender cada método te ayudará a determinar la mejor opción para tu modelo. Con la elección correcta en mente, puedes preparar tus datos para el proceso de importación. La siguiente tabla explica qué tipos de datos se pueden importar con cada método.

1.  **Elemento único**: Permite agregar un elemento de tipo a la vez. Puedes ingresar todos los campos requeridos dentro de un cuadro de diálogo.

2.  **Desde una hoja de cálculo**: Permite agregar tus datos de tipo desde una plantilla de archivo de Excel.

3.  **Desde una tabla de entidades**: Permite agregar tus datos de tipo desde una tabla de entidades alojada.

4.  **Desde la simbología de una capa de entidades**: Permite importar datos de tipo y la simbología correspondiente desde una capa de entidades alojada existente.

5.  **Configurar**: Permite agregar un nombre, un ícono y una descripción para cada elemento dentro de un cuadro de diálogo.


|Método| <th colspan="3">Tipo</th>|
| ----------------------------------- | ----------- | ------------ | ------------- | ------------ | -------------- | -------- | 
|      | Zonificación | Superposición | Uso de suelo | Uso de espacio | Edificio | Estado del proyecto |
| Single Item                         |  ✔️ | ✔️ |   ✔️ |   ✔️ |    ✔️  |       |               |
| From Spreadsheet                    |  ✔️  |  ✔️  |    ✔️|  ✔️ |    ✔️  |      |               |
| From Feature Table                  |   ✔️ | ✔️ |  ✔️|   ✔️ |     ✔️ |     |            |
| From Feature Layer Symbology        |   ✔️|  ✔️ |   ✔️ |   ✔️   |    ✔️ |      |                     |
| Configure                           |     |       |      |     |   |   ✔️  |                     |

# Examinar un esquema de datos de tipos de zonificación

Ahora que comprendes cómo importar datos de tipos de zonificación, examinarás una plantilla de datos de tipos de zonificación. La plantilla se accede desde el menú de Tipos de Zonificación utilizando la opción de descarga en el cuadro de diálogo Desde Hoja de Cálculo. Desde la plantilla, puedes examinar los campos e ingresar datos en la hoja de cálculo para importarlos a tu propio modelo urbano.

Examinarás una plantilla de tipos de zonificación que ya ha sido descargada en la carpeta de datos del curso.

## Instrucciones

1.  Navega hasta [C:\EsriTraining\UrbanImportPlanData](C:\EsriTraining\ArcGIS Urban\UrbanImportPlanData) y abre Zoning-types.xlsx.
    
    ¿Dónde puedo encontrar estos datos?
    
2.  Examina las hojas ZoningTypes y Schema.
    
    Responde las siguientes preguntas.
    
3.  Después de terminar, cierra Microsoft Excel.
    

**Pregunta 1:** ¿Cómo se formatea la cadena de color para el tipo de zonificación en el campo de atributo Color?

_Respuesta:_ El campo de atributo Color utiliza códigos de color Hex para representar el color de zonificación.

**Pregunta 2:** El campo de atributo AllowedSpaceUseTypes puede tener una matriz de valores. ¿Qué tipo de campo utiliza AllowedSpaceUseTypes para contener estos valores?

a) Número b) Entero c) Cadena d) JSON como cadena

**Pregunta 3:** ¿Qué campo de tipos de zonificación te permite especificar la altura máxima de construcción?

_Respuesta:_ El campo HeightMax te permite especificar la altura máxima de construcción en pies o metros.

Espero que esto sea de ayuda. Si tienes alguna otra pregunta, no dudes en preguntar.

## Crear un modelo de ArcGIS Urban


Imagina que eres un analista de planificación y te han pedido que crees un gemelo digital de Hardeeville, Carolina del Sur, utilizando ArcGIS Urban. Comprender los datos y los métodos de importación utilizados en un modelo de Urban proporciona la base para crear tu modelo. Debes acceder a un modelo desde tu cuenta de ArcGIS Online para agregar datos de planificación. En este ejercicio, crearás un nuevo modelo dentro de tu organización basado en una plantilla vacía.

**Tiempo estimado de finalización: 10 minutos**

Para completar los ejercicios, necesitarás lo siguiente:

-   Cuenta organizativa de ArcGIS Online
-   Rol de publicador o equivalente
-   ArcGIS Urban
-   Microsoft Excel 2007 o posterior

**Descargar los datos**

Para completar el ejercicio, debes descargar los datos. Si ya has descargado e instalado los datos, continúa con el siguiente paso.

_¿No puedes encontrar los datos que descargaste?_

**Iniciar sesión en ArcGIS Online**

Para comenzar, iniciarás sesión en tu cuenta organizativa de ArcGIS Online. Al iniciar sesión, podrás crear un modelo de ArcGIS Urban y guardar tu trabajo.

En un navegador web, ve a ArcGIS Online ([www.arcgis.com](http://www.arcgis.com/)) y haz clic en "Sign In" (Iniciar sesión).

Ingresa tu nombre de usuario y contraseña de tu cuenta organizativa, y luego haz clic en "Sign In" (Iniciar sesión).

---

**Expandir paso**

**Abrir ArcGIS Urban**

Ahora que has iniciado sesión en tu cuenta organizativa de ArcGIS Online, accederás a ArcGIS Urban para crear un nuevo modelo.

En la parte superior de la página, haz clic en el botón "Apps" (Aplicaciones).

Selecciona "Urban".

_Nota: Si no tienes la opción de abrir ArcGIS Urban, verifica que tengas los permisos necesarios dentro de tu organización._

**Crear un modelo**

A continuación, crearás un nuevo modelo utilizando una plantilla vacía. El modelo se almacenará en tu contenido de ArcGIS Online.

Bajo "Create A New Model" (Crear un nuevo modelo), haz clic en "Set Up" (Configurar).

Bajo "Choose Model Location" (Elegir ubicación del modelo), escribe "Hardeeville, SC" y presiona Enter.

_Ver resultado_

El área del mapa se actualiza a Hardeeville, SC.

Desplázate hacia abajo hasta la sección "Template" (Plantilla).

Bajo "Template" (Plantilla), elige "Empty" (Vacío), si es necesario.

Bajo "Parcels" (Parcelas), haz clic en "Add" (Agregar).

Bajo "Search" (Búsqueda), haz clic en la flecha hacia abajo y elige "ArcGIS Online" (ArcGIS Online), si es necesario.

En el selector de elementos del portal, busca "owner:EsriTrainingSvc Hardeeville Parcels".

_Ver resultado_

Haz clic en la miniatura para seleccionar "Hardeeville Parcels" de "EsriTrainingSvc".

_Nota: No hagas clic en el título. Hacer clic en el título abre el elemento en lugar de seleccionarlo._

Haz clic en "Next" (Siguiente).

Acepta el ajuste de campo predeterminado y haz clic en "Next" (Siguiente).

ArcGIS Urban valida las 4,759 características de las parcelas.

Haz clic en "OK".

Bajo "Zoning" (Zonificación), haz clic en "Add" (Agregar).

Bajo "Search" (Búsqueda), haz clic en la flecha hacia abajo y elige "ArcGIS Online", si es necesario.

En el selector de elementos del portal, busca "owner:EsriTrainingSvc Hardeeville Zoning".

_Ver resultado_

Selecciona "Hardeeville Zoning" de "EsriTrainingSvc" y luego haz clic en "OK".

Haz clic en "OK".

**¿Cuántos tipos de zonificación válidos calculó ArcGIS Urban?**

_Ver respuesta_

ArcGIS Urban calculó 33 tipos de zonificación válidos.

Haz clic en "Create Urban Model" (Crear modelo urbano).

_Nota: Puede tomar unos minutos para que el modelo se cree._

_Ver resultado_

Tu nuevo modelo de ArcGIS Urban está creado y listo para que agregues datos de planificación.

Si continuarás con el siguiente ejercicio, deja abierto el modelo de Urban; de lo contrario, cierra tu navegador.


## Importar datos en un modelo de ArcGIS Urban

Imprimir ejercicio

Ahora que has creado un modelo de ArcGIS Urban de Hardeeville, Carolina del Sur, basado en una plantilla vacía, puedes agregar datos de planificación para crear el gemelo digital. Una excelente manera de comprender los datos en un modelo de Urban es importar cada uno de los tipos de datos, como los tipos de zonificación y los tipos de uso de suelo, así como las capas de entidades, en un modelo. En este ejercicio, primero agregarás los tipos de datos a través de diferentes métodos de importación y luego agregarás las capas de entidades al modelo.

**Tiempo estimado de finalización: 30 minutos**

Para completar los ejercicios, necesitarás lo siguiente:

-   Cuenta organizativa de ArcGIS Online
-   Rol de publicador o equivalente
-   ArcGIS Urban
-   Microsoft Excel 2007 o posterior

---

**Expandir todos los pasos**

---

**Contraer todos los pasos**

---

**Expandir paso**

**Descargar los datos**

Para completar el ejercicio, debes descargar los datos. Si ya has descargado e instalado los datos, continúa con el siguiente paso.

_¿No puedes encontrar los datos que descargaste?_

---

**Expandir paso**

**Abrir un modelo de Urban**

En el ejercicio anterior, creaste un modelo con una plantilla vacía. Ahora agregarás datos de planificación a ese modelo.

Vuelve a la pestaña del navegador web con tu modelo de Hardeeville, SC.

_¿Has cerrado el navegador web del ejercicio anterior?_

---

**Expandir paso**

**Agregar tipos de uso de espacio**

Con el modelo de Urban abierto, comenzarás agregando tipos de uso de espacio utilizando el método "Desde una tabla de entidades".

Desde la vista general, en la parte superior derecha, haz clic en el botón "Manage" (Administrar).

Se abrirá el administrador de datos.

Haz clic en "System Of Record" (Sistema de registro) y elige "Space Use Types" (Tipos de uso de espacio).

En el panel derecho, haz clic en "Add" (Agregar) y elige "From Feature Table" (Desde una tabla de entidades).

Se abrirá el selector de elementos del portal.

Cambia la ubicación de búsqueda a "ArcGIS Online", si es necesario.

En el campo de búsqueda, escribe "Hardeeville Space Use Types" y presiona Enter.

_Ver resultado_

Haz clic en la miniatura de "Hardeeville Space Use Types" para seleccionarlo.

Haz clic en "Next" (Siguiente).

Se abrirá el cuadro de diálogo "Field Matching" (Coincidencia de campos). Este cuadro de diálogo te permite hacer coincidir los campos del modelo con la tabla de origen.

Bajo "Units In Source" (Unidades en la fuente), haz clic en la flecha hacia abajo y elige "US Standard", si es necesario.

Acepta la coincidencia de campos predeterminada y haz clic en "Next" (Siguiente).

Aparecerá un mensaje que indica que se validaron e importaron 445 tipos de uso de espacio.

Haz clic en "OK".

_Ver resultado_

Los tipos de uso de espacio de la tabla de entidades se agregan.

---

**Expandir paso**

**Agregar tipos de edificios**

Cuando agregas zonificación a tu modelo durante el paso de creación, se agregan tipos de zonificación al sistema de registro. Verificarás que se hayan agregado los tipos de zonificación.

Desde la lista desplegable "System Of Record" (Sistema de registro), elige "Zoning Types" (Tipos de zonificación).

Verás la lista de tipos de zonificación que se agregaron al crear el modelo.

A continuación, agregarás tipos de edificios a tu modelo utilizando el método "Desde una hoja de cálculo".

Desde la lista desplegable "System Of Record" (Sistema de registro), elige "BuildingTypes" (Tipos de edificios).

Haz clic en "Add" (Agregar) y elige "From Spreadsheet" (Desde una hoja de cálculo).

En el cuadro de diálogo "From Spreadsheet: Building Types" (Desde una hoja de cálculo: Tipos de edificios), haz clic en "Choose File" (Elegir archivo).

Navega hasta C:\EsriTraining\UrbanImportPlanData, selecciona "Building-types.xlsx" y haz clic en "Open" (Abrir).

Acepta la coincidencia de campos predeterminada y haz clic en "OK".

Aparecerá un mensaje que indica que se validaron e importaron 41 tipos de edificios.

Haz clic en "OK" para cerrar los resultados.

_¿Cómo puedo acceder a la plantilla de tipos de datos?_

Has agregado datos de tipos de edificios utilizando el método "Desde una hoja de cálculo".

---

**Expandir paso**

**Agregar tipos de uso de suelo**

Ahora que has agregado tipos de edificios, agregarás tipos de uso de suelo utilizando el método de "elemento único". Antes de usar el método de "elemento único", cargarás algunos de los tipos de uso de suelo desde una hoja de cálculo.

Desde la lista desplegable "System Of Record" (Sistema de registro), elige "Land Use Types" (Tipos de uso de suelo).

Haz clic en "Add" (Agregar) y elige "From Spreadsheet" (Desde una hoja de cálculo).

Haz clic en "Choose File" (Elegir archivo) y navega hasta ..\EsriTraining\UrbanImportPlanData.

Selecciona "Land-use-types.xlsx" y haz clic en "Open" (Abrir).

Haz clic en "OK" para aceptar la coincidencia de campos predeterminada.

Se validan e importan diez tipos de uso de suelo.

Haz clic en "OK".

_Ver resultado_

Se agregan los primeros tipos de uso de suelo. Utilizarás el método de "elemento único" para agregar el resto de los tipos de uso de suelo. Agregarás el uso de suelo "Espacio abierto".

Haz clic en "Add" (Agregar) y elige "Single Item" (Elemento único).

En la pestaña "Appearance" (Apariencia), establece los siguientes parámetros:

-   Etiqueta: OS
-   ID personalizado: OS
-   Nombre: Espacio abierto
-   Descripción: Espacio abierto
-   Color: #00ff7f

En la pestaña "Parameters" (Parámetros), establece los siguientes parámetros:

-   Allowed Space Use Types (Tipos de uso de espacio permitidos): Elije "Other" (Otro).
-   Target Distribution (Distribución objetivo): Haz clic en "Other" (Otro) para ver el campo "Target Distribution" (Distribución objetivo), y luego escribe 100.

Haz clic en "OK".

A continuación, agregarás el uso de suelo "Residencial unifamiliar".

Haz clic en "Add" (Agregar) y elige "Single Item" (Elemento único).

En la pestaña "Appearance" (Apariencia), establece los siguientes parámetros:

-   Etiqueta: RES-SF
-   ID personalizado: RES-SF
-   Nombre: Residencial unifamiliar
-   Descripción: Residencial unifamiliar
-   Color: #ffffb7

En la pestaña "Parameters" (Parámetros), establece los siguientes parámetros:

-   Allowed Space Use Types (Tipos de uso de espacio permitidos): Elije "Residential Single-Family" (Residencial unifamiliar).
-   Target Distribution (Distribución objetivo): Haz clic en "Residential Single-Family" (Residencial unifamiliar) para ver el campo "Target Distribution" (Distribución objetivo), y luego escribe 100.

Haz clic en "OK".

Los dos tipos de uso de suelo que agregaste utilizando el método de "elemento único" ahora están en tu modelo.

---

**Expandir paso**

**Configurar datos de tipos**

Ahora que has agregado los datos de tipos utilizando varios métodos de importación, utilizarás el método de configuración para agregar tipos de estado de proyecto y categorías de retroalimentación.

Haz clic en el menú "Projects" (Proyectos) y elige "Project Status Types" (Tipos de estado de proyecto).

Haz clic en "Configure" (Configurar).

En el cuadro de diálogo "Project Status Types" (Tipos de estado de proyecto), haz clic en "Add Status" (Agregar estado).

Haz clic en "New Status" (Nuevo estado) y luego establece los siguientes parámetros:

-   Nombre: Aprobado.
-   Join ID: Aprobado.
-   Icono: Haz clic en la flecha hacia abajo y elige la marca de verificación verde (fila 4, columna 4).
-   Descripción: Proyectos que han sido aprobados para desarrollo.

_Ver resultado_

Haz clic en "OK".

Has agregado un tipo de estado de proyecto. Ahora estás listo para agregar capas de entidades.

---

**Expandir paso**

**Agregar capas de entidades**

Una vez que tienes los datos de tipos en su lugar, puedes agregar capas de entidades a tu modelo. Cuando creaste tu modelo, agregaste las capas de zonificación y parcelas; por lo tanto, no necesitarás agregar esas capas. Si no hubieras agregado esas capas durante el proceso de creación, podrías seguir estos pasos para agregar esas capas. Ahora terminarás de agregar las capas de entidades agregando una capa de polígonos que define los límites de uso de suelo futuro.

Haz clic en "System Of Record" (Sistema de registro) y elige "Land Use Boundaries" (Límites de uso de suelo).

Para "Future Land Use" (Uso de suelo futuro), haz clic en "Add" (Agregar).

Cambia la ubicación de búsqueda a "ArcGIS Online", si es necesario.

En el selector de elementos del portal, busca "owner:EsriTrainingSvc Hardeeville Future Land Use".

_Ver resultado_

Selecciona "Hardeeville Future Land Use" de EsriTrainingSvc y luego haz clic en "Next" (Siguiente).

En el cuadro de diálogo "Field Matching" (Coincidencia de campos), elige los siguientes parámetros:

-   Land Use Type (Tipo de uso de suelo): LandUseTyp
-   ID personalizado: -

Haz clic en "Next" (Siguiente).

Se validan 23 características de uso de suelo y se agrega la capa de uso de suelo a tu modelo.

Haz clic en "OK".

---

**Expandir paso**

**Configurar capas de superposición**

La última capa que se agregará son las superposiciones. Las superposiciones requieren que configures los tipos de superposición antes de agregar la geometría de polígono correspondiente.

Haz clic en "System Of Record" (Sistema de registro) y elige "Overlay Types" (Tipos de superposición).

Haz clic en "Add" (Agregar) y luego en "Single Item" (Elemento único).

En el cuadro de diálogo "New Overlay Type" (Nuevo tipo de superposición), en la pestaña "Appearance" (Apariencia), establece los siguientes parámetros:

-   Nombre: Corredor de entrada
-   Color: #000000
-   Relleno: Diagonal (hacia atrás)
-   Contorno: Sólido

Haz clic en la pestaña "Advanced Settings" (Configuración avanzada).

_¿Qué hacen las superposiciones con los parámetros de zonificación de forma predeterminada?_

Las superposiciones reemplazan los parámetros subyacentes de forma predeterminada.

Haz clic en "OK".

Has configurado los tipos de superposición. Ahora estás listo para agregar los límites de superposición.

Haz clic en "System Of Record" (Sistema de registro) y elige "Overlay Boundaries" (Límites de superposición).

Para "Gateway Corridor" (Corredor de entrada), haz clic en "Add" (Agregar).

Cambia la ubicación de búsqueda a "ArcGIS Online", si es necesario.

En el campo de búsqueda, escribe "owner:EsriTrainingSvc Hardeeville Overlays" y presiona Enter.

_Ver resultado_

Selecciona "Hardeeville Overlays" de EsriTrainingSvc y luego haz clic en "Next" (Siguiente).

Todos los campos se han coincidido con la capa de origen.

Haz clic en "Next" (Siguiente).

Aparecerá un mensaje que indica que se validaron e importaron 17 características de superposición.

Haz clic en "OK".

Has agregado exitosamente los datos de tipos y las capas de entidades a un modelo de Urban. Estos datos de planificación importados crean la base para tus planes y proyectos de Urban.

Cierra la pestaña del navegador web de Urban.

#### Preguntas de la lección

¿Qué puedes descargar para examinar los campos requeridos y los datos de entrada al configurar una hoja de cálculo para importarla en tu modelo de Urban?

Puedes descargar una plantilla de datos de tipos.

Después de importar los tipos de uso de espacio en tu modelo desde una hoja de cálculo, te das cuenta de que olvidaste agregar un tipo de uso de espacio. ¿Qué método te permitiría agregar el tipo de uso de espacio faltante a los datos existentes?

El método "Single Item" (Elemento único).

Un urbanista está creando un nuevo modelo de Urban. Después de elegir la opción de configurar un nuevo modelo de Urban, ¿qué acción debería tomar el urbanista a continuación?

Elegir una ubicación para el modelo.

Cuando se agregan datos de tipos a un modelo de Urban, ¿a qué tipo se pueden agregar iconos?

Al estatus de un proyecto