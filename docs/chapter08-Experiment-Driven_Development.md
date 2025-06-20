## 8.1. Experiment Planning

El Experiment Planning dentro del proceso XDPD es la etapa en la que se definen, priorizan y estructuran los experimentos que permitirán validar hipótesis sobre las posibles mejoras del producto. En esta fase, se transforma el diagnóstico previo (As‑Is Summary) en acciones concretas, estableciendo objetivos claros, métricas de éxito, hipótesis a probar y condiciones de validación para cada experimento. Esto garantiza que las decisiones de diseño y desarrollo estén guiadas por evidencia, y que los recursos se enfoquen en resolver los puntos críticos que más impacto generan en la experiencia del usuario o el valor del negocio.

### 8.1.1. As-Is Summary

El As‑Is Summary en el proceso XDPD es un diagnóstico conciso del estado actual de la solución, que combina datos técnicos (como métricas de rendimiento y accesibilidad), información cualitativa procedente de usuarios piloto y una identificación clara de las principales fricciones en la experiencia y la funcionalidad. Este resumen actúa como línea base para comprender con precisión cómo funciona hoy la plataforma, qué barreras enfrentan los usuarios y qué deficiencias técnicas o de escala existen, de modo que cada experimento posterior se diseñe sobre una realidad consolidada y orientada a resolver los problemas más críticos.

La plataforma MoviGestión, en su fase inicial de desarrollo, integra un conjunto de módulos fundamentales para optimizar la administración de flotas de transporte: registro y edición detallada de vehículos; asignación, filtrado y visualización de envíos; seguimiento en tiempo real del estado de cada entrega; reporte estructurado de incidencias; y consulta histórica de todas las operaciones realizadas. Actualmente solo está en prueba interna, con la participación de seis usuarios piloto (tres gerentes empresariales y tres transportistas), cuyas entrevistas han aportado información valiosa sobre la claridad de la interfaz, funcionalidades demandadas y principales puntos de fricción en el flujo de trabajo.

**Problemas encontrados**

* **Rendimiento técnico insuficiente**

    - El Largest Contentful Paint (LCP) promedia 5,0 s en pantallas críticas (por ejemplo, el dashboard y la lista de envíos), lo que crea una percepción de lentitud y puede desincentivar la interacción continua. <br><br>
    
    - El First Contentful Paint (FCP) alcanza 2,5 s, por encima del rango recomendado de 1 – 1,5 s para brindar una experiencia percibida como ágil y receptiva.<br><br>
   
    - Accesibilidad promedio de 87/100 y SEO promedio de 75/100 en Lighthouse, lo que señala oportunidades de mejora en contraste, estructura semántica y metaetiquetado.<br><br>

* **Usabilidad insuficiente**

    - La ausencia de tutoriales interactivos y coach‑marks impide que los nuevos usuarios se familiaricen rápidamente con la interfaz y perciban un progreso inmediato durante la carga de datos.<br><br>
  
    - Falta de modo oscuro y esquemas de alto contraste que garanticen comodidad en entornos con poca luz y cumplan con WCAG AAA.<br><br>

* **Falta de posibles funcionalidades esenciales**

    - Falta un sistema de notificaciones multicanal (push, email y SMS) que los usuarios puedan configurar para recibir alertas sobre incidencias, asignaciones y cambios de estado en tiempo real.<br><br>
  
    - No se ha implementado un módulo de optimización de rutas dinámico, capaz de calcular trayectos óptimos según tráfico, disponibilidad de vehículos y ventanas horarias.<br><br>
  
    - La plataforma carece de herramientas para exportar datos y generar reportes descargables (PDF y Excel) con plantillas personalizables, lo que dificulta la elaboración de informes periódicos.<br><br>

