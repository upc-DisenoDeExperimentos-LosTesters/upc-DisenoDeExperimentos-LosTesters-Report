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

El análisis estático del código es un pilar fundamental en la metodología de desarrollo de MoviGestión. Consiste en la inspección automatizada del código fuente sin necesidad de ejecutarlo, con el objetivo primordial de identificar tempranamente fallos potenciales, vulnerabilidades de seguridad y desviaciones de las buenas prácticas de programación. Este enfoque proactivo es vital para mantener una base de código robusta, optimizar la eficiencia del desarrollo y reducir la acumulación de deuda técnica a lo largo del ciclo de vida del proyecto. Dado que MoviGestión abarca un frontend web con Vue.js, un backend en .NET Framework y una aplicación móvil con Flutter, la estrategia de análisis estático se adapta a las particularidades de cada ecosistema tecnológico.

### 6.2.1.1. Coding stantard & Code conventions

La consistencia en el estilo y las convenciones de codificación es crucial para la legibilidad, mantenibilidad y la colaboración efectiva dentro del equipo de MoviGestión. Establecer y adherirse a un conjunto claro de directrices asegura que el código sea uniforme, fácil de comprender y modificar por cualquier desarrollador, independientemente de la tecnología específica. En MoviGestión, nos guiamos por los siguientes principios clave:

