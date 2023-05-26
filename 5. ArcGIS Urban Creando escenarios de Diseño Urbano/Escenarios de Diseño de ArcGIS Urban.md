  
## Creando un modelo ArcGIS Urban 

El flujo de trabajo del modelo ArcGIS Urban consta de cinco pasos principales. Después de iniciar sesión en ArcGIS Online utilizando una cuenta con una licencia Urban, creas el modelo Urban a partir de una plantilla. Luego, gestionas los ajustes del modelo e importas tus datos de planificación al modelo. Con los datos añadidos, puedes crear escenarios de diseño urbano utilizando planes y proyectos. Finalmente, puedes compartir y colaborar con otros usando tu nuevo modelo Urban. Este curso se centra en el cuarto paso: creación de escenarios de diseño urbano utilizando planes y proyectos.

Rectángulos apilados representando los pasos del flujo de trabajo El flujo de trabajo de ArcGIS Urban tiene cinco pasos principales: crear un nuevo modelo Urban, gestionar los ajustes del modelo, importar los datos de planificación, crear escenarios de diseño urbano y compartir y colaborar.

## Tipos de escenarios de diseño 

Una vez que hayas creado un modelo de ArcGIS Urban, gestionado los ajustes e importado los datos de planificación, puedes crear escenarios de diseño. Se utilizan dos tipos de escenarios de diseño en ArcGIS Urban: proyectos y planes. Los proyectos son para procesos de planificación a corto plazo (de 1 a 5 años) a nivel de parcela, mientras que los planes son para procesos de planificación a largo plazo (de 10 a 50 años) a escalas más grandes.

### Proyectos 

Un proyecto es un escenario de diseño compuesto por un modelo 3D que visualiza características como terreno, edificios, árboles, vehículos y mobiliario urbano. Por ejemplo, se pueden añadir varias propuestas de edificios a un solo proyecto como escenarios individuales.

Gráfico conceptual de tres edificios organizados dentro de un proyecto Los proyectos de ArcGIS Urban pueden estar compuestos por múltiples escenarios.

Cada proyecto puede mostrar un modelo detallado de información de edificios. Los modelos de proyectos se sitúan dentro del contexto de su entorno real para permitir la comparación de escenarios. Poder revisar cada escenario en el contexto de la condición actual del área del proyecto ayuda al público y a los interesados en la toma de decisiones. Urban también organiza los proyectos para facilitar la gestión de sus estados.

![[Pasted image 20230524171332.png]]

### Planes 

Un plan es un escenario de diseño para actividades de planificación a largo plazo. Los planes proporcionan el conjunto de herramientas necesario para analizar y comparar diferentes escenarios. Puedes crear dos tipos de planes en ArcGIS Urban: uso de suelo y zonificación. Los planes de uso de suelo se utilizan para desarrollar planes generales basados en el uso futuro designado de una parcela. Los planes de zonificación se utilizan para desarrollar planes extensos basados en cómo se puede utilizar una parcela. Aunque los planes de zonificación son más detallados que los planes de uso de suelo, un plan de zonificación puede ser validado contra un plan de uso de suelo.

Gráfico conceptual de seis edificios organizados dentro de un plan Los planes de ArcGIS Urban pueden tener múltiples escenarios de desarrollo.

Los planes ayudan a cuantificar y comunicar cómo los cambios propuestos, basados en escenarios, podrían contribuir a los objetivos estimados generales, como las demandas de vivienda y el crecimiento de la población dentro de una ciudad. Los escenarios de planificación urbana pueden ser examinados para determinar el efecto de varios cambios en otras métricas, como las emisiones de CO2, la disponibilidad de aparcamiento y la producción de residuos sólidos.

Los planes también permiten aplicar digitalmente las regulaciones de zonificación y ajustarlas en función de los escenarios. Esta zonificación digital crea visualizaciones 3D de los parámetros de zonificación mostrando un sobre máximo y la forma del edificio.

![[Pasted image 20230524171340.png]]


### Métricas en ArcGIS Urban 

# Métricas de ArcGIS Urban

Ahora exploraremos cómo se pueden utilizar las métricas para comparar escenarios. Cada modelo Urban tiene su propio conjunto de métricas que pueden ser llenadas con valores llamados valores de métricas. A medida que creas proyectos y planes, puedes añadir métricas adicionales. Una métrica define el cálculo de valores numéricos dentro de los escenarios de diseño y consta de una fuente de métrica o valor de métrica existente. Cuando se utilizan fuentes de métricas, los valores se agregan como una suma ponderada. También puedes añadir métricas personalizadas introduciendo tus propios valores. El panel proporciona una forma de visualizar métricas para planes y proyectos. Cuando cambias entre escenarios, los valores de las métricas se actualizan en el panel para reflejar los cambios.

![[Pasted image 20230524172233.png]]

# Cálculo de métricas de escenarios de diseño

Las métricas juegan un papel importante en los escenarios de diseño. Al comparar escenarios, las métricas te permiten cuantificar y analizar los escenarios. Cuando creas un proyecto o un plan, las métricas se copian de tu modelo Urban. También puedes añadir métricas manualmente a los proyectos y planes. Las métricas se configuran de manera diferente dependiendo de si los valores son para proyectos o planes.

## Métricas de proyectos

Cuando creas un proyecto, las métricas se copian de tu modelo Urban. Además, se pueden añadir métricas manualmente desde el editor de proyectos. Sin embargo, los valores de las métricas de tu modelo Urban no se copiarán a tu proyecto; necesitarás editar el panel para cada escenario de proyecto para añadir los valores de las métricas.

## Métricas de planes

De manera similar a un proyecto, cuando creas un plan, las métricas de tu modelo Urban se copian y también se pueden añadir manualmente desde el editor de planes. Cualquier valor de métrica en tu modelo Urban también se copiará a tu plan. Puedes editar los valores de las métricas para un plan en el panel o configurar los valores de las métricas utilizando un gráfico de dependencias para crear cálculos.

Un gráfico de dependencias es un gráfico que crea conexiones entre métricas y define cómo las métricas dependen unas de otras.

![[Pasted image 20230524172343.png]]

_Los valores de las métricas de los planes se pueden explorar y configurar utilizando un gráfico de dependencias._

El área de espacio neto está definida por los tipos de uso del espacio del plan. Todos los cálculos de las métricas comienzan con el área de espacio neto como entrada. Luego, cada métrica se calcula utilizando un peso basado en la fuente. La métrica ponderada comienza con las condiciones existentes y luego se calcula en función de los cambios del escenario del plan.

Por ejemplo, considera un área de plan que tiene 50 hogares existentes con un área de uso de espacio neto de 4 millones de pies cuadrados. La dependencia de los hogares se establece en 1 hogar por cada 40,000 pies cuadrados. El cálculo ponderado sería 4 millones de pies cuadrados divididos por 40,000 pies cuadrados. El resultado sería 100 hogares nuevos, con un total de 150 hogares.


![[Pasted image 20230524172355.png]]


