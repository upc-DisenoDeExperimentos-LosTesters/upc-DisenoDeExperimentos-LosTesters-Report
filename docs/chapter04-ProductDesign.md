# Capítulo IV: Product Design

## 4.1. Style Guidelines

En esta parte, exponemos el plan de diseño, estilo y estética que hemos preparado para nuestro proyecto. El enfoque principal de este plan es garantizar una experiencia de usuario de alta calidad, brindando una interfaz que sea accesible, intuitiva y visualmente agradable. Buscamos que cada usuario, sin importar su experiencia tecnológica, pueda navegar con facilidad y disfrute de un entorno atractivo. Para ello, seleccionamos de manera cuidadosa elementos visuales que combinan claridad y estética, como una paleta de colores armónica, tipografías legibles adecuadas al contenido, e iconografía y gráficos que enriquecen el diseño sin recargarlo. Además, hemos definido criterios estrictos para evitar la incorporación de elementos visuales que resulten inadecuados o sobrecarguen la interfaz.

Es importante destacar que un diseño coherente y unificado no solo embellece una plataforma, sino que también potencia su funcionalidad y facilidad de uso. Las directrices de estilo son fundamentales para asegurar una presentación uniforme y profesional en todas las páginas web y actividades móviles del proyecto. Como señala Zeldman (2024), una guía de estilo no solo establece la apariencia y el comportamiento de los componentes de una interfaz, sino que también ofrece un marco de trabajo que promueve la colaboración eficiente entre los equipos de diseño y desarrollo, favoreciendo la consistencia y agilidad en la ejecución del proyecto.

### 4.1.1. General Style Guidelines

**Colores:**

El color es un elemento fundamental y destacado en el diseño de interfaces de usuario, ya que juega un papel clave en la creación de una experiencia visual atractiva. Según Saraswati y Giantari (2022), elegir los colores adecuados para el logotipo y los materiales de marketing de una empresa puede ser determinante para construir una identidad visual única y fácilmente reconocible. Esta identidad no solo ayuda a los consumidores a identificar y recordar la marca, sino que también permite a la empresa generar emociones profundas y subjetivas en su público objetivo. Además, en un mercado altamente competitivo, los colores se convierten en una herramienta esencial para que una marca se distinga de sus competidores. Un esquema de colores original o poco convencional no solo atrae la atención de los consumidores, sino que también hace que la marca sea más memorable y perdure en la mente de los usuarios (Wang et al., 2018).

Para MoviGestión, hemos escogido una paleta que gira en torno al amarillo como color principal, acompañado de grises claros y grises oscuros para aportar equilibrio y versatilidad. Este conjunto no solo realza la identidad de la plataforma, sino que refleja nuestros valores: innovación, fiabilidad y enfoque en la optimización operativa. La paleta principal está compuesta por cinco colores cuidadosamente seleccionados, y se complementa con una gama análoga de entre seis y nueve tonos adicionales, permitiendo adaptaciones contextuales sin perder coherencia visual.