* **Mantenimiento y escalabilidad**

    - No existe un sistema centralizado de logging o monitoreo de errores en tiempo real que detecte y alerte sobre fallos antes de que afecten a un mayor número de usuarios.<br><br>
  
    - La arquitectura actual, de carácter más monolítico, no está preparada para escalar horizontalmente, lo cual podría comprometer la estabilidad a medida que crezca la base de usuarios y el volumen de datos procesados.<br><br>

* **Falta de internacionalización y traducciones**

    - Toda la interfaz y los contenidos están únicamente en español: no hay soporte para formatos internacionales (fecha, moneda, zona horaria) ni traducciones disponibles, lo que limita la adopción por hablantes de otros idiomas y obstaculiza la expansión regional.<br><br>
  
**Objetivos de mejora**

1. **Optimización de rendimiento**

    - Reducir First Contentful Paint a < 1,5 s y Largest Contentful Paint a < 2 s en vistas clave (dashboard, lista de envíos) mediante mejoras en el rendering, división inteligente de espacios, cards y lists, y compresión avanzada de recursos.<br><br>

2. **Accesibilidad y personalización UI**
   
    - Introducir un modo oscuro y esquemas de alto contraste, cumpliendo con el nivel AAA de las WCAG.<br><br>
    
    - Ajustar tipografías, espaciados y tamaños de elemento para maximizar la legibilidad en todo tipo de dispositivos y entornos de iluminación.<br><br>

3. **Onboarding y soporte contextual**

    - Desarrollar tutoriales interactivos y coach‑marks que guíen al usuario en los flujos esenciales durante su primera sesión.<br><br>
    
    - Integrar un widget de ayuda contextual o chat en vivo para resolver dudas y reducir la dependencia de documentación externa.<br><br>

4. **Notificaciones multicanal configurables**

    - Desplegar alertas push, email y SMS para incidencias, confirmaciones de entrega y cambios de asignación.<br><br>
    
    - Permitir a cada usuario definir el canal preferido y la frecuencia de recepción de avisos, mejorando la relevancia de las notificaciones.<br><br>

5. **Optimización de rutas en tiempo real**

    - Añadir un motor de cálculo dinámico de rutas que considere tráfico en vivo, capacidad del vehículo y ventanas horarias, ofreciendo itinerarios óptimos y flexibles.<br><br>

6. **Exportación avanzada de datos**

    - Ofrecer generación y descarga de reportes en formatos PDF y Excel, con plantillas personalizables que incluyan métricas de rendimiento, entregas e incidencias.<br><br>
    
    - Proporcionar una interfaz para definir periodos y filtros, facilitando la obtención de informes periódicos.<br><br>

7. **Monitorización y escalado automático**

    - Implementar un sistema de registro centralizado de errores y métricas de rendimiento, con alertas en tiempo real.<br><br>
    
    - Migrar gradualmente a una arquitectura de contenedores o una arquitectura en la nube para soportar picos de carga y crecimiento continuo.<br><br>

8. **Internacionalización completa**
     
    - Añadir soporte para formatos internacionales (fechas, moneda, zonas horarias) y traducir toda la interfaz al inglés.<br><br>
    
    - Garantizar que la documentación, tutoriales y mensajes de error estén disponibles en más de un idioma.<br><br>

9. **Medición continua y feedback**

    - Instrumentar encuestas breves in‑app tras eventos clave (por ejemplo el cierre de una entrega por un transportista) para recopilar opiniones cualitativas.<br><br>
    
    - Definir, monitorizar y comunicar KPIs de adopción y satisfacción, como la tasa de retención, número de tareas completadas por sesión y NPS interno.

### 8.1.2. Raw Material: Assumptions, Knowledge Gaps, Ideas, Claims

**Assumptions:**

- **Rendimiento excepcional como diferenciador:**
Creemos que reducir el First Contentful Paint por debajo de 1,5 s y el Largest Contentful Paint por debajo de 2 s no solo aliviará la percepción de lentitud, sino que también aumentará la adopción diaria y la retención de usuarios en al menos un 15 %, alineándose con los estándares de las aplicaciones más competitivas. <br><br>

