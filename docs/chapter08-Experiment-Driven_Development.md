# 8.1. Experiment Planning

El Experiment Planning dentro del proceso XDPD es la etapa en la que se definen, priorizan y estructuran los experimentos que permitirán validar hipótesis sobre las posibles mejoras del producto. En esta fase, se transforma el diagnóstico previo (As‑Is Summary) en acciones concretas, estableciendo objetivos claros, métricas de éxito, hipótesis a probar y condiciones de validación para cada experimento. Esto garantiza que las decisiones de diseño y desarrollo estén guiadas por evidencia, y que los recursos se enfoquen en resolver los puntos críticos que más impacto generan en la experiencia del usuario o el valor del negocio.

## 8.1.1. As-Is Summary

El As‑Is Summary en el proceso XDPD es un diagnóstico conciso del estado actual de la solución, que combina datos técnicos (como métricas de rendimiento y accesibilidad), información cualitativa procedente de usuarios piloto y una identificación clara de las principales fricciones en la experiencia y la funcionalidad. Este resumen actúa como línea base para comprender con precisión cómo funciona hoy la plataforma, qué barreras enfrentan los usuarios y qué deficiencias técnicas o de escala existen, de modo que cada experimento posterior se diseñe sobre una realidad consolidada y orientada a resolver los problemas más críticos.

La plataforma MoviGestión, en su fase inicial de desarrollo, integra un conjunto de módulos fundamentales para optimizar la administración de flotas de transporte: registro y edición detallada de vehículos; asignación, filtrado y visualización de envíos; seguimiento en tiempo real del estado de cada entrega; reporte estructurado de incidencias; y consulta histórica de todas las operaciones realizadas. Actualmente solo está en prueba interna, con la participación de seis usuarios piloto (tres gerentes empresariales y tres transportistas), cuyas entrevistas han aportado información valiosa sobre la claridad de la interfaz, funcionalidades demandadas y principales puntos de fricción en el flujo de trabajo.

**Problemas encontrados**

* **Rendimiento técnico insuficiente**

    - El Largest Contentful Paint (LCP) promedia 5,0 s en pantallas críticas (por ejemplo, el dashboard y la lista de envíos), lo que crea una percepción de lentitud y puede desincentivar la interacción continua.
    
    - El First Contentful Paint (FCP) alcanza 2,5 s, por encima del rango recomendado de 1 – 1,5 s para brindar una experiencia percibida como ágil y receptiva.
   
    - Accesibilidad promedio de 87/100 y SEO promedio de 75/100 en Lighthouse, lo que señala oportunidades de mejora en contraste, estructura semántica y metaetiquetado.

* **Usabilidad insuficiente**

    - La ausencia de tutoriales interactivos y coach‑marks impide que los nuevos usuarios se familiaricen rápidamente con la interfaz y perciban un progreso inmediato durante la carga de datos.
  
    - Falta de modo oscuro y esquemas de alto contraste que garanticen comodidad en entornos con poca luz y cumplan con WCAG AAA.

* **Falta de posibles funcionalidades esenciales**

    - Falta un sistema de notificaciones multicanal (push, email y SMS) que los usuarios puedan configurar para recibir alertas sobre incidencias, asignaciones y cambios de estado en tiempo real.
  
    - No se ha implementado un módulo de optimización de rutas dinámico, capaz de calcular trayectos óptimos según tráfico, disponibilidad de vehículos y ventanas horarias.
  
    - La plataforma carece de herramientas para exportar datos y generar reportes descargables (PDF y Excel) con plantillas personalizables, lo que dificulta la elaboración de informes periódicos.

* **Mantenimiento y escalabilidad**

    - No existe un sistema centralizado de logging o monitoreo de errores en tiempo real que detecte y alerte sobre fallos antes de que afecten a un mayor número de usuarios.
  
    - La arquitectura actual, de carácter más monolítico, no está preparada para escalar horizontalmente, lo cual podría comprometer la estabilidad a medida que crezca la base de usuarios y el volumen de datos procesados.

* **Falta de internacionalización y traducciones**

    - Toda la interfaz y los contenidos están únicamente en español: no hay soporte para formatos internacionales (fecha, moneda, zona horaria) ni traducciones disponibles, lo que limita la adopción por hablantes de otros idiomas y obstaculiza la expansión regional.
  
**Objetivos de mejora**

1. **Optimización de rendimiento**

    - Reducir First Contentful Paint a < 1,5 s y Largest Contentful Paint a < 2 s en vistas clave (dashboard, lista de envíos) mediante mejoras en el rendering, división inteligente de espacios, cards y lists, y compresión avanzada de recursos.

2. **Accesibilidad y personalización UI**
   
    - Introducir un modo oscuro y esquemas de alto contraste, cumpliendo con el nivel AAA de las WCAG.
    
    - Ajustar tipografías, espaciados y tamaños de elemento para maximizar la legibilidad en todo tipo de dispositivos y entornos de iluminación.

3. **Onboarding y soporte contextual**

    - Desarrollar tutoriales interactivos y coach‑marks que guíen al usuario en los flujos esenciales durante su primera sesión.
    
    - Integrar un widget de ayuda contextual o chat en vivo para resolver dudas y reducir la dependencia de documentación externa.

4. **Notificaciones multicanal configurables**

    - Desplegar alertas push, email y SMS para incidencias, confirmaciones de entrega y cambios de asignación.
    
    - Permitir a cada usuario definir el canal preferido y la frecuencia de recepción de avisos, mejorando la relevancia de las notificaciones.

5. **Optimización de rutas en tiempo real**

    - Añadir un motor de cálculo dinámico de rutas que considere tráfico en vivo, capacidad del vehículo y ventanas horarias, ofreciendo itinerarios óptimos y flexibles.

6. **Exportación avanzada de datos**

    - Ofrecer generación y descarga de reportes en formatos PDF y Excel, con plantillas personalizables que incluyan métricas de rendimiento, entregas e incidencias.
    
    - Proporcionar una interfaz para definir periodos y filtros, facilitando la obtención de informes periódicos.

7. **Monitorización y escalado automático**

    - Implementar un sistema de registro centralizado de errores y métricas de rendimiento, con alertas en tiempo real.
    
    - Migrar gradualmente a una arquitectura de contenedores o una arquitectura en la nube para soportar picos de carga y crecimiento continuo.

8. **Internacionalización completa**
     
    - Añadir soporte para formatos internacionales (fechas, moneda, zonas horarias) y traducir toda la interfaz al inglés.
    
    - Garantizar que la documentación, tutoriales y mensajes de error estén disponibles en más de un idioma.

9. **Medición continua y feedback**

    - Instrumentar encuestas breves in‑app tras eventos clave (por ejemplo el cierre de una entrega por un transportista) para recopilar opiniones cualitativas.
    
    - Definir, monitorizar y comunicar KPIs de adopción y satisfacción, como la tasa de retención, número de tareas completadas por sesión y NPS interno.

## 8.1.2. Raw Material: Assumptions, Knowledge Gaps, Ideas, Claims
  
## 8.1.3. Experiment-Ready Questions
  
## 8.1.4. Question Backlog
  
## 8.1.5. Experiment Cards
  
# 8.2. Experiment Design

## 8.2.1. Hypotheses
  
## 8.2.2. Measures
  
## 8.2.3. Conditions
  
## 8.2.4. Scale Calculations and Decisions
  
## 8.2.5. Methods Selection
  
## 8.2.6. Data Analytics: Goals, KPIs and Metrics Selection
  
## 8.2.7. Web and Mobile Tracking Plan
