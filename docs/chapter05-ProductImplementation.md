# Capítulo V: Product Implementation 

## 5.1. Software Configuration Management. 

Para administrar la configuración de software de nuestra app, nos centraremos en tres aspectos principales: el control del código fuente, que implica gestionar las versiones y establecer una estructura organizada para el código; la configuración del entorno de desarrollo, donde nos aseguramos de que todos los miembros del equipo cuenten con herramientas consistentes; y la configuración de implementación, que se ocupa del despliegue en entornos de producción. Estas decisiones garantizan la coherencia y eficacia a lo largo de todo el ciclo de vida de la aplicación.

## 5.1.1. Software Development Environment Configuration. 

En esta sección, detallaremos y explicaremos los productos utilizados en el proyecto digital, así como su propósito y cómo se accede a cada uno de ellos y siguiendo las restricciones establecidas.

**Project Management**

Para gestionar el proyecto, se utilizaron herramientas de comunicación y control de versiones. Se estableció una organización en GitHub para gestionar el código y las versiones del proyecto. Además, para las reuniones de equipo y la comunicación interna, se utilizaron plataformas como Google Meet y Discord.

* Github: https://github.com/ 
* Google Meet: https://meet.google.com/ 
* Discord: https://discord.com/download 

**Requirements Management**

Para la gestión de requisitos se llevó a cabo mediante el uso de herramientas personalizadas que permitieron recopilar, organizar y priorizar los requisitos del proyecto de manera eficiente. Se utilizó Trello, una herramienta visual para la gestión de requisitos, permitiendo la creación tableros personalizados para organizar y priorizar las tareas del proyecto que permitió realizar los Task board y Pivotal Tracker, utilizado para gestionar y realizar un seguimiento del Product Backlog del proyecto.

* Trello: https://trello.com/es
* Pivotal Tracker: https://www.pivotaltracker.com/

**Product UX/UI Design**

Para el diseño de la experiencia de usuario (UX) y diseño de interfaz de usuario (UI) del producto se utilizo la herramienta Figma, esta herrmienta permitio al equipo crear wireframes, mockups y prototipos interactivos para visualizar y validad el diseño del producto antes de la implementación. Por otro lado, para la creación de User Personas, Empathy Maps, Journey Maps e Impact Maps se utilizó UXPressia y para la creación de As-Is y To-Be Scenario Maps se utilizó Miro.

* Figma: https://www.figma.com/downloads/
* UXPressia: https://uxpressia.com/
* Miro: https://miro.com/es/

**Software Development**

Para el desarrollo de software se utilizó HTML5, CSS3 y JavaScript para el desarrollo de la Landing Page de la startup, por otro lado, para la creación del Web Application de la startup se utilizarán el framework de Vue por el lado del Frontend y en el Backend se utilizará ASP.NET Core Framework y C#. Para trabajar con estas tecnologías, se emplearon los siguientes IDEs:

Visual Studio Code: Herramienta principal para el desarrollo Frontend y Backend, que ofrece una amplia gama de extensiones para mejorar la productividad del equipo. (En nuestro caso solo fue utilizado para la Landing Page). JetBrains Toolbox: Proporciona un entorno integrado para el desarrollo web, con características avanzadas de edición y depuración que faciitan la creación de aplicaciones web robustas.

* Visual Studio Code: https://code.visualstudio.com/
* JetBrains Toolbox: https://www.jetbrains.com/toolbox-app/

Software Documentation: La documentación del software se realizó utilizando GitHub, además de ser utilizado como plataforma de control de versiones, GitHub también se empleó para alojar la documentación técnica del proyecto. Se crearon repositorios específicos para almacenar toda la información. La documentación se gestionó mediante archivos Markdown para facilitar la creación y edición colaborativa.
GitHub: https://github.com/

5.1.2. Source Code Management. 
En este proyecto, utilizaremos GitHub como plataforma y sistema de control de versiones para gestionar el código fuente de nuestras diferentes partes del proyecto dentro de una organización.

**Repositorios en GitHub:**

* Organización: https://github.com/upc-AppWeb-BicasTeam
* Landing Page: https://github.com/upc-AppWeb-BicasTeam/upc-AppWeb-BicasTeam-LandingPage
* Report : https://github.com/upc-AppWeb-BicasTeam/upc-AppWeb-BicasTeam-Report

**GitFlow Workflow**