- Claridad y Expresividad: Adoptamos la filosofía de que el código debe ser autoexplicativo siempre que sea posible. Esto implica el uso de nombres completos y significativos para variables, funciones, clases y componentes, que reflejen claramente su propósito y el dominio de negocio (gestión de flotas, envíos, incidencias). Se prioriza la legibilidad sobre la brevedad, buscando que el flujo lógico del programa sea evidente a simple vista.<br><br>
- Modularidad y Responsabilidad Única: Cada unidad de código (ya sea una función en Vue.js, un método en C# o un widget en Flutter) debe tener una única responsabilidad bien definida. Esto promueve la creación de componentes y servicios pequeños, cohesivos y fáciles de probar y mantener. En el backend de .NET, esto se manifiesta en una clara separación de capas; en el frontend web, en componentes Vue reutilizables; y en la aplicación Flutter, en la descomposición de la interfaz de usuario en widgets manejables.<
- Uniformidad Estructural: Se establecen reglas específicas para el formato del código, incluyendo la indentación, el uso de espacios, la colocación de llaves y la organización de importaciones. Esta uniformidad, aplicada transversalmente en todos los lenguajes y frameworks de MoviGestión, elimina distracciones visuales y permite a los desarrolladores enfocarse en la lógica de negocio, no en las diferencias de estilo. Se utilizan herramientas de formato automatizadas para garantizar la adherencia constante a estas convenciones.

### 6.2.1.2. Code Quality & Code Security

Garantizar la alta calidad y la robustez del código es fundamental para la fiabilidad de MoviGestión, un sistema que gestiona operaciones críticas de flotas. Esto implica no solo la ausencia de errores, sino también la eficiencia, escalabilidad y seguridad inherente de la solución.

- **Excelencia Técnica y Métricas:** La calidad del código se evalúa y se busca optimizar de forma continua. Esto incluye monitorear métricas como la complejidad ciclomática, que indica la intrincación de los flujos de control del código, y la densidad de "code smells", que señala áreas con posibles problemas de diseño o mantenibilidad. La cobertura de pruebas automatizadas es otra métrica esencial, asegurando que las funcionalidades críticas de MoviGestión estén debidamente validadas. La plataforma SonarQube juega un rol clave en este monitoreo, proporcionando un panorama integral del "estado de salud" del código en todos los módulos del proyecto (Vue.js, .NET, Flutter). <br><br>
- **Seguridad Intrínseca:** La seguridad es diseñada desde las primeras fases de desarrollo. Se implementan prácticas de codificación defensiva para mitigar vulnerabilidades comunes que podrían afectar la integridad de los datos de la flota o la privacidad de los usuarios. Esto incluye:
  - **Validación Rigurosa de Entradas:** Asegurar que todas las entradas de usuario, tanto en el frontend como en el backend, sean validadas y sanitizadas para prevenir ataques como inyección SQL, XSS o path traversal.
  - **Gestión Segura de Dependencias:** Realizar un escaneo regular de las bibliotecas y paquetes de terceros utilizados en Vue.js, .NET y Flutter para detectar y actualizar versiones con vulnerabilidades conocidas.
  - **Principios de Menor Privilegio:** Diseñar el acceso a los recursos y datos con el principio de mínimo privilegio, asegurando que los usuarios y los componentes del sistema solo tengan los permisos estrictamente necesarios. <br><br>
- **Integración de Detección Temprana (SonarLint):** Para infundir una cultura de calidad y seguridad directamente en el flujo de trabajo diario de los desarrolladores, se utiliza SonarLint. Esta extensión se integra directamente en los IDEs y proporciona retroalimentación instantánea sobre problemas de calidad y seguridad mientras el código está siendo escrito. Esto permite a los desarrolladores identificar y corregir posibles fallos de diseño, errores o vulnerabilidades en el momento de su creación, reduciendo la necesidad de correcciones costosas en etapas posteriores del desarrollo.

### 6.2.2. Reviews

Las revisiones de código son un pilar colaborativo en el proceso de desarrollo de MoviGestión, actuando como un complemento indispensable al análisis estático automatizado. Este proceso implica que los desarrolladores examinen y evalúen el código fuente escrito por sus compañeros.

- **Propósitos Fundamentales:**

  - **Validación de Lógica y Diseño:** Ir más allá de los problemas superficiales para identificar errores lógicos sutiles, ineficiencias o deficiencias en el diseño arquitectónico que las herramientas automáticas podrían pasar por alto.<br><br>
  - **Refuerzo de Estándares:** Asegurar que el código no solo sea funcional, sino que también se adhiera a los principios de Clean Code, Modularidad y Uniformidad definidos para MoviGestión.<br><br>
  - **Fomento de la Seguridad Contextual:** Un par de ojos humanos puede identificar vulnerabilidades de seguridad más complejas o específicas del dominio de la aplicación que no son detectables por patrones genéricos de análisis estático.<br><br>
  - **Intercambio de Conocimiento:** Servir como una herramienta de aprendizaje y mentoría, permitiendo que el conocimiento sobre la base de código y las mejores prácticas se difunda entre el equipo, reduciendo la dependencia de un solo experto.<br><br>
  - **Mejora Continua:** Impulsar una cultura de mejora constante, donde los comentarios constructivos llevan a soluciones más robustas, legibles y mantenibles. <br><br>
  - **Metodología de Revisión en MoviGestión (Pull/Merge Requests):**
    Las revisiones en MoviGestión se articulan principalmente a través del proceso de Pull Requests (PRs) o Merge Requests (MRs), una práctica estándar en el desarrollo moderno basado en Git.

**Flujo Operativo:**

1 . Cuando un desarrollador completa una tarea (sea una nueva funcionalidad para envíos, una mejora en la interfaz de reportes de incidentes, o una corrección en el backend de gestión de vehículos), crea un Pull Request. Este PR propone la integración de sus cambios en la rama de desarrollo principal.<br><br>

2 . El PR es asignado a uno o más desarrolladores para su revisión. Estos revisores son responsables de analizar el código propuesto.<br><br>

3 . La revisión abarca una evaluación exhaustiva, considerando aspectos como: - La claridad y la documentación interna del código. - La adhesión a los principios de diseño y arquitectura de MoviGestión. - La eficiencia y el rendimiento de las soluciones implementadas (ej. consultas a base de datos, lógica de procesamiento). - El manejo adecuado de errores, casos excepcionales y la robustez ante entradas inesperadas. - La calidad y la cobertura de las pruebas unitarias y de integración asociadas al cambio. - La seguridad del código, buscando posibles vulnerabilidades o malas prácticas. - El impacto potencial del cambio en otras partes del sistema.<br>

4 . Los comentarios y sugerencias se realizan directamente en la plataforma del PR, facilitando el diálogo entre el autor y los revisores.<br>
5 . El autor del PR es responsable de incorporar la retroalimentación y realizar las modificaciones necesarias hasta que el código satisfaga los estándares y reciba la aprobación de los revisores.<br>
6 . Una vez aprobado, el código es fusionado en la rama de desarrollo, integrándose en la base de código de MoviGestión.<br>

- **Herramientas de Soporte:** La gestión de estos Pull Requests se realiza a través de la plataforma de control de versiones utilizada por el equipo, GitHub, que provee las herramientas necesarias para la colaboración, los comentarios en línea y el seguimiento del estado de cada revisión.<br><br>

- **Periodicidad:** Las revisiones de código son un proceso continuo e integral, que se activa con cada propuesta de cambio significativo al codebase, garantizando un flujo de trabajo ágil que prioriza la calidad y la colaboración.

## 6.3. Validations Interviews

Con el fin de obtener y separar correctamente toda la información obtenida durante las entrevistas, se optó por definir un banco de preguntas según nuestro segmento de mercado identificado anteriormente. Este grupo de preguntas está especializado para la obtención de información específica según la persona entrevistada y según la problemática investigada para el proyecto y la posible solución en la forma de nuestro producto.

### 6.3.1. Diseño de Entrevistas

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

### 6.3.2. Registro de Entrevistas

1. ### <a name="_heading=h.mqpm42spx03x"></a>**_Segmento objetivo: Empresarios_**
   **Entrevista N°1:**

![Entrevsita de validación 1](/assets/chapter02/interview-3.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Abraham Quenta
- **Edad:** 28 años
- **Distrito:** Tacna
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de la entrevista:** 0:00
- **Duración:** 10:45
- **Resumen:** Abraham se presenta como un profesional del transporte con 5 años de experiencia en el sector transporte provincial, cuya ruta principal es de Tacna a Puno. Comenta sobre la página de destino de su servicio, que incluye información sobre los servicios ofrecidos y permite la personalización del idioma. Abraham explora las características y funcionalidades del sitio web, como la gestión de la flota, los informes de los conductores y la gestión de vehículos, y aprecia el aspecto organizativo de la plataforma, señalando que es fácil encontrar las funciones deseadas. Abraham menciona algunos problemas menores con la visibilidad del texto y la navegación, pero en general considera que la interfaz de usuario es clara y sencilla. información del vehículo, así como las estrategias de marketing y el diseño de la página de destino, pero en general. considera que la aplicación es valiosa, especialmente para monitorear las actividades de los conductores.

**Entrevista N°2:**

![Entrevista de validación 2](/assets/chapter02/interview-1.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Gustavo Manrique
- **Edad:** 40 años
- **Distrito: Chorrillos**
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de la entrevista:** 10:46
- **Duración:** 6:40
- **Resumen:** El empresario Gustavo Manrique expresó una opinión muy bien sobre MoviGestion, destacando la utilidad de las estadísticas de rendimiento y el seguimiento de envíos exitosos. Considera que la plataforma es fácil de usar y que su equipo podría adaptarse rápidamente. También, identificó como desafíos principales el seguimiento de envíos, gestión de incidencias y optimización de rutas, áreas donde cree que MoviGestion puede ayudar significativamente. Mencionó la necesidad de una herramienta para la optimización de rutas en tiempo real. Valora altamente la seguridad de la información y está dispuesto a recomendar la plataforma a otros empresarios del sector.

**Entrevista N°3:**

![Entrevsita de validación 3](/assets/chapter02/interview-2.png)

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

![Entrevsita de validación 4](/assets/chapter02/interview-4.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Renzo Cesar Silva Morales
- **Edad:** 24 años
- **Distrito:** Santiago de Surco
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 19:43
- **Duración:** 7:50
- **Resumen:** Renzo es un transportista que recién está comenzando en el negocio, tuvo una experiencia inicial positiva con la plataforma. En donde destaca las secciones que tenemos implementadas por su funcionalidad. La interfaz le pareció amigable y fácil de usar, pero encontró algunas dificultades técnicas. Considera que sería beneficioso añadir seguimiento en tiempo real para envíos, notificaciones automáticas y soporte por chat en vivo. Aunque las opciones actuales son útiles, a él le gustaría tener más información detallada en cada apartado. Por último, sugiere la inclusión de tutoriales interactivos para que los nuevos usuarios puedan familiarizarse.

**Entrevista N°2:**

![Entrevsita de validación 5](/assets/chapter02/interview-5.png)

- **Datos principales:**
- **Nombre completo del entrevistado:** Ricardo Chate Flores
- **Edad:** 45 años
- **Distrito:** Cercado de Lima
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 28:01
- **Duración:** 8:00
- **Resumen:** El transportista Ricardo Chate Flores expresó una opinión positiva sobre MoviGestion, destacando su facilidad de uso y navegación intuitiva. Consideró útiles las funciones de registro de incidencias y seguimiento de envíos para su trabajo diario. Valora la capacidad de monitorear los sitios de entrega y mencionó que la plataforma podría ayudarle a trabajar de manera más eficiente. Aunque satisfecho con las funcionalidades actuales, sugirió la necesidad de notificaciones más personalizables. José destacó la seguridad de la información y está dispuesto a recomendar MoviGestion a otros transportistas, ya que cree que puede reducir el tiempo de inactividad y aumentar la productividad.

**Entrevista N°3:**

![Entrevista de validación 6](/assets/chapter02/interview-6.jpeg)

- **Datos principales:**
- **Nombre completo del entrevistado:** Víctor Cuba Bautista
- **Edad:** 42 años
- **Distrito:** Villa El Salvador
- **Link:** https://upcedupe-my.sharepoint.com/:v:/g/personal/u20191a453_upc_edu_pe/ERl5IIXzz4FArsqJHHlEohABGg35OtX4K-X123ewVpRjIw?e=k2DFxD&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- **Inicio de entrevista:** 35:37
- **Duración:** 4:50
- **Resumen:** El transportista Víctor Cuba Bautista tras probar la plataforma, reconoció que el uso de las funciones eran más sencillos de lo que esperaba. Encontró especialmente útil el registro de incidencias en tiempo real. Aunque le gustaría ver mejoras en algunas funcionalidades adicionales, valora la capacidad de monitorear los sitios de entrega y la seguridad de los datos proporcionada por la plataforma. Al final, Víctor concluyó que MoviGestion es una herramienta efectiva que puede mejorar su eficiencia y reducir el tiempo de inactividad, y estaría dispuesto a recomendarla a otros transportistas.

### 6.3.3. Evaluaciones según heurísticas

Esta sección contiene el proceso de evaluación de las sesiones de validación basado en heurísticas, considerando heurísticas de usabilidad, arquitectura de información e inclusive design de la experiencia propuesta. Para esto la sección usamos la estructura del formato para evaluaciones de heurísticas indicado.

**UX Heuristics & Principles Evaluation**

**Usability – Inclusive Design – Information Architecture**

**CARRERA : Ingeniería de Software**

**CURSO : Diseño de Experimentos de Ingeniería de Software**

**SECCIÓN : 4441**

**PROFESORES : Julio Manuel Noriega Melendez**

**AUDITOR : EventWine**

**CLIENTE : LosTesters**

**SITE o APP A EVALUAR:**

**MoviGestion**

**TAREAS A EVALUAR:**

_El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:_

_1._ _Gestión y edición de perfil de usuario._

_2. Visualización de asignación de envíos que pertenecen a cada transportista_

_3. Agregar un nuevo vehículo a la flota de vehículos._

_4. Eliminar un vehículo de la flota de vehículos._

_5. Visualización de alertas de cada transportista._

**ESCALA DE SEVERIDAD:**

_Los errores serán puntuados tomando en cuenta la siguiente escala de severidad_

| **_Nivel_** | **_Descripción_**                                                                                                                                                                                                                                     |
| :---------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1           | Problema superficial: puede ser fácilmente superado o hasta ignorado por el usuario ó ocurre con muy poca frecuencia. El error no necesita ser arreglado de forma inmediata en la mayoría de las casos, a no ser que exista disponibilidad de tiempo. |
| 2           | Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja para resolverlo de cara antes de la siguiente entrega o actualización.                         |
| 3           | Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta.                                                                                       |
| 4           | Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento.                                                                                     |

**TABLA RESUMEN:**

|  #  |                                                 Problema                                                 | Escala de severidad |         Heurística/Principio violado          |
| :-: | :------------------------------------------------------------------------------------------------------: | :-----------------: | :-------------------------------------------: |
|  1  |                         Incluye un botón “See More” pero no tiene funcionalidad                          |          3          |    Information Architecture: Is it usable     |
|  2  | No parece haber consistencia en la forma en que se presentan las opciones para actualizar la información |          2          |     Usability: Consistencia y estándares      |
|  3  |                            Información de pagos no está claramente presentada                            |          3          | Usability: Visibilidad del estado del sistema |
|  4  |                             No funciona cancelar el agregado de un vehículo.                             |          2          |   Usability: Libertad y control del usuario   |

**DESCRIPCIÓN DE PROBLEMAS:**

**PROBLEMA #1:**

**Severidad:** 3

**Heurística violada:** Information Architecture: Is it usable?

**Problema:**

La aplicación incluye un botón “See More” pero no tiene funcionalidad, lo que confunde a los usuarios y les impide acceder a contenido adicional esperado.

![H1](/assets/chapter06/h1.png)

**Recomendación:**

Eliminar el botón “See More” si no hay contenido adicional disponible, o implementar la funcionalidad esperada para que los usuarios puedan acceder a más información.

**PROBLEMA #2:**

**Severidad:** 2

**Heurística violada:** Usability - Consistencia y estándares

**Problema:**

La interfaz de Settings incluye campos para Nickname, Bio, Email y Avatar, pero no parece haber consistencia en la forma en que se presentan las opciones para actualizar la información. Por ejemplo, el botón ‘Choose’ para actualizar el avatar está separado del campo ‘Avatar’, lo que podría confundir a los usuarios.

![H2](/assets/chapter06/h2.png)

**Recomendación:**

Asegurar que todos los campos de entrada y botones relacionados estén agrupados de manera coherente y clara para mejorar la comprensión y la facilidad de uso.

**PROBLEMA #3:**

**Severidad:** 3

**Heurística violada:** Usability: Visibilidad del estado del sistema

**Problema:**

La información relacionada con Organization no está claramente presentada, lo que puede causar confusión a la hora de querer tener información y dificulta la asignación de envíos.

![H3](/assets/chapter06/h3.png)

**Recomendación:**

Mejorar la presentación y accesibilidad de la información relacionada con "Organization" puede mejorar significativamente la experiencia del usuario y facilitar la asignación de envíos en la aplicación.

**PROBLEMA #4:**

**Severidad:** 2

**Heurística violada:** Usability: Libertad y control del usuario

**Problema:**

Al momento de ingresar los datos del nuevo vehículo, no se puede cerrar hasta darle darle al botón “Close” y luego se tiene que eliminar en el botón “Delete Vehicle”, esto obliga a agregar nuevos carros no deseados, también incrementando así la cantidad de esfuerzo del usuario.

![H4](/assets/chapter06/h4.png)

**Recomendación:**

Hacer que el botón "Close" tenga la funcionalidad para cerrar la ventana emergente sin guardar los datos del vehículo ingresados.

---

## 6.4. Auditoría de Experiencias de Usuario

La auditoría de experiencias de usuario es un proceso clave para evaluar la efectividad, accesibilidad y satisfacción que ofrece una interfaz digital a sus usuarios. A través de un análisis detallado de cada punto de interacción, esta auditoría permite identificar fricciones, inconsistencias y oportunidades de mejora que impactan directamente en la usabilidad y la percepción del producto. Su objetivo es asegurar que la experiencia ofrecida sea intuitiva, eficiente y alineada con las necesidades y expectativas del público objetivo.

### 6.4.1. Auditoría realizada

Se realizó una auditoría de experiencias de usuario para identificar problemas de usabilidad y mejorar la interacción con la interfaz, enfocándose en la eficiencia y satisfacción del usuario.

#### 6.4.1.1. Información del grupo auditado

La auditoría contó con un panel de usuarios representativos del público objetivo de la plataforma, seleccionados cuidadosamente de acuerdo con criterios de perfil demográfico, nivel de experiencia digital y frecuencia de uso. Esta muestra equilibrada permitió capturar tanto las necesidades de usuarios primerizos como las de power users, garantizando insights completos sobre los distintos flujos y puntos de fricción de la interfaz.

**Entidad auditora:** LosTesters

**Equipo:** Especialistas multidisciplinarios en diseño de interfaces (UI), accesibilidad web y experiencia inclusiva, con amplia trayectoria en proyectos de evaluación de usabilidad.

**Inicio:** 13 de junio de 2025

**Cierre:** 21 de junio de 2025

**Objetivos principales:**

- Identificar barreras de usabilidad y accesibilidad en los flujos críticos.

- Evaluar el rendimiento técnico y la consistencia visual de la interfaz.

- Proponer acciones concretas para optimizar la experiencia multi‑dispositivo y bajo distintos niveles de carga.

**Metodología:**
La auditoría combinó técnicas cualitativas y cuantitativas, incluyendo pruebas de usabilidad moderadas y no moderadas, análisis de métricas de rendimiento y validación de pautas de accesibilidad WCAG 2.1.

**Herramientas y entornos empleados:**

- **Selenium WebDriver:** para automatizar y reproducir interacciones de usuario, detectar bloqueos de flujo y validar transiciones de pantalla.

- **Lighthouse (CLI):** para medir puntajes de rendimiento, accesibilidad, mejores prácticas y SEO en entornos de desarrollo y producción.

- **WebPageTest**: para analizar tiempos de carga y renderizado desde múltiples ubicaciones geográficas y dispositivos reales.

- **RedLine13:** para simular escenarios de alto tráfico y evaluar el comportamiento bajo estrés.

**Herramientas complementarias:**

- Mapas de calor y grabaciones de sesión para detectar patrones de scroll y clic.

- Test de contraste de color y validadores ARIA para asegurar cumplimiento de estándares inclusivos.

**Entregables esperados:**

- Informe de auditoría preliminar con hallazgos cuantitativos y cualitativos.

- Guía de recomendaciones agrupadas por prioridad (alto, medio, bajo).

- Checklist de accesibilidad y rendimiento con evidencias visuales (capturas y gráficas).

#### 6.4.1.2. Cronograma de auditoría realizada.

Cada fase de la auditoría fue diseñada para maximizar la trazabilidad de los hallazgos y garantizar una implementación eficiente de las mejoras. Comenzamos con la revisión y análisis de datos recopilados en las etapas previas (entrevistas, mapas de calor, métricas cuantitativas), continuamos con la elaboración de informes y validaciones internas, y cerramos con pruebas finales y ajustes de detalle basados en retroalimentación directa de usuarios reales.

| Fecha      | Fase                                                                                                                                                                | Objetivo principal                                                                                                           | Entregable                                  | Responsable        |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- | ------------------ |
| 13/06/2025 | Análisis de resultados y redacción del informe preliminar                                                                                                           | Sintetizar datos cualitativos y cuantitativos para identificar patrones de uso, fricciones y oportunidades de mejora         | Borrador de informe con hallazgos clave     | Fabrizio Sanchez   |
| 14/06/2025 | Revisión cruzada del informe y validación de hallazgos                                                                                                              | Asegurar la precisión de los datos y el consenso metodológico entre auditores                                                | Acta de validación con comentarios          | Juan Cueto         |
| 14/06/2025 | Presentación de resultados y recomendaciones al equipo cliente                                                                                                      | Comunicar de manera clara y visual las áreas de oportunidad y posibles soluciones                                            | Slide deck de presentación y plan de acción | Flavio Trigueros   |
| 15/06/2025 | Revisión del diseño visual con base en los hallazgos                                                                                                                | Ajustar componentes gráficos y flujos de interfaz que generan confusión o baja conversión                                    | Prototipo visual actualizado (Figma/Sketch) | Aldhair Valenzuela |
| 16/06/2025 | Implementación de ajustes de accesibilidad                                                                                                                          | Corregir deficiencias de contraste, navegación por teclado y etiquetas ARIA Registro de cambios y checklist de accesibilidad | Piero Tarazona                              |
| 17/06/2025 | Optimización del rendimiento basada en métricas de Lighthouse                                                                                                       | Reducir tiempos de carga y mejorar puntuaciones de Core Web Vitals                                                           | Informe de mejoras de rendimiento           | Juan Cueto         |
| 18/06/2025 | Ejecución de pruebas de regresión automatizadas con Selenium                                                                                                        | Verificar que las modificaciones no introduzcan nuevos errores ni rompan funcionalidades existentes                          | Logs y resultados de pruebas automatizadas  | Juan Cueto         |
| 19/06/2025 | Validación final con usuarios (pruebas de usabilidad remotas/presenciales)                                                                                          | Confirmar que los ajustes mejoran la experiencia real y recabar impresiones finales                                          | Video clips y reportes de feedback          | Fabrizio Sanchez   |
| 20/06/2025 | Recopilación y análisis de feedback posterior a ajustes                                                                                                             | Consolidar comentarios de usuarios y stakeholders para detectar posibles ajustes puntuales antes del cierre final            | Informe de feedback y plan de refinamiento  | Flavio Trigueros   |
| 21/06/2025 | Elaboración y entrega del informe final de auditoría de experiencia de usuario Integrar todos los hallazgos, evidencias y recomendaciones en un documento ejecutivo | Informe final completo (PDF + presentación)                                                                                  | Aldhair Valenzuela                          |

**Notas de proceso:**

- **Metodología:** Cada fase combinó técnicas cuantitativas (analítica web, Lighthouse, A/B testing) y cualitativas (entrevistas, test de usabilidad).

- **Comunicación:** Se convocaron reuniones diarias de sincronización (stand‑ups) para informar avances y mitigar bloqueos.

- **Herramientas:** Figma/Sketch para prototipos. Lighthouse CLI para auditorías de rendimiento. Selenium WebDriver para pruebas automatizadas. Google Analytics para métricas.

#### 6.4.1.3. Contenido de auditoría realizada.

La auditoría abarcó una revisión integral de la experiencia de usuario, evaluando aspectos como la usabilidad, el rendimiento, la accesibilidad y la eficiencia del sistema. Se analizaron distintos flujos de navegación, tiempos de carga, consistencia visual e interacción del usuario mediante herramientas automatizadas y criterios estandarizados, con el fin de identificar áreas de mejora y asegurar una experiencia óptima.

| #   | Problema detallado                                                                                                                                                                             | Severidad | Heurística / Principio violado                                   | Impacto en el usuario                                                                                                                                     | Recomendación                                                                                                                                               |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- | ---------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | El texto rojo oscuro sobre fondo negro en la pantalla principal genera un contraste insuficiente, dificultando la lectura para personas con baja visión o condiciones de luminosidad variable. | 3         | Accesibilidad; Estética y diseño minimalista                     | Fatiga visual, posibles errores de interpretación de contenido y abandono de la tarea.                                                                    | Ajustar colores para cumplir con ratio de contraste mínimo (4.5:1). Usar herramientas de test de contraste y aplicar tests de usuarios con visión reducida. |
| 2   | Elementos del encabezado (logo y botones) se muestran demasiado pequeños en pantallas de alta resolución, perdiendo visibilidad y jerarquía dentro de la interfaz.                             | 2         | Estética y diseño minimalista; Consistencia y estándares         | Dificultad para localizar acciones clave, sensación de desproporción y confusión sobre la identidad de la marca.                                          | Definir tamaños relativos (em/rem) escalables, establecer un tamaño mínimo de tap targets (44×44 px) y probar en distintos breakpoints.                     |
| 3   | Botones como “Sign In” y “Home” carecen de atributos aria-label, impidiendo su correcta interpretación por lectores de pantalla.                                                               | 4         | Accesibilidad; Ayuda y documentación                             | Usuarios con discapacidad visual no reciben contexto ni feedback al navegar, lo que bloquea el acceso a funciones esenciales.                             | Añadir aria-label descriptivos en todos los controles interactivos y verificar la navegabilidad con NVDA, VoiceOver o JAWS.                                 |
| 4   | Los módulos de “fermentación”, “clarificación”, etc., no presentan una jerarquía visual clara (títulos, subtítulos, agrupaciones), lo que dispersa la atención del usuario.                    | 2         | Consistencia y estándares                                        | Usuarios tardan más en ubicar información relevante y pueden omitir secciones importantes por falta de orden visual.                                      | Usar encabezados (h2, h3) de forma consistente, agrupar contenidos en contenedores con espaciado definido y aplicar diseño modular con tarjetas.            |
| 5   | Al presionar acciones como “Export” o “New” no aparece indicador de carga ni confirmación, provocando incertidumbre y posibles clics repetidos.                                                | 3         | Visibilidad del estado del sistema; Prevención de errores        | Frustración ante la falta de feedback, riesgo de acciones duplicadas y pérdida de datos en procesos largos.                                               | Implementar spinners o barras de progreso, deshabilitar botones durante la operación y mostrar notificaciones al completar la tarea.                        |
| 6   | Mensajes de validación de formulario se limitan a “Campo obligatorio” sin explicar formato, longitud o ejemplos, dejando al usuario sin guía clara.                                            | 2         | Prevención de errores; Ayuda y documentación                     | Mayor tasa de errores de ingreso, aumento del tiempo para completar formularios y posible abandono por frustración.                                       | Incluir mensajes contextuales (“Debe tener al menos 8 caracteres, incluir número y mayúscula”), ejemplos y posicionarlos junto al campo correspondiente.    |
| 7   | No existe un mecanismo intuitivo para editar o ver en detalle registros ya ingresados (editar en línea, modal, página dedicada), lo que reduce la flexibilidad de uso.                         | 2         | Flexibilidad y eficiencia de uso; Control y libertad del usuario | Usuarios tienen que recurrir a rutas improvisadas o abandonar el flujo principal para corregir datos, aumentando la carga cognitiva y el tiempo de tarea. | Incorporar acciones de “Editar” y “Ver detalles” directamente en tablas o listas, usar modales o inline editing para accesos rápidos.                       |
| 8   | El selector de idioma (EN/ES) no traduce todos los textos (mensajes de error, tooltips, labels), generando inconsistencias que confunden a usuarios no bilingües.                              | 3         | Consistencia y estándares; Flexibilidad y eficiencia de uso      | Interrupción del flujo al cambiar de idioma, desconfianza en la calidad de la traducción y posibles malentendidos en procesos críticos.                   | Auditar cadenas de texto, asegurar que todas las keys de i18n estén cubiertas y automatizar pruebas de regresión lingüística tras cada despliegue.          |
| 9   | La interfaz no permite agrandar el tamaño de fuente ni respeta configuraciones de zoom del navegador, limitando a usuarios con baja visión o preferencia de texto grande.                      | 4         | Accesibilidad                                                    | Usuarios con dificultades visuales no pueden adaptar la UI a sus necesidades, lo que imposibilita el acceso completo al contenido.                        | Utilizar unidades relativas (em/rem), evitar tamaños fijos en pixeles, y verificar el comportamiento con zoom al 150–200 % en distintas plataformas.        |
| 10  | Reglas de contraseña estrictas (mínimo de caracteres, combinación de tipos) se imponen sin orientación contextual ni ejemplos, provocando múltiples intentos fallidos.                         | 3         | Prevención de errores; Ayuda y documentación                     | Usuarios experimentan frustración y abandonan el registro al no entender requisitos, afectando la tasa de conversión de nuevos usuarios.                  | Mostrar barra de fortaleza en tiempo real, explicar requisitos antes o durante el ingreso, y ofrecer “mostrar contraseña” para validar lo escrito.          |

### 6.4.2. Auditoría recibida

La auditoría recibida permitió obtener una visión objetiva y detallada sobre el estado actual de la experiencia de usuario en el sistema evaluado. A través de los hallazgos presentados, se identificaron fortalezas, debilidades y recomendaciones clave que servirán como base para futuras mejoras en diseño, accesibilidad y rendimiento.

#### 6.4.2.1. Información del grupo auditor

El grupo auditor estuvo conformado por especialistas en experiencia de usuario, accesibilidad y rendimiento web. Contaban con conocimientos en herramientas como Selenium, Lighthouse y WebPageTest, lo que permitió realizar una evaluación técnica y centrada en el usuario, garantizando resultados precisos y relevantes para la mejora del sistema.

El grupo auditor estuvo conformado por un equipo multidisciplinario de alto nivel, integrado por especialistas en experiencia de usuario, accesibilidad digital y optimización de rendimiento web. Su sólido dominio de metodologías de evaluación centradas en el usuario y de herramientas de análisis automatizado garantizó una revisión exhaustiva tanto de la interfaz como de la arquitectura técnica del sistema.

**Entidad auditora:** EventWine

**Equipo:** Diseñadores de interfaces (UI) con experiencia en principios de diseño responsivo y mobile-first. Expertos en accesibilidad web certificados en estándares WCAG 2.1. Ingenieros de rendimiento con conocimientos avanzados en medición de Core Web Vitals y optimización de cargas.

**Inicio:** 13 de junio de 2025

**Cierre:** 21 de junio de 2025

**Objetivos de la auditoría:**

- **Usabilidad:** Detectar y priorizar cuellos de botella en los flujos críticos de usuario (registro, compra, navegación).

- **Accesibilidad:** Verificar el cumplimiento de pautas para garantizar acceso a personas con discapacidades visuales, auditivas y motoras.

- **Rendimiento:** Medir y mejorar tiempos de carga, interactividad y estabilidad visual bajo distintos escenarios de red y dispositivo.

**Metodología empleada:**

- Pruebas de usabilidad moderadas con usuarios finales, para obtener feedback cualitativo sobre la percepción y claridad de la interfaz.

- Análisis automatizado mediante scripts de Selenium WebDriver que reprodujeron secuencias de uso y detectaron errores de flujo.

- Medición de rendimiento con Lighthouse en entornos de desarrollo y producción, evaluando métricas de rendimiento, accesibilidad, buenas prácticas y SEO.

- Test de carga y estrés con RedLine13 para simular tráfico concurrente y determinar la capacidad real de la plataforma.

- Comparativa de ubicaciones usando WebPageTest, recorriendo rutas de carga desde distintas regiones geográficas y dispositivos reales para identificar variaciones de experiencia.

**Herramientas y su uso específico:**

- Selenium WebDriver: Automatización de interacciones complejas (formularios, menús dinámicos) y generación de logs de errores en consola.

- Lighthouse (CLI): Auditorías periódicas de Core Web Vitals (Largest Contentful Paint, First Input Delay, Cumulative Layout Shift) y reportes de accesibilidad.

- WebPageTest: Captura de waterfall charts y comparativa de tiempos de carga en móviles 3G, 4G y conexiones de escritorio.

- RedLine13: Escenarios de alto tráfico (100–1 000 usuarios simultáneos) para medir impacto de picos de uso y detectar cuellos de botella de backend.

**Herramientas complementarias:**

- Mapas de calor y grabaciones de sesiones para analizar comportamiento real de clic y scroll.

- Validadores ARIA y contrast checkers para asegurar cumplimiento de estándares inclusivos.

**Entregables esperados:**

- Informe preliminar con hallazgos categorizados por prioridad y evidencia visual.

- Guía de recomendaciones detallada: mejoras de código, ajustes de diseño y cambios en la infraestructura.

- Checklist de accesibilidad y rendimiento con checklist de verificación y resultados antes/después.

- Plan de seguimiento para verificar la implementación de las mejoras y volver a medir resultados tras cada iteración.

Con este enfoque integral, EventWine aseguró una evaluación precisa, alineada con las mejores prácticas de UX, accesibilidad y optimización web, proporcionando al equipo cliente una hoja de ruta clara para elevar la calidad y robustez del sistema.

#### 6.4.2.2. Cronograma de auditoría recibida

El cronograma de la auditoría recibida detalla las fechas y actividades realizadas por el equipo auditor durante cada fase del proceso. Desde la evaluación inicial hasta la entrega del informe final, cada etapa se llevó a cabo de manera estructurada para garantizar una revisión completa, precisa y alineada con los objetivos del análisis.

Cada una de estas actividades se diseñó para abordar aspectos clave de usabilidad, accesibilidad, consistencia visual e internacionalización. El equipo trabajó de forma coordinada para que los hallazgos fuesen validados, documentados y transformados en recomendaciones prácticas.

| Fecha      | Actividad detallada                                                                                                                          | Objetivo principal                                                                                                      | Entregable                                                                          | Responsable     |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | --------------- |
| 13/06/2025 | Ejecución de auditoría automática con Lighthouse y WebPageTest en entornos de desarrollo y producción                                        | Obtener métricas iniciales de rendimiento, accesibilidad, mejores prácticas y SEO                                       | Reporte de Lighthouse (scores y sugerencias) y gráficas de waterfall de WebPageTest | Deybbi Crisanto |
| 14/06/2025 | Simulación de navegación completa con NVDA (lector de pantalla)                                                                              | Verificar que todos los elementos interactivos y de contenido sean accesibles para usuarios con discapacidad visual     | Video demostrativo y lista de errores ARIA                                          | Moises Donayre  |
| 15/06/2025 | Análisis de la estructura de navegación y mapeo de flujos críticos (registro, compra, configuración)                                         | Detectar rutas confusas o redundantes que impacten la eficiencia de uso                                                 | Diagrama de flujo actualizado y puntos de fricción                                  | Gustavo Huanca  |
| 15/06/2025 | Revisión exhaustiva de formularios: validaciones, mensajes de ayuda y gestión de errores                                                     | Garantizar que los usuarios entiendan claramente los requisitos de cada campo y reciban feedback contextualizado        | Matriz de validaciones y ejemplos de mensajes de error                              | July Paico      |
| 16/06/2025 | Comprobación de ratios de contraste y jerarquía visual según WCAG 2.1                                                                        | Asegurar legibilidad óptima en cualquier condición de luz y dispositivo                                                 | Capturas con marcadores de contraste y recomendaciones de estilo                    | Jesús Paucar    |
| 16/06/2025 | Evaluación de consistencia en iconografía, etiquetado y tamaño de botones en desktop y móvil                                                 | Mantener una experiencia coherente y predecible en todas las vistas                                                     | Guía de patrones UI con ejemplos antes/después                                      | Moises Donayre  |
| 17/06/2025 | Pruebas de internacionalización (i18n): cobertura de textos, tooltips y validación de formatos EN/ES                                         | Verificar que la traducción y presentación de contenido sea completa y libre de errores para hablantes de ambos idiomas | Checklist de keys i18n cubiertas y capturas de errores                              | July Paico      |
| 17/06/2025 | Medición de rendimiento bajo carga con RedLine13 y repaso de WebPageTest para detectar degradaciones por concurrencia                        | Determinar la capacidad de la plataforma ante picos de tráfico y proponer ajustes de infraestructura o caching          | Gráficos de latencia vs. usuarios simultáneos                                       | Gustavo Huanca  |
| 18/06/2025 | Identificación de errores de diseño y usabilidad en pantallas de registro, login y módulos internos (layout roto, elementos solapados, etc.) | Corregir fallos visuales que obstaculicen la interacción y el flujo de tareas esenciales                                | Reporte de defectos UI con capturas anotadas                                        | Jesús Paucar    |
| 18/06/2025 | Clasificación y priorización de hallazgos críticos por nivel de severidad                                                                    | Establecer un plan de acción enfocado en resolver primero los incidentes de mayor impacto en la experiencia             | Tabla de severidad y plan de acciones inmediatas                                    | Deybbi Crisanto |
| 19/06/2025 | Diseño de propuestas de mejora visual, estructural y de contenido (wireframes y ejemplos de copy optimizado)                                 | Generar soluciones concretas alineadas con las mejores prácticas UX/UI                                                  | Wireframes actualizados y borradores de copy                                        | July Paico      |
| 19/06/2025 | Sesión de revisión interna para validar observaciones y ajustar recomendaciones antes de la entrega final                                    | Asegurar coherencia metodológica y aprovechamiento del feedback del equipo auditor                                      | Acta de reunión con ajustes finales                                                 | Moises Donayre  |
| 20/06/2025 | Redacción y consolidación del informe final de auditoría: integración de hallazgos, evidencias visuales y criterios heurísticos              | Producir un documento ejecutivo que sirva de hoja de ruta para el equipo de desarrollo                                  | Informe PDF completo con anexos y presentación senior                               | Gustavo Huanca  |
| 20/06/2025 | Presentación formal de resultados y entregables al equipo de desarrollo y stakeholders clave, seguida de un Q&A para aclarar dudas           | Alinear prioridades de implementación y resolver consultas técnicas o de negocio                                        | Slide deck entregable y registro de preguntas y respuestas                          | Deybbi Crisanto |

Notas de proceso:

Se mantuvieron reuniones diarias de sincronización para revisar avances y resolver bloqueos rápidamente.

Todos los entregables incluyeron evidencias visuales (capturas de pantalla, videos, gráficos) para facilitar la comprensión de los hallazgos.

La priorización de acciones se basó en la combinación de severidad del problema, frecuencia de ocurrencia y esfuerzo estimado de implementación.

#### 6.4.2.3. Contenido de auditoría recibida

El contenido de la auditoría recibida incluye un análisis detallado de la interfaz evaluada, considerando aspectos como accesibilidad, tiempos de carga, usabilidad y consistencia visual. Los resultados se sustentan en métricas objetivas y observaciones técnicas, acompañados de recomendaciones concretas para optimizar la experiencia del usuario y mejorar el rendimiento general del sistema.

El informe recibido documenta un análisis exhaustivo de la interfaz evaluada, con foco en criterios de accesibilidad, usabilidad, rendimiento visual y consistencia estructural. La auditoría se basó en estándares reconocidos como las Heurísticas de Nielsen y las pautas WCAG 2.1, e incluyó tanto pruebas manuales como automáticas. Los hallazgos están sustentados en métricas objetivas y evidencia técnica, lo que permite priorizar acciones correctivas y generar mejoras tangibles en la experiencia del usuario final.

A continuación, se detallan los principales problemas identificados, clasificados por severidad y principio heurístico afectado:

| #   | Problema detallado                                                                                                                                                                   | Severidad | Heurística / Principio violado                                    | Impacto en el usuario                                                                                                  | Recomendación concreta                                                                                                               |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------- | ----------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| 1   | Los botones “Ver Detalle” y “Registrar” presentan bajo contraste con el fondo, especialmente en estados hover y focus. Esto compromete la legibilidad para usuarios con baja visión. | 3         | Accesibilidad; Estética y diseño minimalista                      | Dificultad para ubicar acciones clave, especialmente en condiciones de luz adversas o en usuarios con visión reducida. | Ajustar el contraste siguiendo el ratio mínimo 4.5:1 (según WCAG 2.1). Aplicar pruebas con herramientas como Color Contrast Checker. |
| 2   | Se repite el mismo modelo y placa de vehículo (ejemplo ABC123) en distintas secciones, sin diferenciadores contextuales ni agrupamiento lógico.                                      | 3         | Consistencia y estándares                                         | Genera ambigüedad, riesgo de selección incorrecta y dificulta el control de flotas o registros múltiples.              | Implementar validaciones de unicidad, mostrar identificadores adicionales (color, fecha de registro) o etiquetas descriptivas.       |
| 3   | Algunas imágenes de perfil no se cargan correctamente y muestran íconos rotos. Esto ocurre principalmente en la sección de usuario o avatar del perfil.                              | 2         | Estética y diseño minimalista; Visibilidad del estado del sistema | Transmite sensación de error o descuido en el sistema, afectando la percepción de calidad.                             | Incluir fallback visual predeterminado (ej. avatar genérico) y verificar rutas de carga de imágenes mediante pruebas automatizadas.  |
| 4   | En el formulario de registro de vehículos, campos clave como “ID interno” o “número de serie” no tienen etiquetas claras ni validaciones contextuales.                               | 3         | Ayuda y documentación; Prevención de errores                      | Aumenta el riesgo de errores de ingreso, frustra al usuario y puede generar datos inválidos en el sistema.             | Añadir etiquetas explicativas, placeholders y mensajes de ayuda contextual sobre formato y uso esperado del campo.                   |
| 5   | En formularios como “Editar Perfil” y “Registrar Vehículo” no se indica visualmente qué campos son obligatorios, ni se muestran asteriscos o mensajes de ayuda.                      | 2         | Prevención de errores; Estética y diseño minimalista              | Genera confusión y múltiples intentos fallidos al completar formularios.                                               | Utilizar asteriscos o íconos para denotar campos obligatorios y mostrar leyenda aclaratoria.                                         |
| 6   | En la sección de reportes no se permite aplicar filtros ni realizar búsquedas, dificultando la navegación en conjuntos de datos extensos.                                            | 2         | Flexibilidad y eficiencia de uso                                  | Usuarios pierden tiempo explorando visualmente o no logran encontrar datos relevantes rápidamente.                     | Incorporar buscador y sistema de filtros dinámicos (por fecha, estado, tipo de evento, etc.).                                        |
| 7   | Al guardar cambios en el perfil no se muestra ninguna notificación o confirmación visual, lo que deja al usuario sin claridad sobre si la acción fue exitosa.                        | 2         | Visibilidad del estado del sistema                                | Falta de retroalimentación genera incertidumbre y puede derivar en duplicación de acciones o pérdida de información.   | Mostrar mensajes toast o banners de confirmación (éxito/error) tras cada acción de guardado.                                         |
| 8   | Algunos componentes visuales, como los títulos de las tarjetas de reporte o íconos de acción, están desalineados o flotan fuera de su contenedor.                                    | 1         | Estética y diseño minimalista                                     | Afecta la estética general del sistema y puede hacer que la interfaz luzca inconsistente o inacabada.                  | Aplicar reglas claras de alineación y espaciado, emplear sistemas de grilla y revisar el comportamiento en distintos breakpoints.    |

#### 6.4.2.4. Resumen de modificaciones para subsanar hallazgos.

A partir de los hallazgos identificados durante la auditoría, se implementaron una serie de modificaciones orientadas a mejorar la experiencia de usuario. Estas acciones incluyeron ajustes en el diseño visual, optimización del rendimiento, corrección de errores de accesibilidad y mejoras en la navegación. Cada cambio fue realizado con el objetivo de subsanar las observaciones detectadas y garantizar una interacción más fluida, intuitiva y eficiente para los usuarios finales.

| #   | Problema detecado                                                                                                                                     | Acción de subsanación                                                                                                                                                                     | Impacto esperado                                                                |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| 1   | El avatar cargado no se muestra en el formulario de edición de perfil hasta recargar la página, generando confusión sobre si se guardó correctamente. | Se ajustó la lógica de binding: al finalizar la subida, el componente de imagen vuelve a renderizar automáticamente su src con la URL actualizada.                                        | El usuario verá su avatar al instante sin necesidad de recarga manual.          |
| 2   | Falta de feedback visual tras guardar cambios en el perfil; el usuario no sabe si la operación fue exitosa o fallida.                                 | Se incorporó un componente de notificación (toast/snackbar) que muestra mensajes de estado (“Perfil actualizado con éxito” o “Error al guardar”) con estilos diferenciales de color.      | Claridad inmediata sobre el resultado de la acción; menor incertidumbre.        |
| 3   | El botón “Save Changes” permanece estático durante el procesamiento, lo que impulsa múltiples clics y posibles peticiones duplicadas.                 | Se añadió un spinner inline dentro del botón y se deshabilitó temporalmente hasta recibir la respuesta del servidor; se restablece su estado al terminar la petición.                     | Evita clics redundantes, mejora la percepción de velocidad de respuesta.        |
| 4   | Los campos requeridos vacíos no muestran ninguna señalización visual (ni borde ni mensaje), provocando errores silenciosos al intentar guardar.       | Se implementó validación en tiempo real: los inputs obligatorios se rodean de un borde rojo y despliegan un texto de ayuda en rojo (“Este campo es obligatorio”) al perder el foco vacío. | Reducción de errores de formulario, guía clara para completar todos los campos. |
| 5   | Discrepancia de estilos entre el menú lateral y el área de contenido principal, rompiendo la coherencia estética de la aplicación.                    | Se normalizó la hoja de estilos: variables CSS compartidas (--primary-color, --border-radius, --font-size) y mixins para componentes comunes, asegurando uniformidad en ambas áreas.      | Interfaz más armónica y profesional, refuerzo de la identidad visual.           |
| 6   | Contraste insuficiente en la barra lateral (texto y iconos oscuros sobre fondo oscuro), incumpliendo ratios WCAG y dificultando la lectura.           | Se recalibraron los colores usando tonos que alcanzan un ratio mínimo de 4.5:1 (texto #FFFFFF sobre #2A2A2A); se añadieron pruebas automáticas de contraste en el pipeline de CI.         | Mejora de legibilidad para usuarios con baja visión y cumplimiento WCAG.        |
| 7   | Tras guardar el perfil, el usuario permanece en la misma vista sin confirmación ni redirección, dejando la sensación de estar “estancado”.            | Se definió un flujo de post-guardado: al confirmarse el éxito, se despliega un modal breve con un botón “Regresar al dashboard” y enlace a “Editar detalles nuevamente”.                  | Flujo más intuitivo, permite continuar con la siguiente tarea sin ambigüedad.   |
| 8   | El campo “Bio” carece de placeholder y no orienta al usuario sobre el tipo de información que debería incluir (longitud, tono, ejemplos).             | Se añadió un placeholder descriptivo (“Escribe una breve biografía: experiencia, intereses, hobbies…”), con contador de caracteres y validación de longitud mínima/máxima en tiempo real. | Guía proactiva para creación de contenido, mejora la calidad de dato            |

### 6.4.3 Auditoría del equipo

| Miembro del equipo     | Validaciones / Avances realizados                                                                                                                                                                                     | Nota |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---- |
| **Juan Cueto**         | - Registro de vehículos con validación de campos vacíos<br>- Validación de formato de placa<br>- Prevención de duplicados<br>- Vista de listado funcional y ordenada<br>- Botón de eliminación con confirmación modal | 20   |
| **Fabrizio Sanchez**   | - Edición de perfil con campos persistentes<br>- Validación de imagen de avatar<br>- Validación de email en formato y unicidad<br>- Lógica de guardado con feedback<br>- Interfaz responsiva en todos los tamaños     | 20   |
| **Flavio Trigueros**   | - Sección de reportes lista y funcional<br>- Filtro de reportes por tipo<br>- Validación de fechas y transportista<br>- Vista sin errores en estado vacío<br>- Orden cronológico asegurado en la visualización        | 20   |
| **Aldhair Valenzuela** | - Ajustes de contraste y fondo entre secciones<br>- Sidebar funcional en diferentes resoluciones<br>- Test de accesibilidad en botones<br>- Revisión de colores y consistencia<br>- Pruebas de navegación fluida      | 20   |
| **Piero Tarazona**     | - Detalle del envío completo<br>- Carga de datos dinámica por ID<br>- Visualización de transportista, fecha y estado<br>- Renderizado condicional según estado<br>- Prueba de diseño responsive en vista detalle      | 20   |

- **Juan Cueto**: Demostró un trabajo sólido al implementar correctamente el módulo de registro de vehículos. Cumplió con las validaciones esperadas (formato de placa, campos obligatorios, control de duplicados) y desarrolló una interfaz funcional para el listado. Sin embargo, presentó retrasos en los primeros días del sprint y algunas validaciones menores fueron completadas tras retroalimentación.

- **Fabrizio Sanchez**: Sobresalió en la implementación del módulo de perfil, asegurando persistencia de datos, validaciones tanto de formato como de contenido, y un diseño responsivo. Se anticipó a posibles errores del usuario y propuso mejoras de experiencia.

- **Flavio Trigueros**: Logró finalizar correctamente la sección de reportes, incluyendo filtros y validaciones esenciales. Aunque cumplió con las tareas asignadas, hubo pequeños detalles de presentación y organización que requirieron ajustes en fases posteriores.

- **Aldhair Valenzuela**: Trabajó en aspectos visuales y de accesibilidad, como la paleta de colores, contrastes y comportamiento del sidebar. Su participación fue clave para la coherencia visual del sistema, pero algunos ajustes tuvieron que ser afinados por otros miembros en etapas finales.

- **Piero Tarazona**: Implementó de forma eficaz la vista de detalle de envío, garantizando que todos los campos clave fueran visibles y adaptables a diferentes pantallas. Además, realizó pruebas funcionales para asegurar una experiencia sin errores en la navegación del detalle.
