# Capítulo VI: Product Verification & Validation

## 6.1. Testing Suites & Validation

### 6.1.1. Core Entities Unit Tests.

Los Core Entities Unit Tests son esenciales en el desarrollo de software, ya que garantizan la calidad y
correcto funcionamiento de las entidades centrales, previniendo errores y facilitando el mantenimiento
del código.

**Todos los test**

![All_Test](../assets/chapter06/All_Test.png)

**Profile Service Test**

![UnitTest1](../assets/chapter06/UnitTest1.png)

**Report Service Test**

![UnitTest2](../assets/chapter06/UnitTest2.png)

**Shipment Service Test**

![UnitTest3](../assets/chapter06/UnitTest3.png)

**Vehicle Service Test**

![UnitTest4](../assets/chapter06/UnitTest4.png)

### 6.1.2. Core Integration Tests.

Las pruebas de integración central son esenciales para verificar que los controladores se comuniquen correctamente con los demás componentes del sistema, como los servicios y las bases de datos. Al incluir escenarios de fallo, estas pruebas aseguran que el sistema reaccione apropiadamente ante situaciones imprevistas y devuelva los códigos de estado correspondientes. Esto no solo optimiza la experiencia del usuario, sino que también simplifica el proceso de depuración y promueve el desarrollo de un software robusto y de calidad.

**Vehicle Creation Integration Test**

![IntegrationTest1](../assets/chapter06/Integral_Test_1.png)

**Vehicle Assigment Integration Test**

![IntegrationTest2](../assets/chapter06/Integral_Test_2.png)

**Shipment Creation Integration Test**

![IntegrationTest3](../assets/chapter06/Integral_Test_3.png)

**Shipment Alert Integration Test**

![IntegrationTest4](../assets/chapter06/Integral_Test_4.png)

**Restrict Acces Integration Test**

![IntegrationTest5](../assets/chapter06/Integral_Test_5.png)

### 6.1.3. Core Behavior-Driven Development

Modelo de todas las pruebas Behaviour-Driven Development realizadas en Cucumber

![All Gherkin Tests made with Cucumber](../assets/chapter06/gherkin-test-all.png)

Gherkin tests for individual User Stories. Puedes usar este link para revisar todas las pruebas Gherkin: https://github.com/upc-DisenoDeExperimentos-LosTesters/upc-DisenoDeExperimentos-LosTesters-Gherkin/blob/main/us-04-visualizacion-de-envios-asignados.feature

![Gherkin Test for US-1](../assets/chapter06/gherkin-test-us-1.png)

![Gherkin Test for US-3](../assets/chapter06/gherkin-test-us-3.png)

![Gherkin Test for US-5](../assets/chapter06/gherkin-test-us-5.png)

![Gherkin Test for US-7](../assets/chapter06/gherkin-test-us-7.png)

![Gherkin Test for US-9](../assets/chapter06/gherkin-test-us-9.png)

![Gherkin Test for US-11](../assets/chapter06/gherkin-test-us-11.png)

### 6.1.4. Core System Tests.

En este proyecto se utilizó Selenium para llevar a cabo las pruebas de Core System Tests. Esta herramienta permite automatizar interacciones con la aplicación a través de su interfaz, lo que facilita la validación del comportamiento de los controladores en conjunto con otros componentes clave del sistema, como los servicios y las bases de datos. Las pruebas realizadas aseguran que ante distintos escenarios incluidos aquellos con errores el sistema responda correctamente, mejorando así la experiencia del usuario, facilitando la depuración y contribuyendo al desarrollo de un software confiable y de alta calidad.

**Mobile**
![Mobile](../assets/chapter06/LightHouse_1.png)
![Mobile](../assets/chapter06/LightHouse_2.png)
![Mobile](../assets/chapter06/LightHouse_3.png)
![Mobile](../assets/chapter06/LightHouse_4.png)
![Mobile](../assets/chapter06/LightHouse_5.png)

**Desktop**

![Mobile](../assets/chapter06/LightHouse_Desktop_1.png)
![Mobile](../assets/chapter06/LightHouse_Desktop_2.png)
![Mobile](../assets/chapter06/LightHouse_Desktop_3.png)
![Mobile](../assets/chapter06/LightHouse_Desktop_4.png)


## 6.2. Static testing & Verification

### 6.2.1. Static Code Analysis

### 6.2.1.1. Coding stantard & Code conventions

### 6.2.1.2. Code Quality & Code Security

### 6.2.2. Reviews