Implementaremos el modelo GitFlow como Workflow de control de versiones, siguiendo las convenciones y prácticas establecidas para una gestión eficiente del desarrollo de software.

**Branches Principales:**

main: Rama principal del repositorio, contiene el código estable y liberado.
develop: Rama de desarrollo donde se integran las nuevas características y mejoras.

**Branches de Funcionalidades (Feature Branches):**

Para cada nueva funcionalidad, se creará una rama de funcionalidad con el prefijo feature/, seguido del nombre descriptivo de la función o característica. En nuestro caso, creamos 8 branches de características correspondientes a los 8 capítulos de nuestro informe, donde se realizan los commits respectivos antes de fusionarlos con la rama develop cuando estén listos.

**Branches de Lanzamiento (Release Branches) y Branches de Corrección (Hotfix Branches):** En nuestro caso, no hicimos uso de estas branches ya que no lo vimos necesario al ser solo documentación del reporte.

Versionado Semántico Seguimos la especificación Semantic Versioning 2.0.0 para nombrar nuestras versiones, siguiendo el formato: 

    MAJOR.MINOR.PATCH.

**Conventional Commits:**

Aplicamos el estándar de Conventional Commits para los mensajes de commit, siguiendo un formato estructurado que describe claramente los cambios realizados. Esto nos ayudó a automatizar la generación de notas de versión y facilitar la comprensión del historial de cambios del proyecto.

Con estas prácticas y convenciones adaptadas a una organización en GitHub, buscamos mantener un flujo de desarrollo ordenado, colaborativo y bien documentado.

### 5.1.3. Source Code Style Guide & Conventions

En esta sección, se establece las convenciones y prácticas que seguiremos para nombrar elementos y programar en los lenguajes utilizados en la solución, que incluyen HTML, CSS, JavaScript, Vue.js, C#, y Gherkin para los archivos .feature. Todas las convenciones seguirán la nomenclatura en inglés y adoptarán convenciones estándares de codificación.

**HTML y CSS:**

1. Basado en las recomendaciones de W3C y otras fuentes de la comunidad, se establecerán convenciones para el nombramiento de elementos hTML y estilo de la codificación CSS.

2. Se seguirán las convenciones recomendadas por Google para HTML y CSS, que incluyen el uso de indentaciones de 2 espacios, el uso de comillas dobles para atributos y el uso de comentarios descriptivos.

3. Se utilizará la metodología BEM para organizar las clases CSS en bloques, elementos y modificadores, lo que facilitará la modularidad y la reutilización del código.

4. Se debe utilizar los elementos HTML de manera semántica para una correcta descripción del contenido del sitio web, incluyendo el uso adecuado de etiquetas.

5. Para el desarrollo con Vue.js, se adoptarán las convenciones recomendadas por la comunidad de Vue, que incluyen el uso de PascalCase para los nombres y componentes y el uso de camelCase para las propiedades y métodos de los componentes.

**JavaScript:**

1. Se tomarán en cuenta las directrices proporcionadas por MDN para la escritura de JavaScript, que incluyen el uso de nombres descriptivos para variables y funciones en camelCase, el uso de declaración de variables con let o const en lugar de var, y el uso de punto y coma al final de cada declaración.
   
2. Se seguirán las convenciones de codificación recomendadas por Google para JavaScript, que incluyen el uso de comillas simples para literales de cadena, el uso de comentarios descriptivos y el uso de funciones de flecha para expresiones de función.

**Vue.js:**

1. Se adoptarán las convenciones de codificación recomendadas por la comunidad de aplicaciones Vue.js, que incluyen el uso de directivas v-bind y v-on abreviadas, el uso de ciclo de vida y la organización de componentes en carpetas y subcarpetas según su función.

**C# (ASP.NET Core):**

1. Se seguirán las convenciones de codificación establecidas por Microsoft para el lenguaje C#, que incluyen el uso de PascalCase para nombres de clases y métodos, el uso de camelCase para nombres de variables locales y parámetros, y el uso de comentarios XML para documentar el código.
   
2. Para el desarrollo en ASP.NET Core, se adoptarán las directrices proporcionadas por Microsoft en sus guías de codificación, que incluyen el uso de inyección de dependencias, la separación clara entre capas de la aplicación y el uso de modelos de vista para la comunicación entre el controlador y la vista.
   
**Gherkin:**