- **Control total de notificaciones:**
Asumimos que permitir a cada usuario configurar canales (push, email y SMS) y la frecuencia de las alertas incrementará drásticamente la velocidad de respuesta ante incidencias críticas, mejorando la coordinación entre gerentes y transportistas.<br><br>

- **Adaptabilidad de la interfaz:**
Creemos que ofrecer un modo claro/oscuro y esquemas de alto contraste (cumpliendo WCAG AAA) prolongará el tiempo de uso en entornos de iluminación adversa y reducirá la fatiga visual, incrementando la satisfacción del usuario.<br><br>

- **Optimización de rutas como ventaja competitiva:**
Suponemos que un motor de planificación de rutas dinámico, que integre datos de tráfico en tiempo real y capacidad de vehículo, puede reducir los kilómetros recorridos y el gasto de combustible entre un 10 % y un 20 %.<br><br>

- **Valor del reporting con documentos impresos:**
Consideramos que la capacidad de exportar datos en PDF y Excel con plantillas configurables ahorrará al menos un 40 % del tiempo dedicado a la elaboración de informes periódicos, liberando recursos para el análisis estratégico.<br><br>

- **Visibilidad proactiva de errores:**
Damos por hecho que implementar un sistema de logging y monitoreo en tiempo real reducirá significativamente el tiempo medio de resolución de incidencias y evitará que los problemas se propaguen, manteniendo la confianza del usuario.<br><br>

- **Internacionalización como motor de crecimiento:**
Asumimos que soportar formatos globales (fechas, monedas, zonas horarias) y traducir la interfaz al inglés permitirá captar nuevos mercados y ampliar la base de usuarios potenciales en un 20 % o más.<br><br>

- **Feedback continuo e iterativo**
Creemos que desplegar encuestas breves in‑app tras eventos críticos (por ejemplo, cierre de una entrega) generará insights cualitativos y cuantitativos que impulsen mejoras, elevando el NPS interno en al menos un 10 %.<br><br>

**Knowledge Gaps:**

- **Tolerancia a la latencia:**
  Desconocemos el punto de ruptura de la experiencia en el que los usuarios abandonan la plataforma, ya sea por un Largest Contentful Paint demasiado largo, por errores constantes u otros factores de alto impacto en la usabilidad y experiencia. <br><br>

- **Preferencias de notificación:** 
  No disponemos de datos sobre qué tipo de canal (push, email o SMS) prefieren los gerentes y transportistas para recibir distintos avisos, ni en qué circunstancias un medio resulta más efectivo que otro. Sabemos que todos son usados, pero no sabemos cual es el preferido o más usado.<br><br>

- ***Interés en internacionalización:**
  Carecemos de información cuantitativa sobre el apetito real por cambiar de idioma a inglés, así como sobre la importancia de soportar formatos de fecha, moneda y zona horaria en mercados clave.<br><br>

- **Formatos de reporte y filtros:**
    Carecemos de información sobre qué combinaciones de datos (fechas, transportistas, estados de envío) y qué tipos de plantillas (gráficos, tablas, resúmenes ejecutivos) resultan más útiles para cada perfil de usuario al generar informes periódicos.<br><br>

- **Canal de soporte preferido:**
   Falta información sobre si los usuarios prefieren un chat en vivo integrado, un widget de preguntas frecuentes o documentación contextual, y cómo esto influye en la resolución de dudas y en la satisfacción general.<br><br>

- **Comportamiento cross-device real:** 
    Carecemos de métricas segmentadas que muestren diferencias en patrones de uso entre móvil y escritorio, especialmente en entornos de red limitada, para priorizar optimizaciones responsivas.<br><br>

- **Curva de adopción y abandono:**
    No tenemos datos sobre en qué paso exacto del onboarding (registro, primer filtrado, primer reporte) los usuarios tienden a abandonar, ni sobre las razones cualitativas detrás de ese abandono.

**Ideas:**