- **Amarillo Solar (#FFC107)**
  El Amarillo Solar es nuestro color primario de referencia. Evoca energía, optimismo y visibilidad, cualidades esenciales para destacar las funciones críticas en MoviGestión, como alertas de ruta, indicadores de rendimiento y llamadas a la acción principales. Desde el punto de vista psicológico, el amarillo estimula la mente y facilita la rápida identificación de elementos interactivos, reforzando la percepción de una plataforma ágil y dinámica.

- **Amarillo Dorado (#FFD54F)**
  Como variación análoga del amarillo principal, el Amarillo Dorado suaviza transiciones y aporta calidez en componentes de fondo, cabeceras secundarias o íconos informativos. Sirve para jerarquizar contenido sin competir con el Amarillo Solar, ofreciendo un degradado luminoso que enriquece la experiencia visual.

- **Amarillo Mostaza (#FFB300)**
  El Amarillo Mostaza refuerza la sensación de solidez y confianza cuando se usa en botones de confirmación, badges o secciones destacadas de estadísticas. Este tono más profundo funciona como un ancla visual, conectando los elementos más críticos con la identidad energética del amarillo principal.

- **Gris Claro (#F5F5F5)**
  El Gris Claro actúa como color complementario, proporcionando un fondo neutro y limpio que realza la legibilidad y el descanso visual. Ideal para superficies extensas (paneles, formularios, listados) y para contener elementos interactivos sin generar fatiga ocular.

- **Gris Oscuro (#424242)**
  Finalmente, el Gris Oscuro provee contraste y estructura: se emplea en tipografías principales, barras de navegación y componentes fijos. Este tono profundo refuerza la percepción de profesionalismo y solidez, asegurando que los elementos de texto y los gráficos tengan excelente legibilidad sobre fondos claros o amarillos.

- **Paleta complementaria análoga**
  Para una mayor flexibilidad, MoviGestión contará con conjuntos de tonos análogos (entre 6 y 9 cada uno) en torno al amarillo y al gris, que incluyen variaciones de brillo y saturación. Esto permitirá adaptar la interfaz a diferentes contextos (módulos de reporte, alertas de seguridad, modos nocturno/diurno) sin perder la cohesión de la marca.

Con esta estructura cromática, garantizamos una experiencia de usuario uniforme y diferenciada, alineada con la misión de LosTesters: impulsar la eficiencia y la confianza en la gestión de flotas a través de la tecnología.

Figura 18
Modelo de división de colores utilizado en Movigestión para el desarrollo de la interfaz

![fonts](/assets/chapter04/color-division.png)

**Tipografía:**

- La selección tipográfica de una marca es un pilar esencial dentro de su identidad visual. Según Dopico (2021), la fuente elegida puede evocar reacciones emocionales en los usuarios, modulando cómo perciben la marca y haciéndola más atractiva, accesible y cercana. No se trata solo de un detalle estético: la tipografía influye en la experiencia afectiva del usuario y en su forma de interactuar con nuestra plataforma. Por eso, resulta imprescindible escoger tipos de letra que refuercen la personalidad y los principios de la empresa, estableciendo así un vínculo emocional sólido con el público objetivo y fomentando su lealtad. Dentro del amplio universo tipográfico, distinguimos dos familias principales:
  **Serif.** Las fuentes con serifas incorporan pequeños remates en los extremos de los caracteres. Estos detalles otorgan un aire más formal, clásico y elegante, por lo que suelen emplearse en textos largos o en soportes impresos—como libros o artículos académicos—donde aportan fluidez a la lectura al guiar la vista de letra en letra (Jay & Lupton, 2024). Ejemplos habituales son Times New Roman y Georgia, ambas valoradas por su legibilidad y su aspecto refinado en medios impresos y digitales.
  **Sans-serif.** Libre de ornamentos, este tipo de letra presenta líneas puras y un diseño más depurado, lo que lo hace muy popular en entornos digitales donde la claridad es prioritaria (Jay & Lupton, 2024). Fuentes como Arial, Helvetica o Roboto (creada específicamente para pantallas) ofrecen un trazo nítido y sencillo, favoreciendo la lectura en interfaces modernas.
  Cuando hablamos de aplicaciones móviles, las tipografías sans-serif se imponen por varias razones:

  1.  Legibilidad en pantallas reducidas. Al carecer de adornos, resultan más legibles en resoluciones pequeñas y minimizan la fatiga visual (Minakata & Beier, 2022).

  2.  Consistencia en distintas densidades de píxeles. Sea un móvil sencillo o un dispositivo de alta gama, las sans-serif conservan su nitidez y facilidad de lectura (Gonzalez-Rodrigueza et al., 2024).

  3.  Estética minimalista. Su sencillez encaja con las tendencias de diseño contemporáneo, centradas en la funcionalidad y un aspecto limpio (Minakata & Beier, 2022).

  4.  Rendimiento en interfaces dinámicas. Al no incluir elementos superfluos, acompañan fluidamente animaciones y desplazamientos sin distraer (Vecino et al., 2022).
      Por todas estas razones, hemos optado por emplear exclusivamente tipografías sans-serif en nuestra aplicación. Dentro de ese universo, seleccionaremos variantes específicas según su contexto de uso (cabeceras, cuerpo de texto, botones, etc.), garantizando siempre una experiencia coherente y óptima para el usuario.

**Tipo de Letra Primaria:**
Para MoviGestión, hemos seleccionado Open Sans como nuestra fuente principal. Open Sans es una tipografía sans-serif reconocida por su neutralidad y excelente legibilidad, cualidades fundamentales para ofrecer una experiencia de usuario clara y accesible. Su diseño contemporáneo y de líneas suaves aporta un equilibrio perfecto entre funcionalidad y estilo, ideal para una plataforma que busca combinar eficiencia y profesionalismo.
La versátil estructura de Open Sans facilita la lectura en cualquier dispositivo y resolución, desde encabezados hasta textos de cuerpo y botones de acción. Sus proporciones armónicas garantizan que el contenido se muestre de modo uniforme, sin importar el tamaño de pantalla. Además, la claridad y precisión de sus formas refuerzan la coherencia visual de MoviGestión, proyectando una imagen pulida y confiable en cada interacción.
Figura 18
Categoría de fuentes utilizadas para la letra primaria en el diseño de Movigestión

![fonts](/assets/chapter04/font-category.png)

**Tono de comunicación y lenguaje aplicado:**

- Según Smith y Zook (2022), el tono de comunicación es un elemento fundamental en el diseño de las páginas, secciones o apartados de una aplicación, ya que influye directamente en cómo la audiencia percibe la marca y su mensaje. Al definir el tono, es importante determinar si el contenido adoptará un estilo formal, informal, técnico o amigable, ya que estas decisiones impactan tanto en las emociones del usuario como en la efectividad de la comunicación. Un tono bien trabajado no solo fortalece la identidad de la empresa o producto, sino que también facilita una mayor conexión emocional con los usuarios, incrementando su sentido de pertenencia.
- Asimismo, las directrices de estilo abarcan aspectos como la selección de palabras, la- construcción de oraciones y el nivel de complejidad del lenguaje, lo cual incide en la claridad,- accesibilidad y capacidad de transmitir confianza y profesionalismo. Considerando el perfil de- nuestros segmentos objetivos, se recomienda utilizar un tono respetuoso y amigable, manteniendo- la formalidad adecuada para el contexto empresarial y el enfoque en el desarrollo profesional.- Este balance favorece que los usuarios se enfoquen en el contenido y refuercen su confianza en- la plataforma.
- En las secciones que explican las funcionalidades de la aplicación y en la presentación de la misión, visión y valores, se sugiere optar por un tono entusiasta que resalte los beneficios y fortalezca la conexión emocional con los usuarios, impulsando su integración al mundo laboral. Por otro lado, se debe emplear un estilo más serio y formal en los apartados críticos, como la interacción con empresas y la presentación de cualidades personales y certificaciones.
- Al mantener este equilibrio entre entusiasmo y formalidad, se logra una comunicación clara, accesible y efectiva que atrae, retiene y genera credibilidad ante los usuarios, asegurando una imagen profesional en todas las áreas de la aplicación.

### 4.1.2. Web Style Guidelines.

Los esquemas cromáticos empleados en la interfaz web de MoviGestión se diseñan con estricto apego a las directrices establecidas en nuestra guía general de estilo. Estas personalizaciones no solo atienden al formato y al estilo de presentación actualizados, sino que también se adaptan de manera dinámica a cada sección o página que el usuario visite. Con el fin de preservar la coherencia visual y facilitar una experiencia fluida, hemos definido distintos entornos en los que los matices y las transparencias se ajustan de forma puntual siguiendo los lineamientos de diseño.

- **Fondos:**
  Para mantener una estética atemporal y garantizar su correcta integración con los variados degradados presentes en la plataforma, hemos optado por una paleta de grises neutros. Esta selección aporta una versatilidad excepcional, pues equilibra la sobriedad y la elegancia sin sacrificar la legibilidad del contenido, sin importar la combinación de colores del fondo. Además, la aplicación de diferentes niveles de opacidad sobre estos grises permite generar contrastes adecuados entre elementos gráficos y tipografía, optimizando así la claridad visual y reduciendo la fatiga ocular.

  En aquellas secciones donde la interfaz requiera destacar módulos secundarios o superponer capas de información, ajustamos cuidadosamente los valores de transparencia para conservar la jerarquía visual. De este modo, cada elemento—ya sea un panel de datos, una tarjeta de notificaciones o un modal de acciones—mantiene su identidad gráfica sin desentonar con el entorno general de la aplicación.

  Con este enfoque, MoviGestión ofrece un diseño riguroso y coherente, capaz de adaptarse a múltiples contextos de uso sin perder la calidad estética ni la funcionalidad que caracterizan nuestra propuesta.

  Figura 19
  Grupo de colores utilizados en los fondos de pantalla en las interfaces de Movigestión

![fonts](/assets/chapter04/color-group.png)

- **Tipografia:**
  La selección cromática para la tipografía en MoviGestión responde directamente al fondo sobre el que se despliega cada elemento textual. Con el fin de conservar una estética clásica y atemporal, hemos adoptado una paleta de grises neutros que se ajusta armoniosamente a una amplia variedad de fondos, desde degradados sutiles hasta superficies de color más intensas. Esta elección aporta una versatilidad visual que conjuga sobriedad y elegancia, garantizando siempre un contraste suave pero definido. De este modo, el lector experimenta una legibilidad óptima en cualquier entorno, mientras la interfaz mantiene un aire de neutralidad que refuerza la identidad corporativa y facilita la adaptación a futuros cambios o añadidos de color.

  Figura 20
  Serie de colores utilizados en la tipografía de Movigestión para el desarrollo web

![fonts](/assets/chapter04/color-series.png)

Para asegurar la máxima claridad y coherencia, hemos definido Open Sans como nuestra tipografía principal. Elegida por su diseño humanista y sus líneas equilibradas, Open Sans ofrece una excelente legibilidad tanto en pantallas de escritorio como en dispositivos móviles. En particular, optamos por el peso Light a un tamaño de 95px para títulos y encabezados destacados. Esta combinación proporciona:

- **Presencia Imponente:** El tamaño generoso de 95 px capta inmediatamente la atención del usuario, ideal para jerarquizar información clave.

- **Elegancia y Delicadeza:** El trazo fino del peso Light aporta una sensación de ligereza visual, evitando la pesadez que pueden generar las fuentes más gruesas en tamaños grandes.

- **Claridad en Alta Resolución:** En pantallas de última generación, donde la densidad de píxeles es elevada, Open Sans Light se conserva nítida y libre de artefactos, asegurando una lectura cómoda y sin esfuerzo.

- **Consistencia de Marca:** Al emplear una tipografía web-segura y de amplio soporte, reforzamos la uniformidad del producto en diferentes navegadores y sistemas operativos.

Con este planteamiento, MoviGestión logra un equilibrio perfecto entre impacto visual y funcionalidad, elevando la experiencia de usuario y subrayando la profesionalidad de la plataforma.

Figura 21
Tamaño de muestra de fuentes utilizadas para la letra primaria de Open Sans Light de MoviGestión

![fonts](/assets/chapter04/font-sizes.png)

### 4.1.3. Mobile Style Guidelines

La versión móvil de MoviGestión ha sido diseñada siguiendo estrictos principios de diseño responsivo, con el objetivo de ofrecer una experiencia táctil optimizada, accesible y visualmente coherente en dispositivos de pantalla reducida. Para lograrlo, se emplean rejillas fluidas basadas en tecnologías como CSS Grid y Flexbox, acompañadas de puntos de quiebre adaptativos que reorganizan dinámicamente el contenido de acuerdo con la orientación y el ancho disponible en la pantalla del dispositivo.
Con el fin de mejorar la precisión y comodidad de la interacción táctil, se respetan las zonas mínimas recomendadas de interacción: 44×44 pt en dispositivos iOS y 48×48 dp en entornos Android, conforme a las directrices establecidas por Apple Human Interface Guidelines y Material Design, respectivamente. Este enfoque minimiza los errores de interacción y garantiza que todos los elementos sean fácilmente accesibles mediante gestos naturales.
La navegación en la versión móvil se organiza utilizando patrones estandarizados y familiares para el usuario. En Android, se implementan barras de navegación inferiores con entre tres y cinco destinos principales, siguiendo los lineamientos de Material Design; mientras que en iOS se emplea la barra de pestañas nativa, asegurando así una experiencia coherente con las expectativas de cada ecosistema.
En cuanto a la tipografía, se respetan los sistemas tipográficos característicos de cada plataforma para maximizar la legibilidad y cohesión visual:

- **Android:**
  Se utiliza la fuente Roboto, con un tamaño mínimo de 14 sp para textos de cuerpo y 20 sp para encabezados, en cumplimiento de la escala tipográfica sugerida por Material Design.

- **iOS:**
  Se emplea la familia tipográfica San Francisco, con un tamaño mínimo de 11 pt para cuerpos de texto y 17 pt para títulos, habilitando además la funcionalidad de ajuste dinámico del tamaño de texto (Dynamic Type) para mejorar la accesibilidad y adaptabilidad de la lectura.

Asimismo, se asegura un contraste mínimo de 4.5:1 entre el texto y el fondo, en conformidad con las pautas de accesibilidad WCAG (Web Content Accessibility Guidelines), y se proporciona soporte completo para modos claro y oscuro, adaptándose a las preferencias del usuario. Los componentes interactivos se destacan mediante el uso de bordes suaves, sombras sutiles y microanimaciones que refuerzan la respuesta visual ante acciones táctiles. <br>
En materia de accesibilidad, MoviGestión se compromete a cumplir criterios fundamentales, incluyendo:

- Etiquetado adecuado de elementos (uso de accesibilityLabel y roles semánticos correctos).
- Compatibilidad con lectores de pantalla.
- Soporte para ajuste dinámico del tamaño de fuente a demanda del usuario.

Finalmente, se mantiene la coherencia visual y de marca mediante el uso consistente de la paleta de colores, iconografía y espaciados definidos en la versión web, adaptándonos cuidadosamente a las convenciones gráficas y de interacción propias de cada sistema operativo. De este modo, MoviGestión asegura una experiencia de usuario fluida, intuitiva y en completa sintonía con los estándares de calidad más exigentes en diseño de aplicaciones móviles.

#### 4.1.3.1. iOS Mobile Style Guidelines

- **Aplicación de las Human Interface Guidelines para la versión iOS de MoviGestión:**
  Con el objetivo de garantizar una experiencia de usuario fluida, accesible y plenamente integrada en el ecosistema de Apple, la versión iOS de MoviGestión sigue de manera estricta las recomendaciones establecidas en las Human Interface Guidelines.
- **Tamaño mínimo de áreas táctiles:**
  Siguiendo las directrices oficiales, todos los controles interactivos cuentan con un área táctil mínima de 44 × 44 puntos. Esta dimensión asegura que los usuarios puedan interactuar fácilmente con botones, iconos y enlaces, minimizando el riesgo de toques accidentales y mejorando la precisión en la navegación táctil. De este modo, se optimiza tanto la accesibilidad como la comodidad general en el uso de la aplicación.

Figura 22
Ejemplo de división de tamaño mínimo de áreas táctiles en distintos dispositivos

![fonts](/assets/chapter04/device-sizes.png)

- **Tipografía San Francisco y Dynamic Type:**
  MoviGestión utiliza como fuente principal la familia San Francisco, la tipografía oficial de Apple para sus dispositivos. Además, se integra el soporte para Dynamic Type, permitiendo que los usuarios ajusten dinámicamente el tamaño de la letra desde los ajustes del sistema. Esta implementación no solo mejora la legibilidad para un amplio rango de usuarios, sino que también respeta las preferencias individuales de accesibilidad, asegurando una experiencia personalizada e inclusiva.

Figura 23
Modelo de tipografía San Francisco Dynamic Type, utilizada en el la versión de iOS de MoviGestión
![fonts](/assets/chapter04/san-francisco.png)

- **Barra de pestañas inferior (Tab Bar):**
  La navegación principal de la aplicación se estructura mediante el uso de una UITabBar nativa, conforme a los estándares de diseño de iOS. Se utilizan iconos claros y etiquetas legibles que identifican de forma precisa las secciones principales —como Inicio, Órdenes y Perfil—, garantizando un acceso rápido, intuitivo y consistente a las funcionalidades más relevantes de MoviGestión.

Figura 24
Modelo de UITabBar utilizado para la interfaz principal de MoviGestión
![fonts](/assets/chapter04/tab-bar.png)

- **Gestos y transiciones:**
  Se aprovechan al máximo los gestos nativos del sistema operativo, tales como el swipe horizontal para cambiar de vistas y el pull-to-refresh para actualizar contenidos dinámicamente. Además, se integran animaciones suaves mediante el uso de UIKit Dynamics, proporcionando una experiencia de navegación intuitiva, fluida y alineada con el comportamiento esperado de las aplicaciones de alta calidad en iOS.

Figura 25
Modelo de gestos utilizados para el funcionamiento de la Experiencia de Usuario de Movigestión

![fonts](/assets/chapter04/gestures.png)

- **Modo claro/oscuro:**
  MoviGestión ofrece soporte completo para el modo claro y el modo oscuro de iOS, adaptando automáticamente su paleta de colores, iconografía e imágenes para preservar el contraste, la legibilidad y la consistencia estética en ambos modos de visualización. Esta adaptación se realiza de manera cuidadosa, asegurando que la identidad visual de la aplicación se mantenga sólida y reconocible, independientemente de las preferencias de visualización del usuario.

Figura 26
Modelo de gestos utilizados para el funcionamiento de la Experiencia de Usuario de Movigestión
![fonts](/assets/chapter04/polarity.png)

#### 4.1.3.2. Android Mobile Style Guidelines.

- **Aplicación de las Pautas de Material Design para la versión Android de MoviGestión:**
  Con el fin de ofrecer una experiencia de usuario intuitiva, accesible y en perfecta sintonía con los principios de diseño de Android, la versión de MoviGestión para dispositivos Android adopta de manera rigurosa las recomendaciones establecidas en Material Design.

- **Dimensiones y separación de áreas táctiles:**
  Se definen touch targets con un tamaño mínimo de 48 × 48 dp, asegurando que todos los elementos interactivos sean lo suficientemente grandes para facilitar su uso en pantallas táctiles. Además, se mantiene una separación mínima de 8 dp entre los controles, reduciendo el riesgo de toques accidentales y optimizando la precisión y comodidad en la navegación.

Figura 27
Modelo de separación de áreas táctiles junto a sus dimensiones de toque
![fonts](/assets/chapter04/separation-area.png)

- **Bottom Navigation Bar:**
  La navegación principal se implementa mediante la Bottom Navigation Bar de Material Design, que incluye entre tres y cinco destinos principales. Esta barra combina iconos y etiquetas persistentes para identificar claramente las secciones más importantes, ofreciendo un acceso directo, coherente y eficiente a las funciones esenciales de MoviGestión.

Figura 28
Barra de navegación utilizada en la versión de Android de Movigestión
![fonts](/assets/chapter04/navbar.png)

- Tipografía Roboto:
  Se emplea la fuente oficial Roboto, optimizada para pantallas digitales y adaptada a los principios de Material Design. Se establece una escala tipográfica donde se utiliza un tamaño mínimo de 14 sp para el cuerpo del texto y 20 sp para los encabezados principales. Esta jerarquía tipográfica garantiza una presentación clara, legible y estructurada del contenido, mejorando la comprensión y la experiencia de lectura en todo tipo de dispositivos Android.

Figura 29
Serie de tamaño de fuentes de la tipografía Roboto para Movigestión
![fonts](/assets/chapter04/roboto.png)

- Floating Action Button (FAB):
  Se incorpora un único Floating Action Button (FAB) para representar la acción primaria de cada pantalla, en conformidad con las mejores prácticas de Material Design. El diseño del FAB asegura un contraste mínimo de 3:1 entre el icono y su fondo, garantizando su visibilidad en todo tipo de escenarios de uso. En caso de expansión del FAB para mostrar acciones secundarias, se limita el número de opciones desplegadas a un máximo de seis, evitando la sobrecarga cognitiva y manteniendo la simplicidad en la interacción.

Figura 30
Modelo de botones flotantes utilizados en la interfaz Android de Movigestión.
![fonts](/assets/chapter04/floating-buttons.png)

- Animaciones de Material Motion:
  Se siguen las pautas de Material Motion para proporcionar animaciones naturales y coherentes que mejoran la experiencia del usuario sin distraerlo. Todas las transiciones y microinteracciones tienen una duración máxima de 300 milisegundos y emplean curvas de animación estándar, como el standard easing, lo que permite una respuesta fluida y predecible del sistema ante las acciones del usuario.

Figura 31
Guía de animaciones utilizadas para la aplicación Android de Movigestión.
![fonts](/assets/chapter04/animations.png)

## 4.2. Information Architecture

La arquitectura de la información de MoviGestión ha sido concebida cuidadosamente para facilitar la comprensión, la navegación y el uso eficiente de la aplicación, priorizando siempre la experiencia del usuario. Se han implementado sistemas de organización estructurados que permiten a los usuarios localizar, acceder y gestionar información de forma intuitiva, eficiente y contextualizada según sus necesidades operativas.

### 4.2.1. Organization Systems.

Para presentar el contenido de manera coherente y en sintonía con las necesidades específicas de los usuarios, se han definido en MoviGestión tres grandes patrones de organización de la información: jerárquico (visual), secuencial y matricial. Estos patrones se complementan con esquemas de categorización adicionales, tales como el ordenamiento alfabético, la agrupación por tópicos y la segmentación por audiencia.

1. Organización jerárquica
   Todo el contenido dentro de la plataforma se estructura siguiendo niveles claros y bien diferenciados, facilitando una navegación intuitiva. El menú principal agrupa las principales secciones operativas: Dashboard, Flotas, Conductores, Órdenes, Reportes y Configuración. Cada sección, a su vez, desplegará subsecciones organizadas en función de su prioridad y frecuencia de uso.

Los títulos de nivel superior y las acciones críticas, como el botón “Crear Orden”, se destacan mediante tamaños tipográficos prominentes y colores diferenciadores, guiando la atención del usuario hacia las funcionalidades más relevantes. Esta estructura jerárquica no sólo mejora la eficiencia en la localización de opciones, sino que también reduce la carga cognitiva del usuario, facilitando un flujo de trabajo fluido y lógico.

2. Organización secuencial
   Para los procesos operativos más importantes, como la creación de una nueva orden de transporte, se ha optado por un flujo secuencial de pasos claramente definidos. El usuario avanza a través de un proceso progresivo compuesto por las siguientes etapas:

- Selección del vehículo
- Asignación del conductor
- Definición de la ruta
- Confirmación de la orden

Cada paso muestra únicamente los campos esenciales requeridos en esa fase, minimizando la sobrecarga de información. El avance a través del flujo se indica mediante elementos visuales como una barra de progreso superior o breadcrumbs, permitiendo al usuario conocer en todo momento su ubicación dentro del proceso y anticipar los pasos siguientes. Esta metodología reduce el margen de error, optimiza el tiempo de interacción y favorece una experiencia de uso más amigable y estructurada.

3. Organización matricial y esquemas de categorización
   Para la gestión y comparación de conjuntos de datos más complejos, MoviGestión emplea un enfoque matricial, utilizando tablas en las que cada fila representa un ítem individual (por ejemplo, un vehículo) y las columnas reflejan atributos clave (como conductor asignado, última ruta realizada, estado operativo, entre otros).

Complementariamente, se aplican distintos esquemas de categorización para facilitar la búsqueda rápida y eficiente de información relevante:

- **Orden alfabético:**
  La lista de conductores se organiza de la A a la Z, agilizando la localización de un perfil específico mediante criterios reconocibles.

- **Clasificación por tópicos:**
  Dentro del módulo de Reportes, las métricas se agrupan en categorías como Rendimiento, Consumo de Combustible y Mantenimiento Preventivo, ofreciendo una organización lógica que refleja los focos de gestión operativa.

- **Segmentación por audiencia:**
  El contenido se personaliza en función del rol del usuario. Por ejemplo, un administrador puede acceder a métricas globales de desempeño de la flota, mientras que un conductor visualiza únicamente la información relacionada con sus rutas asignadas y desempeño personal.

La combinación de un esquema matricial y una categorización múltiple permite una comparación simultánea y efectiva de múltiples elementos, favoreciendo la toma de decisiones informada y la optimización de procesos en la gestión de flotas.

### 4.2.2. Labeling Systems.

Con el objetivo de asegurar que cada elemento de la interfaz de MoviGestión comunique su propósito de forma clara, precisa y coherente, hemos implementado las mejores prácticas en materia de etiquetado y nomenclatura. Estas buenas prácticas incluyen el uso de etiquetas breves y descriptivas, la aplicación consistente de reglas de capitalización, la incorporación de verbos de acción en botones y llamadas a la acción (CTAs), y la selección de términos que resulten familiares y comprensibles para nuestro público objetivo.

A continuación, se describen las estrategias de etiquetado adoptadas en las distintas áreas de la plataforma:

1. **Navegación principal (Navbar)**
   La barra de navegación principal organiza las secciones más relevantes de la aplicación, siguiendo una lógica funcional y de fácil acceso para el usuario:

- Dashboard: Centro de control que agrupa las métricas más importantes y proporciona accesos rápidos a las principales funcionalidades como flotas, órdenes y reportes.

- Flotas: Visualización de la lista completa de vehículos registrados, junto con su estado operativo actualizado.

- Conductores: Registro detallado de todos los conductores, incluyendo sus asignaciones actuales y antecedentes de rutas.

- Órdenes: Gestión integral del historial de órdenes, permitiendo tanto el monitoreo de las órdenes en curso como la consulta de las finalizadas.

- Reportes: Acceso directo a informes analíticos sobre desempeño de flotas, consumo de combustible y actividades de mantenimiento preventivo y correctivo.

- Ajustes: Sección dedicada a la configuración de parámetros de usuario, gestión de roles, personalización de preferencias y ajustes generales de la aplicación.

2. **Encabezados de Sección (Page Headings)**
   Cada pantalla principal de la plataforma cuenta con un encabezado claramente definido, que establece el contexto de la información o la tarea que el usuario está visualizando o ejecutando:

- **Resumen de Flota:** Encabezado que introduce la sección de visualización del estado general de la flota de vehículos.

- **Crear Nueva Orden:** Título que marca el inicio del proceso secuencial para la generación de una nueva orden de transporte.

- **Detalle de Reporte:** Encabezado de las pantallas dedicadas al análisis detallado de métricas específicas relacionadas con el rendimiento operativo.

- **Perfil de Usuario:** Indicación de la sección donde el usuario puede consultar y editar sus datos personales y preferencias de uso.

3. **Botones y Llamadas a la Acción (CTAs)**

Las llamadas a la acción (Call to Actions) se redactan utilizando verbos en infinitivo para indicar de manera directa e inmediata la acción que el usuario puede realizar:

- **Añadir Orden:** En lugar de "Crear orden", se emplea un verbo de acción en infinitivo para indicar la tarea de forma más natural y activa.

- **Guardar Cambios:** CTA que confirma la intención de persistir modificaciones realizadas en un formulario o sección editable.

- **Filtrar Resultados:** Botón disponible en tablas de datos que permite aplicar criterios específicos de búsqueda y segmentación.

- **Exportar PDF:** Acción que indica la generación y descarga de un reporte en formato PDF.

- **Volver al Dashboard:** CTA que permite regresar de manera clara y directa al panel principal de control.

4. **Campos de Formulario y Validación**
   En los formularios, cada campo cuenta con etiquetas claras y textos de ayuda que guían al usuario en la introducción correcta de la información:

- **Vehículo (placa):** Campo de texto acompañado de un ejemplo de formato (“ej. ABC-123”) para minimizar errores de entrada.

- **Conductor (nombre completo):** Campo con autocompletado habilitado, donde etiqueta y placeholder siguen una nomenclatura uniforme.

- **Fecha de entrega:** Campo que despliega un selector de calendario emergente para facilitar la elección de fechas válidas.

- **Comentarios adicionales:** Área de texto opcional con contador de caracteres visible, permitiendo controlar la extensión de los comentarios.

- **Enviar Orden:** Botón de acción principal en los formularios de órdenes, siempre visible en la parte inferior de la pantalla para un acceso rápido.

5. **Enlaces de Pie de Página (Footer)**
   El pie de página incluye enlaces informativos y de soporte que refuerzan la transparencia, el acompañamiento al usuario y el cumplimiento normativo:

- **Acerca de:** Enlace a información corporativa, visión, misión y valores de MoviGestión.

- **Centro de Ayuda:** Acceso a una colección de preguntas frecuentes (FAQs) y guías de usuario para resolver dudas comunes.

- **Términos y Condiciones:** Documento legal que regula el uso de la plataforma por parte de los usuarios.

- **Política de privacidad:** Declaración detallada sobre el tratamiento de datos personales y uso de cookies.

- **Contáctanos:** Acceso directo a un formulario de soporte para enviar consultas, incidencias o solicitudes específicas.

### 4.2.3. SEO Tags and Meta Tags

Para maximizar la visibilidad de la Landing Page de MoviGestión en buscadores y redes sociales, hemos definido un conjunto de metaetiquetas que describen el contenido, guían el rastreo y mejoran la apariencia de nuestros enlaces compartidos:

1. **Etiqueta de título (Title Tag)**
   Un título conciso (50–60 caracteres) ayuda a los usuarios a comprender de un vistazo de qué trata la página y evita que Google lo trunque en los resultados de búsqueda . Para MoviGestión hemos elegido:
   MoviGestión – Gestión de flotas empresariales en un solo lugar

2. **Meta descripción (Description Tag)**
   Un resumen claro de 50–160 caracteres que incluya nuestras palabras clave principales mejora la tasa de clics (CTR) desde el SERP, ofreciendo al usuario un adelanto de los beneficios de la plataforma . Propuesta para MoviGestión:
   MoviGestión simplifica la gestión de flotas: estadísticas en tiempo real, reportes de incidencias, seguimiento de envíos y planes flexibles para optimizar tu transporte empresarial.

3. **Meta keywords**
   Aunque Google dejó de utilizarlas como factor de ranking en 2009, algunas plataformas secundarias o CMS internos aún pueden beneficiarse de ellas. Mantendremos una lista breve y relevante para documentar nuestra intención:
   gestión de flotas, transporte empresarial, logística, seguimiento de envíos, reportes de rendimiento.

4. **Robots**
   Para garantizar que los motores de búsqueda indexen todas nuestras páginas y sigan los enlaces internos, empleamos: index, follow .

5. **Canonical**
   Señalamos la URL preferida de cada página para evitar contenido duplicado y consolidar señales de enlaces externos en una única dirección.

### 4.2.4. Searching Systems.

Con el propósito de maximizar la visibilidad de la Landing Page de MoviGestión en motores de búsqueda y plataformas de redes sociales, hemos definido cuidadosamente un conjunto integral de metaetiquetas. Estas metaetiquetas permiten describir el contenido de manera precisa, orientar el rastreo de los buscadores y optimizar la presentación de los enlaces compartidos, mejorando así tanto la accesibilidad como el atractivo de la página en diferentes canales digitales.

A continuación, se detallan los principales elementos establecidos:

1. **Barra de búsqueda global con autocompletado**
   La barra de búsqueda, presente en la cabecera de cada pantalla, permite introducir términos libres (por ejemplo, número de orden o nombre de conductor). Ofrece sugerencias instantáneas basadas en coincidencias parciales y búsquedas frecuentes, y usa un retardo (“debounce”) de 300 ms para evitar sobrecarga de consultas al servidor y mejorar la fluidez de la experiencia.

2. **Filtrado (sidebar de filtros)**
   En la vista de resultados, una columna lateral agrupa los filtros más relevantes (Estado, Fecha, Tipo de servicio, Conductor). Cada categoría se muestra con checkboxes, sliders o menús desplegables según el tipo de dato, permitiendo aplicar múltiples criterios para afinar la búsqueda.

3. **Chips de filtros aplicados y limpieza rápida**
   Al activar un filtro, aparece un “chip” encima de la lista de resultados que muestra el criterio seleccionado (“Estado: En curso”). El usuario puede quitar cada filtro individual con un clic en la “X” o restablecer todos con un botón “Limpiar filtros”, recuperando la búsqueda global sin pasos adicionales

### 4.2.5. Navigation Systems.

MoviGestión ofrece un conjunto de patrones de navegación diseñados para que el usuario encuentre lo que busca con el mínimo esfuerzo y sin perderse en caminos secundarios. A continuación presentamos una versión optimizada de las técnicas empleadas:

1. **Navegación global persistente**
   El menú principal permanece visible en todo momento: en escritorio como barra horizontal en la cabecera, y en móvil como panel deslizante (drawer) o barra de pestañas inferior (tab bar) para las 5–7 secciones clave (Dashboard, Flotas, Conductores, Órdenes, Reportes, Ajustes). Los ítems se ordenan según frecuencia de uso y siguen la regla de no exceder 7–9 enlaces top-level para mantener la claridad.

2. **Breadcrumbs y navegación contextual**
   Bajo la cabecera de cada página se muestran “migas de pan” (breadcrumbs) que indican la ruta seguida (p. ej., Dashboard > Órdenes > Detalle), permitiendo al usuario volver a niveles superiores sin usar el botón atrás del navegador. Además, se incluyen enlaces “relacionados” en el pie de sección para explorar contenido afín.

3. **Desplazamiento anclado y scroll-spy**
   En la Landing Page, cada bloque (Inicio, Servicios, Precios, FAQs) cuenta con un ancla y la navegación “scroll-spy” resalta en el menú el punto activo al hacer scroll. Esto guía el recorrido secuencial y refuerza la sensación de orientación.

4. **Llamadas a la acción (CTAs) estratégicas**
   Los botones de descarga (“App Store”, “Google Play”) y de registro/inicio de sesión aparecen en puntos de alta visibilidad: hero, pie de cada sección y footer. Se emplea contraste alto y verbos claros en infinitivo (“Descargar”, “Registrarse”) para maximizar la conversión.

5. **Selector de idioma accesible**
   Un switcher de idioma (ES / EN) se sitúa en la esquina superior derecha. Al cambiarlo, todos los enlaces de navegación y CTAs se traducen al instante, garantizando coherencia y minimizando fricciones para usuarios multilingües.

6. **Navegación secundaria en el footer**
   El pie de página agrupa enlaces menos prioritarios en columnas temáticas: Empresa (Acerca, Equipo), Ayuda (FAQs, Soporte), Legal (Términos, Privacidad) y Social. Su diseño en cuadrícula facilita la exploración rápida sin recargar el header.
   Con estas estrategias combinadas, MoviGestión asegura que tanto usuarios nuevos como recurrentes puedan orientarse y cumplir sus objetivos (buscar órdenes, generar reportes o descargar la app) de forma rápida, intuitiva y coherente en todos los dispositivos.

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

La landing page consta de 6 secciones, sin incluir el navbar y el footer. La sección principal es un hero con el objetivo de captar la atención del usuario y motivarlo a seguir navegando. A continuación, se encuentran "about us" y "about team", donde se describen los beneficios de la web y se presentan los miembros del equipo. En la sección de "services", se pueden ver las características y funcionalidades principales de la web. Finalmente, en las secciones de "pricing" y "contact us" se describe el plan de pago y se muestra un formulario para que el usuario se ponga en contacto con nosotros.

Figura 32
Modelo de Wireframes de la Landing Page de la aplicación móvil
![fonts](/assets/chapter04/landing-wireframe.png)

Figura 33
Wireframe de modelo de error 404 en la Landing Page móvil
![fonts](/assets/chapter04/landing-404-wireframe.jpeg)

### 4.3.2. Landing Page Mock-up

El mockup siguió el orden establecido previamente tanto para el Desktop Web Browser como para el Mobile Web Browser. Se priorizó el uso de una paleta de grises que se ajustara al sector del transporte con el que trabajamos, resaltando el color amarillo para fluir entre las transiciones. Además, se utilizó la tipografía Open Sans para mantener una apariencia limpia y elegante. Estos detalles se pueden encontrar en las referencias.

Figura 34
Modelo de Mockups de la Landing Page de la aplicación móvil
![fonts](/assets/chapter04/landing-mockup.png)

Figura 35
Mockups de modelo de error 404 en la Landing Page móvil
![fonts](/assets/chapter04/landing-404-mockup.jpeg)

## 4.4. Mobile Applications UX/UI Design

### 4.4.1. Mobile Applications Wireframes

En esta sección introduciremos los Wireframes de nuestro proyecto. Para ello, hemos hecho uso de la aplicación Figma.

Link de Figma: https://www.figma.com/design/gu0SdYkebsOKLB8p5YvOzL/BicasTeam-AppMobile?node-i d=0-1&t=pWIPFUunkX9T0x0G-1

Figura 36
Modelo UX/UI design de la aplicación móvil para la página de inicio de sesión
![fonts](/assets/chapter04/login-mobile-wireframe.jpeg)

Figura 37
Modelo UX/UI design de la aplicación móvil para la página de perfiles
![fonts](/assets/chapter04/profile-mobile-wireframe.jpeg)

Figura 38
Modelo UX/UI design de la aplicación móvil para la página de envíos
![fonts](/assets/chapter04/orders-mobile-wireframe.jpeg)

Figura 39
Modelo UX/UI design de la aplicación móvil para la página de vehiculos
![fonts](/assets/chapter04/vehicle-mobile-wireframe.jpeg)

Figura 40
Modelo UX/UI design de la aplicación móvil para la página de reportes
![fonts](/assets/chapter04/reports-mobile-wireframe.jpeg)

### 4.4.2. Mobile Applications Wireflow Diagrams

**User Goal:** El usuario tiene dos opciones de registro en la aplicación: como
“Businessmen” o como “Transportist”.

Si el usuario elige registrarse como “Businessmen”, el proceso comienza en la
pantalla de registro, donde se solicitan datos del usuario, como correo electrónico y
contraseña, así como datos personales.

Si el usuario completa todos los campos requeridos con información válida, acepta los términos y condiciones y hace clic en el botón “Crear cuenta”, se mostrará un formulario. En este formulario, el usuario deberá ingresar los correos
electrónicos de los conductores que forman parte de su flota de vehículos.

Si el usuario completa este formulario correctamente, aparecerá una ventana con el mensaje “REGISTRO EXITOSO”. Si no, se mostrará un mensaje que indica “El correo es inválido o no existe”.

Si el usuario elige registrarse como “Transportist”, el proceso también comienza en la
pantalla de registro, donde se solicitan datos del usuario y datos personales. Si el usuario completa todos los campos requeridos con información válida, acepta los términos y condiciones y hace clic en el botón “Crear cuenta”, aparecerá una ventana con el mensaje “REGISTRO EXITOSO. Ahora eres parte de la organización [Nombre de la Empresa]”. Si no, se mostrará un mensaje que indica “El correo es inválido o no existe”.

Figura 41
Wireflow de la aplicación móvil para el registro de cuentas e inicio de sesión
![fonts](/assets/chapter04/login-mobile-wireflow-1.jpeg)
![fonts](/assets/chapter04/login-mobile-wireflow-2.jpeg)

### 4.4.3. Mobile Applications Mock-ups

En esta sección introduciremos los Mock-Ups de nuestro proyecto. Para ello, hemos hecho uso de la aplicación Figma.

Link de Figma: https://www.figma.com/design/gu0SdYkebsOKLB8p5YvOzL/BicasTeam-AppMobile?node-i d=0-1&t=pWIPFUunkX9T0x0G-1

![fonts](/assets/chapter04/mobile-mockup-1.jpeg)
![fonts](/assets/chapter04/mobile-mockup-2.jpeg)
![fonts](/assets/chapter04/mobile-mockup-3.png)
![fonts](/assets/chapter04/mobile-mockup-4.png)

### 4.4.4. Mobile Applications User Flow Diagrams

En esta parte del proyecto se realizará la creación de los User Flow Diagrams para la aplicación móvil. Estos diagramas se encargarán de mostrar visualmente el recorrido que los usuarios seguirán dentro de la app para completar tareas específicas. Para ello, se deberán identificar las pantallas clave, las decisiones que los usuarios pueden tomar y las interacciones que conectan cada acción con la pantalla o función siguiente.

**User Goal: El usuario puede registrarse como Transportista o Gerente.**
![fonts](/assets/chapter04/mobile-userflow-1.jpeg)
**User Goal: El usuario puede iniciar sesión dependiendo de su tipo de usuario**
![fonts](/assets/chapter04/mobile-userflow-2.jpeg)
**User Goal: Usuario puede actualizar sus datos **
![fonts](/assets/chapter04/mobile-userflow-3.png)
**User Goal: Gerente puede asignar un nuevo envío**
![fonts](/assets/chapter04/mobile-userflow-4.png)
**User Goal: Gerente puede eliminar un envío**
![fonts](/assets/chapter04/mobile-userflow-5.png)
**User Goal: Gerente registra un nuevo vehículo**
![fonts](/assets/chapter04/mobile-userflow-6.png)
**User Goal: Transportista puede registrar un nuevo reporte**
![fonts](/assets/chapter04/mobile-userflow-7.png)

## 4.5. Mobile Applications Prototyping

### 4.5.1. Android Mobile Applications Prototyping

Se realizó la creación de un prototipo interactivo para la aplicación móvil Android utilizando Figma. El prototipo muestra el flujo principal de navegación, las pantallas clave y la estructura inicial de la interfaz de usuario. Para complementar esta fase, se elaboró un video demostrativo donde se presenta el recorrido completo por el prototipo, permitiendo visualizar la experiencia de usuario prevista.

![fonts](/assets/chapter04/android-prototyping.jpeg)

https://upcedupe-my.sharepoint.com/:v:/g/personal/u20201f572_upc_edu_pe/ET9JS4FGvSNDltJpP5nEhn8Bql7cxtMuvxPaCU5ZJFP5pw?e=o6QBex&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

### 4.5.2. iOS Mobile Applications Prototyping

![fonts](/assets/chapter04/android-prototyping.jpeg)

https://upcedupe-my.sharepoint.com/:v:/g/personal/u20201f572_upc_edu_pe/ET9JS4FGvSNDltJpP5nEhn8Bql7cxtMuvxPaCU5ZJFP5pw?e=o6QBex&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

## 4.6. Web Applications UX/UI Design

### 4.6.1. Web Applications Wireframes

![fonts](/assets/chapter04/webApp-wireframe-1.jpeg)
![fonts](/assets/chapter04/webApp-wireframe-2.png)
![fonts](/assets/chapter04/webApp-wireframe-3.png)

### 4.6.2. Web Applications Wireflow Diagrams

**User Goal:** El usuario tiene dos opciones de registro en la aplicación: como “Businessmen” o como “Transportist”.

Si el usuario elige registrarse como “Businessmen”, el proceso comienza en la pantalla de registro, donde se solicitan datos del usuario, como correo electrónico y contraseña, así como datos personales. Si el usuario completa todos los campos requeridos con información válida, acepta los términos y condiciones y hace clic en el botón “Crear cuenta”, se mostrará un formulario. En este formulario, el usuario deberá ingresar los correos electrónicos de los conductores que forman parte de su flota de vehículos. Si el usuario completa este formulario correctamente, aparecerá una ventana con el mensaje “REGISTRO EXITOSO”. Si no, se mostrará un mensaje que indica “El correo es inválido o no existe”.

Si el usuario elige registrarse como “Transportist”, el proceso también comienza en la pantalla de registro, donde se solicitan datos del usuario y datos personales. Si el usuario completa todos los campos requeridos con información válida, acepta los términos y condiciones y hace clic en el botón “Crear cuenta”, aparecerá una ventana con el mensaje “REGISTRO EXITOSO". Ahora eres parte de la organización [Nombre de la Empresa]”. Si no, se mostrará un mensaje que indica “El correo es inválido o no existe”.

![fonts](/assets/chapter04/webApp-wireflow-1.png)
![fonts](/assets/chapter04/webApp-wireflow-2.png)

### 4.6.3. Web Applications Mock-ups

![fonts](/assets/chapter04/webApp-mockup-1.png)
![fonts](/assets/chapter04/webApp-mockup-2.png)
![fonts](/assets/chapter04/webApp-mockup-3.png)
![fonts](/assets/chapter04/webApp-mockup-4.png)
![fonts](/assets/chapter04/webApp-mockup-5.png)

### 4.6.4. Web Applications User Flow Diagrams

**User Goal:** El usuario tiene dos opciones de registro en la aplicación: como “Businessmen” o como “Transportist”.

Si el usuario elige registrarse como “Businessmen”, el proceso comienza en la pantalla de registro, donde se solicitan datos del usuario, como correo electrónico y contraseña, así como datos personales. Si el usuario completa todos los campos requeridos con información válida, acepta los términos y condiciones y hace clic en el botón “Crear cuenta”, se mostrará un formulario. En este formulario, el usuario deberá ingresar los correos electrónicos de los conductores que forman parte de su flota de vehículos. Si el usuario completa este formulario correctamente, aparecerá una ventana con el mensaje “REGISTRO EXITOSO”. Si no, se mostrará un mensaje que indica “El correo es inválido o no existe”.

Si el usuario elige registrarse como “Transportist”, el proceso también comienza en la pantalla de registro, donde se solicitan datos del usuario y datos personales. Si el usuario completa todos los campos requeridos con información válida, acepta los términos y condiciones y hace clic en el botón “Crear cuenta”, aparecerá una ventana con el mensaje “REGISTRO EXITOSO". Ahora eres parte de la organización [Nombre de la Empresa]”. Si no, se mostrará un mensaje que indica “El correo es inválido o no existe”.

![fonts](/assets/chapter04/webApp-useflow-1.png)

![fonts](/assets/chapter04/webApp-useflow-2.png)

## 4.7. Web Applications Prototyping

## 4.8. Domain-Driven Software Architecture

### 4.8.1. Software Architecture Context Diagram

![fonts](/assets/chapter04/context-diagram.png)

### 4.8.2. Software Architecture Container Diagrams

![fonts](/assets/chapter04/container-diagram.png)

### 4.8.3. Software Architecture Components Diagrams

![fonts](/assets/chapter04/component-diagram-1.png)
![fonts](/assets/chapter04/component-diagram-2.png)

## 4.9. Software Object-Oriented Design

### 4.9.1. Class Diagrams

![fonts](/assets/chapter04/class-diagrams.png)

Link for LucidChart: https://lucid.app/lucidchart/2d956275-81a0-403d-b9f2-005fa58431f6/edit?viewport_loc=-1886%2C-1663%2C3923%2C1908%2C0_0&invitationId=inv_f6f786bf-d4b8-4d72-bd35-97214589f959

### 4.9.2. Class Dictionary

En esta seccion se definiran las clase que se identificaron en el Class Diagram:

- **Class Vehicules:** Representa los vehículos en el sistema.
- **Class ReportVehicule:** Representa los informes relacionados con los vehículos en el sistema.
- **Classs ReportInfraction:** Representa los informes de infracción relacionados con los vehículos en el sistema.
- **Class VehiculeFeatures**: Representa las características de los vehículos en el sistema.
- **Class Feaures:** Representa las características en general.
- **Class Carriers:** Representa a los transportistas en el sistema.
- **Class CarrierContacts:** Representa los contactos relacionados con los transportistas en el sistema.
- **Class Managers:** Representa a los gerentes en el sistema.
- **Class ManagerContacts:** Representa los contactos relacionados con los gerentes en el sistema.
- **Class Items:** Representa los artículos en el sistema.
- **Class Packet:** Representa los paquetes en el sistema.
- **Class ReportPacket:** Representa los informes relacionados con los paquetes en el sistema.
- **Class HasShipped:** Representa los envíos en el sistema.
- **Class TransportationCost:** Representa los costos de transporte en el sistema.
- **Class ReportAccident:** Representa los informes relacionados con los accidentes en el sistema.
- **Class Destination:** Representa los destinos en el sistema.
- **Class VehiculeRoute:** Representa las rutas de vehículos en el sistema

## 4.10. Database Design

### 4.10.1. Relational/Non-Relational Database Diagram

![fonts](/assets/chapter04/database-diagram.png)

Link for Vetabelo: https://my.vertabelo.com/public-model-view/5yI4V4ChbQGarfXWiMjxVVIcacFNuarlrFWq26NToht19NwAIKDlIQ60hc4OJ0M4?x=1918&y=2759&zoom=0.6028