1. Se aplicarán las convenciones recomendadas para escribir especificaciones legibles en Gherkin, que incluyen el uso de palabras clave como Given, When y Then para describir el comportamiento del sistema, el uso de un lenguaje sencillo y claro, y la organización de los escenarios en contextos, acciones y resultados.

2. Se seguirán las mejores prácticas recomendadas por Cucumber para escribir escenarios de prueba en Gherkin, que incluyen la reutilización de pasos de prueba, la modularización de escenarios y la escritura de pruebas autoexplicativas.
   
3. Además de estas referencias, se promoverá el uso de buenas prácticas y metodologías estándar en el desarrollo de software, como la modularidad, la reutilización de código, la legibilidad del código, la optimización del rendimiento y la seguridad. Con estas guías de estilo y convenciones de codificación, buscamos asegurar la coherencia, la calidad y la mantenibilidad del código a lo largo de todo el proyecto.

### 5.1.4. Software Deployment Configuration

En esta sección, describiremos la configuración necesaria para desplegar satisfactoriamente cada uno de los productos digitales de nuestra solución, incluyendo Landing Page, los Web Services y las Frontend Web Applications. Pasos para el despliegue:

**Landing Page:**

1. Clonar o descargar el repositorio desde GitHub.
2. Configurar el servidor web para alojar la Landing Page.
3. Copiar los archivos HTML5, CSS y JavaScript en el directorio correspondiente del servidor.
4. Configurar cualquier dependencia adicional, como bibliotecas de JavaScript o imágenes.
5. Verificar que la Landing Page se cargue correctamente en el navegador.

**Web Services (API):**

1. Preparar el código fuente del servicio web, asegurando que esté correctamente estructurado y documentado.
2. Configurar un entorno de desarrollo o pruebas para realizar pruebas exhaustivas del servicio antes del despliegue.
3. Desplegar el código en un servidor adecuado para el entorno de producción.
4. Configurar la seguridad y la autenticación según los requisitos del sistema.
5. Documentar la API utilizando OpenAPI Specification para facilitar su integración y uso por parte de otros sistemas.

**Frontend Web Applications:**

1. Clonar repositorio desde GitHub.
2.Compilar y empaquetar las aplicaciones frontend. En nuestro caso, utilizamos el framework Vue.js, por lo que se debe ejecutar los comandos de construcción (npm run build) para generar los archivos estáticos.
3. Una vez empaquetadas, las Frontend Web Applications se pueden servir utilizando un servidor de aplicaciones compatible con archivos estáticos, como Nginx o incluso GitHub Pages para proyectos estáticos más simples.
4. Si es necesario, se deben configurar las rutas en el servidor de aplicaciones para que coincidan con las rutas esperadas por las aplicaciones frontend.

### 5.1.5. Acuerdo de Servicio SaaS

**Introducción**

Bienvenido a MoviGestión, la plataforma móvil diseñada por LosTesters, un equipo de innovación tecnológica enfocado en soluciones para la gestión inteligente de flotas terrestres de transporte de bienes. Nuestra misión es brindar a empresas y operadores de transporte herramientas fiables, seguras y fáciles de usar que optimicen la asignación de vehículos, el seguimiento de envíos y el análisis de rendimiento, impulsando la eficiencia operativa y el crecimiento organizacional.

Estos Términos y Condiciones (en adelante, los “Términos”) constituyen un acuerdo legal, vinculante y de cumplimiento obligatorio entre LosTesters (en adelante, “nosotros” o “el Proveedor”) y usted (en adelante, el “Usuario”), en su calidad de persona natural o representante autorizado de una empresa, que accede, descarga, instala o utiliza de cualquier forma la aplicación móvil MoviGestión (en adelante, la “Aplicación”).

Al acceder, descargar, instalar o utilizar la Aplicación, el Usuario:

1. Declara bajo sanción de ley haber leído, comprendido y aceptado en su integridad los presentes Términos, así como las disposiciones de la Ley de Protección de Datos Personales (Ley N.° 29733) y su Reglamento (Decreto Supremo N.° 003-2013-JUS), la Ley de Firma Digital (Ley N.° 27269) y demás normativa aplicable al software y servicios digitales en el Perú.

2. Reconoce que dichos Términos constituyen un contrato de adhesión celebrado a través de un medio electrónico, conforme a lo previsto en el artículo 1353 del Código Civil peruano y la Ley de Comercio Electrónico (Ley N.° 27291).