- **Pruebas A/B de percepción de velocidad:** 
  Comparar dos versiones de las pantallas críticas de la aplicación con variaciones y ediciones distintas, esto para medir cómo varía la satisfacción del usuario y el tiempo hasta la primera interacción perceptible. <br><br>

- **Encuestas in‑app dirigidas y segmentadas:**
    Implementar formularios breves en contextos clave (por ejemplo, al cerrar una entrega o al visualizar un reporte) que pregunten a gerentes y transportistas sobre sus preferencias de notificación, uso de reportes y valor percibido de nuevas funciones.<br><br>

- **Prototipado rápido de modo oscuro y alto contraste:**
   Desarrollar un “theme switcher” mínimo capaz de alternar entre modo claro/oscuro y alto contraste, y organizar sesiones de prueba con usuarios piloto para recoger feedback sobre usabilidad, legibilidad y preferencia de esquema.<br><br>

- **Panel MVP (Producto Mínimo Viable) de exportación de datos:**
 Diseñar una interfaz sencilla donde los usuarios puedan seleccionar métricas, rangos de fechas y formatos (PDF/Excel) para descargar reportes, con capacidad de previsualizar la plantilla y validar la utilidad de los distintos layouts.<br><br>

- **Prototipo de onboarding guiado:**
   Desarrollar una capa de tutorial interactivo con coach‑marks y pasos secuenciales que acompañen al usuario en su primera sesión, midiendo la reducción de la tasa de abandono en cada paso del flujo de registro y configuración inicial.

**Claims:**

- **Percepción de rendimiento mejorada:** 
  Se sostiene que reducir el Largest Contentful Paint por debajo de 2 s no solo disminuirá la frustración inicial del usuario, sino que incrementará la satisfacción global y la retención de la plataforma en al menos un 15 %, acercando la experiencia a los estándares de aplicaciones de alto rendimiento. <br><br>

- **Respuesta más ágil ante incidencias:**
  Se postula que la implementación de notificaciones multicanal configurables (push, email y SMS) permitirá a gerentes y transportistas reaccionar un 30 % más rápido ante reportes críticos, mejorando la coordinación operacional y reduciendo el tiempo de interrupción de los flujos de trabajo.<br><br>

- **Reducción de costes logísticos:**
    Se afirma que incorporar un motor de optimización de rutas dinámico, basado en datos de tráfico en tiempo real y capacidades de vehículo, puede reducir el kilometraje y el consumo de combustible en un 10 %–20 %, traduciéndose en ahorros significativos para las empresas.<br><br>

- **Mayor adopción en entornos oscuros:**
  Se plantea que la introducción de un tema oscuro y esquemas de alto contraste elevará el uso diario de la aplicación en condiciones de baja iluminación en un 25 %, al mejorar la legibilidad y reducir la fatiga visual durante jornadas prolongadas.<br><br>

- **Eficiencia en la elaboración de informes:**
  Se asume que la capacidad de exportar datos en formatos PDF y Excel con plantillas personalizables reducirá hasta en un 40 % el tiempo dedicado a generar reportes periódicos, liberando recursos para el análisis estratégico y la toma de decisiones.<br><br>

- **Incremento del feedback accionable:**
  Se sostiene que la implementación de encuestas breves in‑app tras eventos críticos (por ejemplo, la finalización de una entrega) generará un aumento del 20 % en la tasa de respuesta de usuarios, proporcionando datos cualitativos y cuantitativos que orienten mejoras continuas en la plataforma.
  
### 8.1.3. Experiment-Ready Questions

En esta sección presentamos las Experiment‑Ready Questions, un conjunto de preguntas concretas y priorizadas que guían la validación de nuestras principales hipótesis de mejora. Cada pregunta está diseñada para enfocarse en un aspecto crítico identificado en el As‑Is y el Raw Material, desde la percepción de rendimiento hasta la adopción de nuevas funcionalidades, evaluando de manera cuantitativa el impacto, el riesgo de implementación y el grado de interés de los usuarios. Al responderlas mediante pequeños experimentos controlados, podremos tomar decisiones fundamentadas, optimizar recursos y avanzar en ciclos iterativos que impulsen la evolución de MoviGestión de forma ágil y eficiente.