## 6.3. Validations Interviews
Con el fin de obtener y separar correctamente toda la información obtenida durante las entrevistas, se optó por definir un banco de preguntas según nuestro segmento de mercado identificado anteriormente. Este grupo de preguntas está especializado para la obtención de información específica según la persona entrevistada y según la problemática investigada para el proyecto y la posible solución en la forma de nuestro producto.
### 6.3.1.  Diseño de Entrevistas
**Para los Empresarios:**

- ¿Cuál es su opinión general sobre la plataforma MoviGestion tras la demostración?
- ¿Qué características de MoviGestion le resultaron más útiles para la gestión de su flota?
- ¿Hay alguna función que no encontró en MoviGestion y que consideraría esencial para su operación?
- ¿Cómo evalúa la interfaz de usuario en términos de facilidad de uso y navegación?
- ¿Cuánto tiempo cree que le tomaría a su equipo adaptarse al uso de MoviGestion?
- ¿Cuáles son los principales desafíos que enfrenta actualmente en la gestión de su flota?
- ¿Cómo cree que MoviGestion podría ayudarle a superar esos desafíos?
- ¿Qué tan útil considera la funcionalidad de registro de incidencias en la plataforma?
- ¿Qué aspectos de la gestión de envíos exitosos le parecen más críticos para su operación?
- ¿Está dispuesto a recomendar MoviGestion a otros empresarios del sector? ¿Por qué?
- ¿Cómo valora la seguridad de la información y los datos en la plataforma MoviGestion?

**Para los Transportistas:**

- ¿Cuál fue su impresión general de la plataforma MoviGestion después de la demostración?
- ¿Qué tan fácil le resultó navegar y utilizar las funciones de MoviGestion?
- ¿Qué características de MoviGestion le parecieron más útiles para su trabajo diario?
- ¿Hay alguna función que no encontró en MoviGestion y que consideraría útil para su labor?
- ¿Cómo cree que MoviGestion podría ayudarle a realizar su trabajo de manera más eficiente?
- ¿Qué tan útil considera la funcionalidad de registro de incidencias para reportar problemas en tiempo real?
- ¿Qué tan fácil le resultó el proceso de seguimiento de envíos en MoviGestion?
- ¿Cómo valora la capacidad de monitorear los sitios de entrega a través de la plataforma?
- ¿Le parece intuitiva la interfaz de usuario de MoviGestion? ¿Hay algo que cambiaría?
- ¿Cómo le gustaría que MoviGestion le notificara sobre nuevas tareas o cambios en las entregas?
- ¿Qué mejoras le gustaría ver en futuras actualizaciones de la plataforma?
- ¿Cómo valora la seguridad de la información y los datos en la plataforma MoviGestion?
- ¿Cree que MoviGestion le ayudaría a reducir el tiempo de inactividad y aumentar la productividad?
- ¿Estaría dispuesto a recomendar MoviGestion a otros transportistas? ¿Por qué?

### 6.3.2.  Registro de Entrevistas

1. ### <a name="_heading=h.mqpm42spx03x"></a>***Segmento objetivo: Empresarios***
   **Entrevista N°1:**

   