3. Se obliga a cumplir todas las cláusulas aquí contenidas, así como las políticas internas de seguridad, privacidad y uso aceptable que LosTesters comunique periódicamente.

4. Acepta que el incumplimiento de cualquiera de estas obligaciones podrá ser sancionado con la suspensión o terminación de su acceso, sin perjuicio de las acciones civiles o penales que correspondan.

**Consentimiento Tácito y Modificaciones**

1. El uso continuado de MoviGestión tras la entrada en vigor de cualquier modificación a estos Términos implicará la aceptación tácita de las nuevas condiciones, de conformidad con el artículo 3 de la Ley de Protección de Consumidores y Usuarios (Ley N.° 29571).

2. LosTesters notificará con al menos treinta (30) días de anticipación las modificaciones sustanciales a los Términos mediante correo electrónico al Usuario registrado y/o publicación destacada en el sitio web oficial. La no oposición expresa dentro del plazo señalado se considerará aceptación plena de los cambios.

Si el Usuario no estuviera de acuerdo con alguna cláusula de estos Términos, deberá abstenerse de descargar, instalar o utilizar la Aplicación. En tal supuesto, LosTesters no asumirá responsabilidad alguna por la falta de uso o acceso a la Aplicación.

**LICENCIA DE USO**

LosTesters es titular exclusivo de todos los derechos de propiedad intelectual sobre la Aplicación MoviGestión, incluyendo, sin limitación, derechos de autor conforme a lo dispuesto en la Ley N.º 822, Ley sobre el Derecho de Autor y su Reglamento (Decreto Supremo N.º 005‑99‑MC). En calidad de tal, LosTesters concede al Usuario una licencia limitada, no exclusiva, intransferible, no sublicenciable y revocable, para:

* Acceder, descargar e instalar la Aplicación en dispositivos de su propiedad o bajo su control,

* Ejecutar y usar la Aplicación únicamente para la gestión de flotas de transporte terrestre de bienes, en el territorio de la República del Perú.

La licencia otorgada se limita a los derechos expresamente concedidos en este apartado y no confiere al Usuario ningún derecho de reproducción, modificación, ingeniería inversa, distribución, publicación o explotación comercial de la Aplicación o de sus componentes, más allá de lo estrictamente necesario para su uso según estos Términos (art. 2 de la Ley de Comercio Electrónico N.º 27291 y art. 69 de la Ley N.º 822).

**Duración y Revocación**

La presente licencia tendrá vigencia mientras el Usuario cumpla con estos Términos y no exista resolución anticipada. LosTesters podrá revocar la licencia de forma inmediata y sin previo aviso en caso de incumplimiento de cualquiera de las obligaciones aquí establecidas, así como en supuestos de uso fraudulento o ilícito, sin perjuicio de ejercer las acciones civiles o penales correspondientes (Código Civil, art. 1351).

**Derechos Patrimoniales**

La licencia no constituye transferencia de titularidad ni concesión de derechos patrimoniales sobre la Aplicación o sus elementos, tales como código fuente, diseño gráfico, bases de datos, interfaces o documentación, los cuales permanecerán en todo momento bajo la exclusividad de LosTesters. Cualquier otro uso no expresamente permitido en estos Términos requerirá la previa autorización escrita de LosTesters, bajo pena de responsabilidad por infracción a derechos de autor.

**Restricciones de Uso**

El Usuario se obliga a no emplear la Aplicación de forma que contravenga derechos de propiedad intelectual de LosTesters ni la normativa peruana o internacional aplicable al software. En particular, queda terminantemente prohibido, ya sea de manera directa o indirecta, realizar las siguientes acciones:

* Ingeniería inversa y análisis de código

    Descompilar, desensamblar, aplicar ingeniería inversa, traducir, adaptar, modificar o crear obras derivadas del código fuente o de cualquier componente de la Aplicación, sin la autorización previa, expresa y por escrito de LosTesters.

* Reproducción y distribución no autorizada

    Reproducir, sublicenciar, arrendar, alquilar, transferir, vender, ceder o poner a disposición de terceros la Aplicación o su contenido, total o parcialmente, con o sin ánimo de lucro, sin el consentimiento escrito de LosTesters.

* Uso ilícito o fraudulento

    Utilizar la Aplicación para fines ilegales, fraudulentos o no autorizados, incluidos actos de difamación, violación de privacidad, lavado de activos, envío de spam o cualquier actividad que infrinja derechos de terceros o la ley penal peruana.