| Question	| Confidence |	Risk |	Impact	 |Interest	| Total Score |
|----------|------------------|-------------|--------|---|-------|
¿Mejorará la percepción de velocidad el uso de skeleton screens en pantallas críticas frente al loader clásico?	| 8 – Técnica probada en la industria para reducir la percepción de espera. |	2 – Riesgo bajo, es una modificación visual ligera.	|6 – Puede aumentar el engagement y reducir el abandono inicial.	|5 – Interés moderado, los usuarios notan mejoras sutiles de UX.	|21|
|¿Reducirá el tiempo de respuesta a incidencias la implementación de notificaciones multicanal configurables?	|8 – Buena base en otros sistemas de alertas multicanal.	|3 – Riesgo medio-bajo, implica configuración de infraestructura de mensajería.|8 – Mejora significativa de la coordinación operativa y la resolución de problemas.	|7 – Alta relevancia para gerentes y transportistas que dependen de alertas inmediatas.	|26|
|¿Disminuirán los costes logísticos y kilómetros recorridos la optimización dinámica de rutas en tiempo real?|	6 – Supuesto fundamentado en estudios de tráfico y planificación logística.	|6 – Riesgo moderado-alto, el desarrollo es complejo y dependiente de datos externos.	|9 – Potencial muy alto de ahorro de combustible y mejora de eficiencia operativa.	|8 – Gran interés, ya que impacta directamente en costes de la operación.|	29|
|¿Ahorrará tiempo administrativo la función de exportación de datos a PDF/Excel con plantillas configurables?	|7 – Basado en experiencias de herramientas BI (Business Intelligence) y ERP (Recursos empresariales).	|3 – Riesgo bajo, funcionalidad relativamente sencilla de implementar.	|8 – Reduce carga de trabajo manual y agiliza la generación de informes periódicos.|	6 – Interés moderado, especialmente en perfiles gerenciales y administrativos.	|24|
|¿Reducirá la tasa de abandono en el onboarding la introducción de tutoriales interactivos y coach‑marks?	|8 – Alta confianza, técnicas de onboarding interactivo ampliamente adoptadas.|	5 – Riesgo medio, requiere diseño cuidadoso de flujos y contenido.|	8 – Impacto directo en la adopción y en la curva de aprendizaje de nuevos usuarios.|	7 – Fuerte interés, los usuarios valoran la guía en sus primeros pasos.	|28|
|¿Aumentará el uso en entornos de baja iluminación la implementación de un modo oscuro y alto contraste?|	8 – Funcionalidad popular y de bajo esfuerzo técnico.	|2 – Riesgo bajo, es un cambio de estilos y temas.	|6 – Mejora la comodidad visual, aunque no es crítica para todos los usuarios.|	6 – Interés moderado, especialmente en usuarios con largos periodos de uso nocturno.	|22|
|¿Incrementará la base de usuarios activos la internacionalización al inglés?	|5 – Depende de la demanda real en mercados extranjeros.	|5 – Riesgo medio, implica proceso de traducción y adaptación cultural.|	8 – Puede abrir nuevas oportunidades de mercado y crecimiento de la audiencia.	|6 – Interés variable según perfil de usuario y región.	|24|
  
### 8.1.4. Question Backlog
  
### 8.1.5. Experiment Cards
  
## 8.2. Experiment Design

### 8.2.1. Hypotheses
  
### 8.2.2. Measures
  
### 8.2.3. Conditions
  
### 8.2.4. Scale Calculations and Decisions
  
### 8.2.5. Methods Selection
  
### 8.2.6. Data Analytics: Goals, KPIs and Metrics Selection
  
### 8.2.7. Web and Mobile Tracking Plan