![Entrevsita 1](/assets/chapter02/interview-3.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Abraham Quenta
- **Edad:** 28 años
- **Distrito:** Tacna
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de la entrevista:** 0:00
- **Duración:** 10:45
- **Resumen:** Abraham se presenta como un profesional del transporte con 5 años de experiencia en el sector transporte provincial, cuya ruta principal es de Tacna a Puno. Comenta sobre la página de destino de su servicio, que incluye información sobre los servicios ofrecidos y permite la personalización del idioma. Abraham explora las características y funcionalidades del sitio web, como la gestión de la flota, los informes de los conductores y la gestión de vehículos, y aprecia el aspecto organizativo de la plataforma, señalando que es fácil encontrar las funciones deseadas. Abraham menciona algunos problemas menores con la visibilidad del texto y la navegación, pero en general considera que la interfaz de usuario es clara y sencilla. información del vehículo, así como las estrategias de marketing y el diseño de la página de destino, pero en general. considera que la aplicación es valiosa, especialmente para monitorear las actividades de los conductores.

**Entrevista N°2:**

![Entrevista 2](/assets/chapter02/interview-1.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Gustavo Manrique
- **Edad:** 40 años
- **Distrito: Chorrillos**
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de la entrevista:** 10:46
- **Duración:** 6:40
- **Resumen:** El empresario Gustavo Manrique expresó una opinión muy bien sobre MoviGestion, destacando la utilidad de las estadísticas de rendimiento y el seguimiento de envíos exitosos. Considera que la plataforma es fácil de usar y que su equipo podría adaptarse rápidamente. También, identificó como desafíos principales el seguimiento de envíos, gestión de incidencias y optimización de rutas, áreas donde cree que MoviGestion puede ayudar significativamente. Mencionó la necesidad de una herramienta para la optimización de rutas en tiempo real. Valora altamente la seguridad de la información y está dispuesto a recomendar la plataforma a otros empresarios del sector.


**Entrevista N°3:**

![Entrevsita3](/assets/chapter02/interview-2.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Marco Tarazona
- **Edad:** 57 años
- **Distrito:** Puente Piedra
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de la entrevista:** 17:34
- **Duración:** 2:17
- **Resumen:** El empresario Marco Tarazona expresó una opinión positiva sobre MoviGestion, resaltando su utilidad para la gestión de flotas, especialmente en el seguimiento de envíos y la gestión de incidencias. Mencionó la facilidad de uso de la plataforma y consideró que su equipo podría adaptarse rápidamente. Identificó como posible desafio la optimización de rutas y la necesidad de integración con otros sistemas. Además, valora la seguridad de la información y está dispuesto a recomendar MoviGestion a otros empresarios del sector.



**Segmento objetivo: Transportistas**

**Entrevista N°1:**

![Entrevsita 4](/assets/chapter02/interview-4.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Renzo Cesar Silva Morales
- **Edad:** 24 años
- **Distrito:** Santiago de Surco
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 19:43
- **Duración:** 7:50
- **Resumen:** Renzo es un transportista que recién está comenzando en el negocio, tuvo una experiencia inicial positiva con la plataforma. En donde destaca las secciones que tenemos implementadas por su funcionalidad. La interfaz le pareció amigable y fácil de usar, pero encontró algunas dificultades técnicas. Considera que sería beneficioso añadir seguimiento en tiempo real para envíos, notificaciones automáticas y soporte por chat en vivo. Aunque las opciones actuales son útiles, a él le gustaría tener más información detallada en cada apartado. Por último, sugiere la inclusión de tutoriales interactivos para que los nuevos usuarios puedan familiarizarse.

**Entrevista N°2:**

![Entrevsita 5](/assets/chapter02/interview-5.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Ricardo Chate Flores
- **Edad:** 45 años
- **Distrito:** Cercado de Lima
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 28:01
- **Duración:** 8:00
- **Resumen:** El transportista Ricardo Chate Flores expresó una opinión positiva sobre MoviGestion, destacando su facilidad de uso y navegación intuitiva. Consideró útiles las funciones de registro de incidencias y seguimiento de envíos para su trabajo diario. Valora la capacidad de monitorear los sitios de entrega y mencionó que la plataforma podría ayudarle a trabajar de manera más eficiente. Aunque satisfecho con las funcionalidades actuales, sugirió la necesidad de notificaciones más personalizables. José destacó la seguridad de la información y está dispuesto a recomendar MoviGestion a otros transportistas, ya que cree que puede reducir el tiempo de inactividad y aumentar la productividad.

**Entrevista N°3:**

![Entrevsita 6](/assets/chapter02/interview-6.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Víctor Cuba Bautista
- **Edad:** 42 años
- **Distrito:** Villa El Salvador
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 35:37
- **Duración:** 4:50
- **Resumen:** El transportista Víctor Cuba Bautista tras probar la plataforma, reconoció que el uso de las funciones eran más sencillos de lo que esperaba. Encontró especialmente útil el registro de incidencias en tiempo real. Aunque le gustaría ver mejoras en algunas funcionalidades adicionales, valora la capacidad de monitorear los sitios de entrega y la seguridad de los datos proporcionada por la plataforma. Al final, Víctor concluyó que MoviGestion es una herramienta efectiva que puede mejorar su eficiencia y reducir el tiempo de inactividad, y estaría dispuesto a recomendarla a otros transportistas.


### 6.3.3.  Evaluaciones según heurísticas

Esta sección contiene el proceso de evaluación de las sesiones de validación basado en heurísticas, considerando heurísticas de usabilidad, arquitectura de información e inclusive design de la experiencia propuesta. Para esto la sección usamos la estructura del formato para evaluaciones de heurísticas indicado.


**UX Heuristics & Principles Evaluation**

**Usability – Inclusive Design – Information Architecture**
\***


**CARRERA                	: Ingeniería de Software**

**CURSO                    	: Aplicaciones Web**

**SECCIÓN                   	: SV51**

**PROFESORES         	: Angel Augusto Velasquez Nuñez**

**AUDITOR                 	: Bicas Team**

**CLIENTE                  	: MoviGestion**
1. ## <a name="_heading=h.3ibjgvegxoc5"></a>** 
   **SITE o APP A EVALUAR:**

   **MoviGestion**

   **TAREAS A EVALUAR:**

   *El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:*

*1.* 	*Gestión y edición de perfil de usuario.*

*2.     Visualización de asignación de envíos que pertenecen a cada transportista*

*3. 	Agregar un nuevo vehículo a la flota de vehículos.*

*4. 	Eliminar un vehículo de la flota de vehículos.*

*5. 	Visualización de alertas de cada transportista.*

**ESCALA DE SEVERIDAD:**

*Los errores serán puntuados tomando en cuenta la siguiente escala de severidad*

|***Nivel***|***Descripción***|
| :- | :- |
|*1*|*Problema superficial: puede ser fácilmente superado o hasta ignorado por el usuario ó ocurre con muy poca frecuencia. El error no necesita ser arreglado de forma inmediata en la mayoría de las casos, a no ser que exista disponibilidad de tiempo.*|
|*2*|*Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja para resolverlo de cara antes de la siguiente entrega o actualización.*|
|*3*|*Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta.*|
|*4*|*Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento.*|


**TABLA RESUMEN:**

|*#*|*Problema*|*Escala de severidad*|*Heurística/Principio violada(o)*|
| :-: | :-: | :-: | :-: |
|*1*|*Incluye un botón “See More” pero no tiene funcionalidad*|*3*|*Information Architecture: Is it usable?*|
|*2*|*No parece haber consistencia en la forma en que se presentan las opciones para actualizar la información*|*2*|*Usability: Consistencia y estándares*|
|*3*|*Información de pagos no está claramente presentada*|*3*|*Usability: Visibilidad del estado del sistema*|
|*4*|*No funciona cancelar el agregado de un vehículo.*|*2*|*Usability: Libertad y control del usuario*|





**DESCRIPCIÓN DE PROBLEMAS:**

*PROBLEMA #1:* 

*Severidad: 3*

*Heurística violada: Information Architecture: Is it usable?*

*Problema:*

*La aplicación incluye un botón “See More” pero no tiene funcionalidad, lo que confunde a los usuarios y les impide acceder a contenido adicional esperado.*

![H1](/assets/chapter06/h1.png)

*Recomendación:*

*Eliminar el botón “See More” si no hay contenido adicional disponible, o implementar la funcionalidad esperada para que los usuarios puedan acceder a más información.*

*PROBLEMA #2:* 

*Severidad: 2*

*Heurística violada: Usability - Consistencia y estándares*

*Problema:*

*La interfaz de Settings incluye campos para Nickname, Bio, Email y Avatar, pero no parece haber consistencia en la forma en que se presentan las opciones para actualizar la información. Por ejemplo, el botón ‘Choose’ para actualizar el avatar está separado del campo ‘Avatar’, lo que podría confundir a los usuarios.*

![H2](/assets/chapter06/h2.png)

*Recomendación:*

*Asegurar que todos los campos de entrada y botones relacionados estén agrupados de manera coherente y clara para mejorar la comprensión y la facilidad de uso.*

*PROBLEMA #3:* 

*Severidad: 3*

*Heurística violada: Usability: Visibilidad del estado del sistema*

*Problema:*

*La información relacionada con Organization no está claramente presentada, lo que puede causar confusión a la hora de querer tener información y dificulta la asignación de envíos.*

![H3](/assets/chapter06/h3.png)

*Recomendación:*

*Mejorar la presentación y accesibilidad de la información relacionada con "Organization" puede mejorar significativamente la experiencia del usuario y facilitar la asignación de envíos en la aplicación.* 

*PROBLEMA #4:* 

*Severidad: 2*

*Heurística violada: Usability: Libertad y control del usuario*

*Problema:*

*Al momento de ingresar los datos del nuevo vehículo, no se puede cerrar hasta darle darle al botón “Close” y luego se tiene que eliminar en el botón “Delete Vehicle”, esto obliga a agregar nuevos carros no deseados, también incrementando así la cantidad de esfuerzo del usuario.*

![H4](/assets/chapter06/h4.png)

*Recomendación:*

*Hacer que el botón "Close" tenga la funcionalidad para cerrar la ventana emergente sin guardar los datos del vehículo ingresados.*

---