* Amenazas a la seguridad e integridad

    Introducir virus, malware, troyanos, scripts maliciosos o realizar ataques de denegación de servicio (DoS/DDoS) u otras acciones que comprometan la seguridad, estabilidad o disponibilidad de la Aplicación o de los sistemas de LosTesters.

* Alteración de la funcionalidad

    Manipular, desactivar o eludir mecanismos de seguridad, control de acceso, cifrado o cualquier funcionalidad incorporada en la Aplicación para su protección, sin autorización escrita de LosTesters.

* Interferencia con otros usuarios

    Obstaculizar, interferir o impedir el uso legítimo de la Aplicación por parte de otros Usuarios, mediante acoso, acceso no autorizado a sus sesiones o realización de ataques técnicos.

* Suplantación de identidad y credenciales

    Usar credenciales que no le correspondan, suplantar la identidad de otro Usuario o intentar eludir los mecanismos de autenticación implementados.

* Actividades comerciales no autorizadas

    Emplear la Aplicación para promover productos o servicios, recopilar datos con fines comerciales, publicidad o envío de comunicaciones masivas no solicitadas, sin la autorización de LosTesters y sin cumplir la Ley de Protección de Datos Personales (Ley N.º 29733).

* Acceso a áreas restringidas

    Acceder, explorar o usar funcionalidades, datos o secciones de la Aplicación para los cuales no cuente con permiso expreso, o eludir las restricciones de acceso implementadas por LosTesters.

El incumplimiento de cualquiera de estas restricciones constituirá una violación grave de los presentes Términos, facultando a LosTesters a suspender, restringir o terminar el acceso del Usuario, sin perjuicio de las acciones civiles o penales que correspondan para la protección de sus derechos.

**Creación de Cuenta**

* Requisitos de Registro

    Para habilitar el acceso a funcionalidades restringidas de la Aplicación, el Usuario deberá completar el formulario de registro con datos veraces, completos, precisos y actualizados, en cumplimiento de la Ley N.º 29733 de Protección de Datos Personales y su Reglamento (DS N.º 003‑2013‑JUS). El Usuario garantiza que la información proporcionada es de su titularidad y se responsabiliza de su exactitud. Cualquier cambio deberá ser notificado de inmediato y registrado en la Aplicación.

* Confidencialidad y Seguridad de Credenciales

    El Usuario es el único responsable de la custodia y uso de sus credenciales de acceso (usuario y contraseña), comprometiéndose a:

    - Adoptar medidas de seguridad adecuadas para prevenir accesos no autorizados o robos de información de autenticación.

    - No compartir, ceder ni divulgar sus credenciales a terceros.
  
    En caso de sospecha de compromiso de la cuenta, el Usuario deberá cambiar su contraseña de inmediato y notificar a LosTesters mediante los canales de soporte establecidos.

* Responsabilidad por Actividades en la Cuenta

    Todas las acciones realizadas bajo la cuenta del Usuario se presumen autorizadas por éste, salvo que demuestre lo contrario. El Usuario responderá por cualquier daño, perjuicio o reclamación derivada del uso indebido de su cuenta, incluso si la actividad fue ejecutada por un tercero.

* Actualización de Datos

    El Usuario se obliga a mantener sus datos personales y empresariales actualizados. La omisión o inexactitud en la información podrá motivar la suspensión temporal o la cancelación definitiva de la cuenta, de conformidad con el Código Civil, artículo 1353, y la Ley de Comercio Electrónico N.º 27291.

* Suspensión y Terminación

    LosTesters podrá, a su entera discreción y sin previo aviso, suspender o cancelar la cuenta del Usuario por violaciones a estos Términos, uso fraudulento o riesgo para la seguridad de la Aplicación.La suspensión podrá ser preventiva o definitiva según la gravedad de la infracción. Durante la suspensión, el Usuario no podrá acceder a ninguna funcionalidad de la Aplicación.

    En caso de terminación, LosTesters podrá eliminar o inhabilitar los datos asociados a la cuenta, conforme a su Política de Privacidad y a la Ley N.º 29733. El Usuario acepta que la eliminación de datos podrá ser irreversible y que LosTesters no asumirá responsabilidad por la pérdida de información.

* Solicitud de Baja

    El Usuario podrá solicitar la terminación voluntaria de su cuenta en cualquier momento mediante los procedimientos establecidos por LosTesters (Formulario in‑app o comunicación por correo electrónico). Tras la baja, LosTesters retendrá únicamente los datos necesarios para cumplir obligaciones legales, fiscales o para la resolución de controversias, según lo previsto en su Política de Privacidad.

**Propiedad Intelectual**

Todos los derechos de autor, marcas, diseños, patentes, bases de datos, interfaces, código fuente, elementos gráficos, logotipos, nombres comerciales, sonidos y demás componentes de la Aplicación MoviGestión son propiedad exclusiva de LosTesters o de sus licenciantes. Dichos derechos están protegidos por la Ley N.º 822 – Derecho de Autor, la Ley N.º 27309 – Derecho de Diseños Industriales y Modelos de Utilidad, la Ley N.º 27291 – Comercio Electrónico, la Ley N.º 26887 – de Protección de la Propiedad Intelectual, y demás normativa peruana e internacional aplicable.

**Restricciones de Propiedad Intelectual:**

El Usuario reconoce que la utilización de MoviGestión le confiere únicamente un derecho de licencia limitado, no exclusivo, intransferible, no sublicenciable y revocable, de conformidad con lo dispuesto en estos Términos y en la legislación peruana (Ley N.º 822 Ley sobre el Derecho de Autor, Ley N.º 27291 de Comercio Electrónico). En ningún caso el Usuario adquiere derechos de propiedad, patrimoniales ni morales sobre la Aplicación, sus componentes, contenidos o documentación asociada.

Sin el consentimiento previo, expreso y por escrito de LosTesters, el Usuario no deberá, ni permitir a terceros:

1. Reproducir, copiar, publicar, comunicar públicamente, distribuir, sublicenciar, arrendar, alquilar, vender o ceder de cualquier forma la Aplicación, total o parcialmente, ya sea con o sin ánimo de lucro.

2. Descompilar, desensamblar, aplicar ingeniería inversa, traducir, adaptar, modificar, parchear o generar obras derivadas basadas en el código, la estructura, el diseño o la funcionalidad de la Aplicación.

3. Utilizar la Aplicación o su contenido para actividades comerciales distintas de las autorizadas en estos Términos, incluidas la venta de acceso, la prestación de servicios adicionales o la reventa de datos generados por la Plataforma.

**Marcas y Signos Distintivos**

Todos los nombres, logotipos, marcas comerciales y signos distintivos vinculados a MoviGestión y LosTesters son titularidad de LosTesters o de sus respectivos licenciantes. Queda prohibido su uso sin autorización escrita, pudiendo dar lugar a acciones por infracción de marca (Ley N.º 28236 de Protección de la Propiedad Intelectual).

**Protección de Datos y Privacidad**

El Usuario consiente el tratamiento de sus datos personales conforme a la Política de Privacidad de LosTesters, la Ley N.º 29733 de Protección de Datos Personales y su Reglamento. Se garantizan los derechos ARCO (Acceso, Rectificación, Cancelación y Oposición).

4. Modelo de Tarifas y Planes

Freemium: Funcionalidades básicas gratuitas y suscripciones premium pagadas.

Políticas de Reembolso: Definidas en el contrato de suscripción. Cancelación disponible en cualquier momento, pero no necesariamente reembolsable.

5. Limitaciones de Responsabilidad
No responsables por daños directos, indirectos, pérdida de datos, fallos externos, vulnerabilidades de seguridad, entre otros.

En ningún caso la responsabilidad superará lo pagado en los últimos 12 meses.

6. Garantías y Descargos
Aplicación ofrecida “tal cual” sin garantías de comerciabilidad, idoneidad, disponibilidad, exactitud de contenidos, seguridad, rendimiento ni compatibilidad total.

7. Modificaciones a los Términos
WeHaveAnIdea puede modificar los Términos en cualquier momento.

El uso continuo después de modificaciones implica aceptación automática.

Si las modificaciones son sustanciales, se notificará previamente.

## 5.2. Product Implementation & Deployment 

## 5.2.1. Sprints Backlogs

| **Sprint #**                    | Sprint 1                                                                 |
|---------------------------------|-------------------------------------------------------------------------|
| **Sprint Planning Background**  |                                                                         |
| **Date**                        | 2025-04-07                                                              |
| **Time**                        | 01:30 PM                                                                |
| **Location**                    | Virtual (Discord)                                                       |
| **Prepared By**                 | Fabrizio Sanchez                                                        |
| **Attendees (to planning meeting)** | Fabrizio Sanchez, Piero Tarazona, Flavio Trigueros, Aldhair Valenzuela, Juan Diego Cueto |
| **Sprint 1 - 1 Review Summary**     | Durante el primer sprint, avanzamos significativamente en el desarrollo del producto y logramos una colaboración eficiente dentro del equipo. Alcanzamos hitos importantes y recopilamos retroalimentación valiosa que nos servirá como base para el próximo sprint.    |
| **Sprint 1 - 1 Retrospective Summary**                    | En la retrospectiva del primer sprint identificamos áreas para mejorar, como la comunicación y la estimación de tareas. Estamos comprometidos a implementar acciones correctivas y mejorar continuamente nuestro proceso de trabajo.          |
| **Sprint Goal & User Stories**            |                                                         |
| **Sprint 1 Goal**                 | Alcanzar una métrica de cumplimiento del 100%, lo que indicará que se ha logrado los objetivos del sprint 1     |
| **Sprint 1 Velocity**                 | Acordamos aceptar 4 Story Points como nuestra capacidad de entrega para este sprint.          |
| **Sum of Story Points**                 | La suma de los Story Points para los User Stories que se están incluyendo en este Sprint 1 es 6     |

ssssssssssssssssssssprint 2
sssssssssssssssssssssprint 3
ssssssssssssssssssssprint 4

## 5.2.2. Implemented Landing Page Evidence

Para este punto llevamos a cabo el despliegue de nuestra landing page en GitHub Pages. A continuación, detallamos los pasos realizados:
1. Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de landing page.
2. Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamará main, ya que GitHub Pages toma esta rama como base para el despliegue automático.
3. Preparación del Contenido: Desarrollamos y diseñamos nuestra landing page, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
4. Generación del enlace de GitHub Pages: Navegamos a la sección "Pages" en la configuración del repositorio en GitHub. Configuramos la fuente del GitHub Pages para que tomara el contenido de la rama main.
5. Despliegue Automático: GitHub Pages automáticamente detectó los cambios en la rama main y desplegó la landing page en la URL proporcionada por GitHub Pages.

## 5.2.3. Implemented Frontend-Web Application Evidence

Para este punto, llevamos a cabo el despliegue de nuestro Frontend-Web Application en FireBase. A continuación, detallamos los pasos realizados:
- Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de web service.
- Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamará main, ya que esta rama sirve como base para el despliegue automático.
- Preparación del Contenido: Desarrollamos y diseñamos nuestra web service, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
- Generación del enlace del hosting: Creamos nuestra cuenta en el hosting, le asignamos un nombre y desplegamos el web service en la URL proporcionada por el hosting.

## 5.2.4. Implemented Native-Mobile Application Evidence

Para este punto, llevamos a cabo el despliegue de nuestra Native-Mobile Application en FireBase. A continuación, detallamos los pasos realizados:
- Creación del Repositorio en GitHub: Iniciamos creando un repositorio dedicado en GitHub para nuestro proyecto de web service.
- Configuración de la Rama main: Aseguramos que la rama principal del repositorio se llamará main, ya que esta rama sirve como base para el despliegue automático.
- Preparación del Contenido: Desarrollamos y diseñamos nuestra web service, asegurándonos de que todos los archivos y recursos necesarios estuvieran presentes en el repositorio.
- Generación del enlace del hosting: Creamos nuestra cuenta en el hosting, le asignamos un nombre y desplegamos el web service en la URL proporcionada por el hosting.

## 5.2.5. Implemented RESTful API and/or Serverless Backend Evidence

Para este punto llevamos a cabo el despliegue de nuestro Backend. A continuación, detallamos los pasos realizados:

* Ingresar a Visual Studio
* Descargar el Plugin Azure DevOps en nuestro proyecto
* Ingresamos nuestra cuenta de azure
* Configurar el despliegue de nuestro proyecto
* API desplegado

## 5.2.6. RESTful API documentation

El equipo ha logrado despegar el web service de MoviGestion. Todas las historias de usuario asignadas para este sprint fueron completadas exitosamente. En primer lugar, nos enfocamos en el desarrollo y la implementación del web service que es fundamental para la aplicación MoviGestion. Este esfuerzo incluyó la creación de APIs RESTful, la integración segura y eficiente con la base de datos, y la implementación de pruebas exhaustivas para asegurar la fiabilidad y el rendimiento del servicio.
Capturas de pantalla:

