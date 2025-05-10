# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping.

_Modelo de To-Be Scenario Mapping del primer User Persona._
<img src="/assets/chapter03/to-be-1.png">
_Modelo de To-Be Scenario Mapping del segundo User Persona._
<img src="/assets/chapter03/to-be-2.png">

## 3.2. User Stories.

En esta sección, presentaremos un análisis detallado de cada una de las historias de usuario asignadas a lo largo de todo el ciclo de vida del proyecto. El objetivo primordial es asegurar la completa satisfacción de nuestros segmentos de mercado mediante la comprensión y la satisfacción de sus necesidades y expectativas. Para ello, vamos a especificar los requisitos definidos, así como el conjunto de User Stories y Epics que hemos identificado como fundamentales para el éxito del proyecto. Es importante destacar que cada User Story estará acompañada de sus criterios de aceptación, lo que garantizará una comprensión clara de lo que se espera lograr.

Para comenzar este proceso de presentación, vamos a comenzar con una comprensión clara de lo que representan los Epics en nuestro contexto. Los Epics actúan como contenedores de alto nivel que encapsulan conjuntos de funcionalidades o características más amplias del producto. Son los pilares sobre los cuales se construirá la experiencia del usuario y se alcanzarán los objetivos del proyecto según sus métricas ya establecidas de forma ordenada y controlada (Patton et al., 2014).

Por lo tanto, presentaremos primero nuestro modelo de Epics, que servirá como guía y marco de referencia para comprender la naturaleza y el alcance de las historias de usuario que se presentarán a continuación. Este enfoque asegurará que se tenga una visión clara y completa de los diferentes tipos de historias de usuario, así como de sus divisiones y definiciones correspondientes, facilitando así una mejor comprensión y evaluación del proyecto en su conjunto.

_Tabla de épicas establecidas para las historias de usuarios._

<table border="1" style="text-align: left;">
	<tbody>
		<tr>
			<td colspan="1">Epic ID</td>
            <td colspan="1">Título</td>
            <td colspan="1">Descripción</td>
		</tr>
		<tr>
            <td colspan="1">EP001</td>
            <td colspan="1">Visualización de estadísticas de transportistas </td>
            <td colspan="1">
            <strong>Como</strong>  gerente quiero tener un registro de actividades hechas por todos los transportistas para tener un control y seguimiento del rendimiento general de mis empleados. 
        </td>
		</tr>
        <tr>
            <td colspan="1">EP002</td>
            <td colspan="1">Visualización de estadísticas propias</td>
            <td colspan="1">
            <strong>Como</strong>  transportista quiero ver las acciones hechas durante mi trabajo para tener un registro de las actividades hechas en mi labor.
            </td>
		</tr>
        <tr>
            <td colspan="1">EP003</td>
            <td colspan="1">Gestión de envíos</td>
            <td colspan="1">
            <strong>Como</strong> gerente quiero registrar envíos a mis transportistas y tener un control de ello a través del tiempo para mejorar el rendimiento de los envíos de mi empresa.
            </td>
		</tr>
        <tr>
            <td colspan="1">EP004</td>
            <td colspan="1">Gestión de vehículos </td>
            <td colspan="1">
            <strong>Como</strong> gerente quiero un registro de mis vehículos, así como quien está a cargo de ellos para tener un seguimiento de su estado a través del tiempo  
            </td>
		</tr>
        <tr>
            <td colspan="1">EP005</td>
            <td colspan="1">Reporte de problemas</td>
            <td colspan="1">
            <strong>Como</strong>  transportista quiero reportar problemas que puedan suceder en mi labor para que se tomen las medidas necesarias.
            </td>
		</tr>
        <tr>
            <td colspan="1">EP006</td>
            <td colspan="1">Gestión de datos personales</td>
            <td colspan="1">
            <strong>Como</strong> usuario quiero manejar mi información personal para tenerla actualizada en todo momento.
            </td>
		</tr>
	</tbody>
</table>

_Tabla de las historias de usuarios establecidas para todo el proyecto de MoviGestion_

<table  border="1" style="text-align: left;">
  <thead>
    <tr>
      <th>User Story ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de Aceptación</th>
      <th>Epic Id</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td >US01</td>
      <td >Visualización de paquetes entregados por un transportista</td>
      <td >Como gerente, quiero visualizar el número y detalle de paquetes entregados por un transportista en un período específico para medir su rendimiento en términos de productividad y eficiencia.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Filtrado y Listado de Entregas</b> 
          Dado que el gerente ha iniciado sesión en el sistema, cuando selecciona un  transportista        específico y un rango de fechas en la sección de    visualización de entregas, entonces el     sistema muestra una lista de todos los  paquetes entregados por ese transportista durante     el período seleccionado,   incluyendo el ID del paquete y la fecha/hora de entrega.
          </li>
          <li> 
          <b>Criterio 2: Conteo Total de Entregas</b> 
          Dado que el gerente ha aplicado un filtro de transportista y rango de fechas en la  sección de visualización de entregas, entonces el sistema muestra el número total    de paquetes entregados por el transportista seleccionado en el período     especificado en un lugar visible de la interfaz
          </li>
        </u>
      </td>
      <td >EP01</td>
    </tr>
    <tr>
    </tr>
    <tr>
      <td >US02</td>
      <td >Visualización de reportes de un transportista</td>
      <td >Como gerente, quiero ver los tipos y detalles de los reportes hechos por mis transportistas (ej. incidencias, problemas con paquetes) filtrados por período y transportista para tomar decisiones estratégicas en los próximos envíos basadas en problemas recurrentes o áreas de mejora.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Filtrado de Reportes</b> 
          Dado que el gerente ha iniciado sesión en el sistema, cuando filtra los reportes por un transportista específico y un rango de fechas, y opcionalmente por un tipo de reporte, entonces el sistema muestra una lista de los reportes que coinciden con los criterios de filtro.
          </li>
          <li> 
          <b>Criterio 2: Detalles del Reporte en Listado</b> 
          Dado que se muestra una lista de reportes, entonces para cada reporte en la lista, el sistema muestra la fecha y hora del reporte, el tipo, una breve descripción y el nombre del transportista que lo generó.
          </li>
        </u>
      </td>
      <td >EP01</td>
    </tr>
    <tr>
      <td >US03</td>
      <td >Visualización de envíos asignados a un transportista</td>
      <td >Como gerente, quiero ver el listado de envíos asignados a un transportista, incluyendo fechas de entrega, estado actual y detalles del envío, para poder medir el rendimiento de mis empleados en relación con la carga de trabajo y el cumplimiento de plazos.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Visualización de envíos asignados a un transportista</b> 
          Dado que el gerente ha iniciado sesión en el sistema, cuando selecciona un transportista en la sección de visualización de envíos asignados, entonces el sistema muestra una lista de todos los envíos actualmente asignados a ese transportista, indicando el ID del envío, la fecha de entrega estimada y el estado actual.
          </li>
          <li> 
          <b>Criterio 2: Ver Detalles del Envío</b> 
          Dado que se muestra un envío en la lista, cuando el gerente selecciona o expande la información de ese envío, entonces el sistema muestra detalles adicionales como las direcciones de recogida y entrega.
          </li>
        </u>
      </td>
      <td >EP01</td>
    </tr>
    <tr>
      <td >US04</td>
      <td >Visualización de envíos asignados</td>
      <td >Como transportista, quiero poder ver los envíos que me han sido asignados, incluyendo direcciones de recogida y entrega, horarios estimados, contenido e instrucciones especiales, para poder organizar mejor el orden de mis tareas y optimizar mi ruta.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Listado de Envíos para Transportista</b> 
          Dado que el transportista ha iniciado sesión en la aplicación, cuando accede a la sección de envíos asignados, entonces el sistema muestra una lista de todos los envíos que le han sido asignados. Cada entrada muestra las direcciones de recogida y entrega, la hora estimada de entrega y una breve descripción del contenido.
          </li>
          <li> 
          <b>Criterio 2: Ver Instrucciones Especiales </b> 
          Dado que el transportista selecciona un envío de la lista, entonces el sistema muestra instrucciones especiales detalladas (si las hay) para ese envío.
          </li>
        </u>
      </td>
      <td >EP02</td>
    </tr>
    <tr>
      <td >US05</td>
      <td >Visualización de paquetes entregados</td>
      <td >Como transportista, quiero visualizar la lista de paquetes que he marcado como entregados, incluyendo la hora y la confirmación de entrega (si aplica) para tener un comprobante de trabajo realizado y poder resolver cualquier duda o reclamación.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Listado de Paquetes Entregados por Transportista</b> 
          Dado que el transportista ha iniciado sesión en la aplicación, cuando accede a la sección de paquetes entregados, entonces el sistema muestra una lista de los paquetes que ha marcado como entregados. Cada entrada muestra el ID del paquete y la hora en que se marcó como entregado.
          </li>
          <li> 
          <b>Criterio 2: Ver Confirmación de Entrega </b> 
          Dado que se requiere confirmación de entrega para un paquete, entonces esta información (ej. firma o fotografía) es visible para el transportista junto con el registro de entrega
          </li>
        </u>
      </td>
      <td >EP02</td>
    </tr>
    <tr>
      <td >US06</td>
      <td >Visualización de reportes realizados</td>
      <td >Como transportista, quiero visualizar los reportes que hice en mi labor, incluyendo la fecha, hora, tipo de reporte y descripción del problema, para tener un historial de incidencias en mi trabajo y poder referirme a ellos si es necesario.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Historial de Reportes del Transportista</b> 
          Dado que el transportista ha iniciado sesión en la aplicación, cuando accede a la sección de reportes realizados, entonces el sistema muestra un historial de todos los reportes que ha generado. Cada entrada muestra la fecha y hora del reporte, el tipo de reporte y una breve descripción del problema.
          </li>
          <li> 
          <b>Criterio 2: Ver Instrucciones Especiales  </b> 
          Dado que el transportista selecciona un reporte de la lista, entonces el sistema muestra la descripción completa del problema que reportó
          </li>
        </u>
      </td>
      <td >EP02</td>
    </tr>
    <tr>
      <td >US07</td>
      <td >Asignación de envíos</td>
      <td >Como gerente, quiero poder asignar envíos a mis transportistas seleccionando de una lista de envíos pendientes y transportistas disponibles, considerando la capacidad del vehículo y la ubicación, para distribuir eficientemente los envíos y optimizar los tiempos de entrega.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Asignación Exitosa de Envío</b> 
          Dado que el gerente está en la sección de asignación de envíos, cuando selecciona uno o varios envíos pendientes y un transportista disponible, entonces el sistema permite asignar los envíos al transportista.
          </li>
          <li> 
          <b>Criterio 2: Validación de Capacidad en Asignación </b> 
          Dado que la información de capacidad del transportista está implementada, cuando el gerente intenta asignar un envío, entonces el sistema valida si el transportista tiene capacidad disponible y muestra un mensaje de confirmación de la asignación exitosa o un error si no hay capacidad.
          </li>
        </u>
      </td>
      <td >EP03</td>
    </tr>
    <tr>
      <td >US08</td>
      <td >Visualización de historial de envíos</td>
      <td >Como gerente, quiero ver el historial de envíos realizados, incluyendo el estado final (exitoso, fallido, cancelado), fechas, transportistas asignados y motivos de fallo (si aplica) para saber cuántos de estos fueron exitosos y analizar las causas de los envíos no exitosos para mejorar la eficiencia futura.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Filtrado del Historial de Envíos</b> 
          Dado que el gerente ha iniciado sesión en el sistema, cuando aplica filtros por un rango de fechas y/o por el estado final en la sección de historial de envíos, entonces el sistema muestra una lista de envíos que coinciden con los criterios de filtro.
          </li>
          <li> 
          <b>Criterio 2: Detalles del Envío en el Historial </b> 
          Dado que se muestra un envío en el historial, entonces el sistema muestra el estado final, el transportista asignado y el motivo del fallo si el envío no fue exitoso.
          </li>
        </u>
      </td>
      <td >EP03</td>
    </tr>
    <tr>
      <td >US09</td>
      <td >Asignación de flotas</td>
      <td >Como gerente, quiero asignar flotas (especificando un vehículo o un grupo de vehículos) a mis transportistas para un período determinado o para una ruta específica, considerando la capacidad y el tipo de carga, para que puedan realizar los encargos con el vehículo adecuado.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Asignación de Flota a Transportista</b> 
          Dado que el gerente está en la sección de asignación de flotas, cuando selecciona un transportista y uno o varios vehículos de la lista de flotas disponibles, y opcionalmente especifica un período o ruta, entonces el sistema permite asignar las flotas al transportista.
          </li>
          <li> 
          <b>Criterio 2: Confirmación de Asignación de Flota </b> 
          Dado que la asignación de flota se ha realizado, entonces el sistema confirma la asignación y la registra en el sistema.
          </li>
        </u>
      </td>
      <td >EP04</td>
    </tr>
    <tr>
      <td >US10</td>
      <td >Gestión de inventario de flotas</td>
      <td >Como gerente, quiero añadir nuevas flotas (registrando detalles como tipo, capacidad, placa, estado) a mi negocio para tener un control activo de mis flotas y asegurar la disponibilidad de vehículos para las operaciones.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Adición de Nueva Flota </b> 
          Dado que el gerente está en la sección de gestión de flotas, cuando ingresa los detalles de una nueva flota y guarda, entonces la nueva flota aparece en la lista de flotas disponibles.
          </li>
          <li> 
          <b>Criterio 2: Edición de Detalles de Flota </b> 
          Dado que el gerente selecciona una flota existente en la sección de gestión de flotas, cuando edita su información y guarda los cambios, entonces los cambios se guardan correctamente en el sistema.
          </li>
        </u>
      </td>
      <td >EP04</td>
    </tr>
     <tr>
      <td >US11</td>
      <td >Reporte de infracciones vehiculares</td>
      <td >Como transportista, quiero poder reportar infracciones vehiculares que ocurran durante mis viajes, detallando la ubicación, tipo de infracción y si es posible, adjuntar evidencia, para que el gerente pueda tomar las medidas del caso y garantizar la seguridad y el cumplimiento normativo.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: </b> 
          Dado que el transportista está en la sección de reporte de infracciones, cuando completa el formulario con la ubicación, tipo de infracción y adjunta evidencia (opcional), entonces al enviar el reporte, el sistema guarda la información
          </li>
          <li> 
          <b>Criterio 2: Confirmación de Reporte de Infracción </b> 
          Dado que el reporte se ha enviado exitosamente, entonces el sistema muestra un mensaje de confirmación al transportista.
          </li>
        </u>
      </td>
      <td >EP05</td>
    </tr>
    </tr>
     <tr>
      <td >US12</td>
      <td >Reporte de accidentes en la carretera</td>
      <td >Como transportista, quiero poder reportar accidentes en la carretera que ocurran durante mis viajes, detallando la ubicación, gravedad, si hay heridos y cualquier otra información relevante, para que el gerente pueda organizar las futuras rutas evitando zonas peligrosas o tomar las acciones necesarias de soporte.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Envío de Reporte de Accidente </b> 
          Dado que el transportista está en la sección de reporte de accidentes, cuando completa el formulario con la ubicación, gravedad, información sobre heridos y otros detalles relevantes, entonces al enviar el reporte, el sistema guarda la información.
          </li>
          <li> 
          <b>Criterio 2: Confirmación de Reporte de Accidente </b> 
          Dado que el reporte se ha enviado exitosamente, entonces el sistema muestra un mensaje de confirmación al transportista.
          </li>
        </u>
      </td>
      <td >EP05</td>
    </tr>
    </tr>
     <tr>
      <td >US13</td>
      <td >Reporte de problemas con el paquete</td>
      <td >Como transportista, quiero poder reportar problemas con los paquetes que transporto durante mis viajes, describiendo el problema (daño, faltante, etc.) y el número de paquete, para que el gerente pueda reportarlo al cliente y tomar las medidas correctivas.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Envío de Reporte de Problema de Paquete </b> 
          Dado que el transportista está en la sección de reporte de problemas con paquetes, cuando completa el formulario con la descripción del problema y el número de paquete, entonces al enviar el reporte, el sistema guarda la información.
          </li>
          <li> 
          <b>Criterio 2: Confirmación de Reporte de Problema de Paquete  </b> 
          Dado que el reporte se ha enviado exitosamente, entonces el sistema muestra un mensaje de confirmación al transportista.
          </li>
        </u>
      </td>
      <td >EP05</td>
    </tr>
    </tr>
     <tr>
      <td >US14</td>
      <td >Reporte de problemas técnicos</td>
      <td >Como transportista, quiero poder reportar problemas técnicos que surjan durante mis viajes con el vehículo o la aplicación (ej. fallo del motor, error de navegación), detallando el problema, para que el gerente pueda resolverlo lo antes posible y minimizar el impacto en las entregas.</td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Envío de Reporte de Problema Técnico </b> 
          Dado que el transportista está en la sección de reporte de problemas técnicos, cuando completa el formulario con la descripción del problema con el vehículo o la aplicación, entonces al enviar el reporte, el sistema guarda la información.
          </li>
          <li> 
          <b>Criterio 2: Confirmación de Reporte de Problema Técnico  </b> 
          Dado que el reporte se ha enviado exitosamente, entonces el sistema muestra un mensaje de confirmación al transportista.
          </li>
        </u>
      </td>
      <td >EP05</td>
    </tr>
    </tr>
     <tr>
      <td >US15</td>
      <td >Gestión de Perfil de Gerente</td>
      <td >Como gerente, quiero visualizar y editar mi información personal (como nombre, correo electrónico, número de teléfono) para </td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Visualización de Perfil de Gerente </b> 
          Dado que el gerente ha iniciado sesión en el sistema, cuando accede a la sección de "Mi Perfil", entonces el sistema muestra sus datos personales (nombre, correo electrónico, teléfono).
          </li>
          <li> 
          <b>Criterio 2: Edición y Guardado de Perfil de Gerente  </b> 
          Dado que el gerente edita sus datos personales y guarda los cambios, entonces los cambios se guardan y se reflejan correctamente en el sistema.
          </li>
        </u>
      </td>
      <td >EP06</td>
    </tr>
    </tr>
     <tr>
      <td >US16</td>
      <td >Gestión de Perfil de Transportista</td>
      <td >Como transportista, quiero visualizar y editar mi información personal (como nombre, correo electrónico, número de teléfono, información de contacto de emergencia) para asegurarme de que mis datos estén correctos y actualizados en el sistema. </td>
      <td>
        <ul> 
          <li> 
          <b>Criterio 1: Visualización de Perfil de Transportista </b> 
          Dado que el transportista ha iniciado sesión en la aplicación, cuando accede a la sección de "Mi Perfil", entonces el sistema muestra sus datos personales (nombre, correo electrónico, teléfono, contacto de emergencia).
          </li>
          <li> 
          <b>Criterio 2: Edición y Guardado de Perfil de Transportista  </b> 
          Dado que el transportista edita sus datos personales y guarda los cambios, entonces los cambios se guardan y se reflejan correctamente en el sistema.
          </li>
        </u>
      </td>
      <td >EP06</td>
    </tr>

  </tbody>
</table>

## 3.3. Impact Mapping.

Impact Mapping es una herramienta poderosa que nos ayudará a visualizar y planificar cómo nuestro proyecto puede generar un impacto significativo en nuestros usuarios y en nuestro objetivo final. Nos permitirá identificar claramente los resultados deseados, los comportamientos esperados de nuestros usuarios y las acciones necesarias para alcanzar esos objetivos. Al utilizar Impact Mapping, podremos alinear mejor nuestras actividades con nuestros objetivos, tomar decisiones más informadas y maximizar el impacto de nuestro proyecto.

_Impact Mapping de los dos user persona del proyecto._

---

- **Modelo de Impact Mapping del primer User Persona** <br><br>
  ![ImpactMapping_1](/assets/chapter03/impact-map-1.jpeg) <br><br>
  ![ImpactMapping_2](/assets/chapter03/impact-map-2.jpeg) <br><br>
  ![ImpactMapping_3](/assets/chapter03/impact-map-3.jpeg) <br><br>

- **Modelo de Impact Mapping del segundo User Persona** <br><br>
  ![ImpactMapping_4](/assets/chapter03/impact-map-4.jpeg) <br><br>
  ![ImpactMapping_5](/assets/chapter03/impact-map-5.jpeg) <br><br>
  ![ImpactMapping_6](/assets/chapter03/impact-map-6.jpeg) <br><br>

## 3.4. Product Backlog.

- En esta sección del proyecto vamos a esquematizar y completar el Product Backlog, un elemento fundamental en la gestión ágil de proyectos de desarrollo de software. El Product Backlog actúa como una lista dinámica y priorizada de todas las funcionalidades, mejoras y requisitos que deben ser desarrollados para el producto. Su orden se basa en la priorización del valor para el negocio y es clave para guiar el trabajo del equipo de desarrollo a lo largo del proyecto.
- El Product Backlog se compone de historias de usuario, tareas técnicas y otras actividades relacionadas con el desarrollo del producto. Este orden sigue una lógica clara, colocando en primer lugar aquellas historias relacionadas con la experiencia del usuario en la Landing Page, seguidas de las funcionalidades esenciales de la aplicación web, y finalmente, las historias técnicas necesarias para el desarrollo del sistema (Patton et al., 2014).
- Como parte de nuestra iniciativa para esta sección, hemos integrado un modelo de guía de tareas y actividades señaladas para cada integrante dentro del Product Backlog mediante el uso de la aplicación Trello. Los lectores pueden acceder al planeamiento del Product Backlog completo a través del siguiente enlace:

- https://trello.com/invite/b/6803cdc30d35ce3bf507df7b/ATTI5b41d5e00ebe932f0b2c0940d5beeb9f6ECBFED4/fundamentosdearquitectura-lapicitosteam

<table border="1" cellspacing="0" cellpadding="5">
  <thead>
    <tr>
      <th>#Orden</th>
      <th>User Story ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Story Points (1/2/3/5/8)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>US07</td>
      <td>Asignación de envío</td>
      <td>Como gerente, quiero poder asignar envíos a mis transportistas seleccionando de una lista de envíos pendientes y transportistas disponibles, considerando la capacidad del vehículo y la ubicación, para distribuir eficientemente los envíos y optimizar los tiempos de entrega.</td>
      <td>8</td>
    </tr>
    <tr>
      <td>2</td>
      <td>US09</td>
      <td>Asignación de flota</td>
      <td>Como gerente, quiero asignar flotas (especificando un vehículo o un grupo de vehículos) a mis transportistas para un período determinado o para una ruta específica, considerando la capacidad y el tipo de carga, para que puedan realizar los encargos con el vehículo adecuado.</td>
      <td>8</td>
    </tr>
    <tr>
      <td>3</td>
      <td>US10</td>
      <td>Gestión de inventario de flotas</td>
      <td>Como gerente, quiero añadir nuevas flotas (registrando detalles como tipo, capacidad, placa, estado) a mi negocio para tener un control activo de mis flotas y asegurar la disponibilidad de vehículos para las operaciones.</td>
      <td>8</td>
    </tr>
    <tr>
      <td>4</td>
      <td>US08</td>
      <td>Visualización de historial de envíos</td>
      <td>Como gerente, quiero ver el historial de envíos realizados, incluyendo el estado final (exitoso, fallido, cancelado), fechas, transportistas asignados y motivos de fallo (si aplica) para saber cuántos de estos fueron exitosos y analizar las causas de los envíos no exitosos para mejorar la eficiencia futura.</td>
      <td>8</td>
    </tr>
    <tr>
      <td>5</td>
      <td>US02</td>
      <td>Visualización de reportes de un transportista</td>
      <td>Como gerente, quiero ver los tipos y detalles de los reportes hechos por mis transportistas (ej. incidencias, problemas con paquetes) filtrados por período y transportista para tomar decisiones estratégicas en los próximos envíos basadas en problemas recurrentes o áreas de mejora.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>6</td>
      <td>US03</td>
      <td>Visualización de envíos asignados a un transportista</td>
      <td>Como gerente, quiero ver el listado de envíos asignados a un transportista, incluyendo fechas de entrega, estado actual y detalles del envío, para poder medir el rendimiento de mis empleados en relación con la carga de trabajo y el cumplimiento de plazos.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>7</td>
      <td>US01</td>
      <td>Visualización de paquetes entregados por un transportista</td>
      <td>Como gerente, quiero visualizar el número y detalle de paquetes entregados por un transportista en un período específico para medir su rendimiento en términos de productividad y eficiencia.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>8</td>
      <td>US04</td>
      <td>Visualización de envíos asignados</td>
      <td>Como transportista, quiero poder ver los envíos que me han sido asignados, incluyendo direcciones de recogida y entrega, horarios estimados, contenido e instrucciones especiales, para poder organizar mejor el orden de mis tareas y optimizar mi ruta.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>9</td>
      <td>US13</td>
      <td>Reporte de problemas con el paquete</td>
      <td>Como transportista, quiero poder reportar problemas con los paquetes que transporto durante mis viajes, describiendo el problema (daño, faltante, etc.) y el número de paquete, para que el gerente pueda reportarlo al cliente y tomar las medidas correctivas.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>10</td>
      <td>US11</td>
      <td>Reporte de infracciones vehiculares</td>
      <td>Como transportista, quiero poder reportar infracciones vehiculares que ocurran durante mis viajes, detallando la ubicación, tipo de infracción y si es posible, adjuntar evidencia, para que el gerente pueda tomar las medidas del caso y garantizar la seguridad y el cumplimiento normativo.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>11</td>
      <td>US12</td>
      <td>Reporte de accidentes en la carretera</td>
      <td>Como transportista, quiero poder reportar accidentes en la carretera que ocurran durante mis viajes, detallando la ubicación, gravedad, si hay heridos y cualquier otra información relevante, para que el gerente pueda organizar las futuras rutas evitando zonas peligrosas o tomar las acciones necesarias de soporte.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>12</td>
      <td>US14</td>
      <td>Reporte de problemas técnicos</td>
      <td>Como transportista, quiero poder reportar problemas técnicos que surjan durante mis viajes con el vehículo o la aplicación (ej. fallo del motor, error de navegación), detallando el problema, para que el gerente pueda resolverlo lo antes posible y minimizar el impacto en las entregas</td>
      <td>3</td>
    </tr>
    <tr>
      <td>13</td>
      <td>US05</td>
      <td>Visualización de paquetes entregados</td>
      <td>Como transportista, quiero visualizar la lista de paquetes que he marcado como entregados, incluyendo la hora y la confirmación de entrega (si aplica) para tener un comprobante de trabajo realizado y poder resolver cualquier duda o reclamación.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>14</td>
      <td>US06</td>
      <td>Visualización de reportes realizados</td>
      <td>Como transportista, quiero visualizar los reportes que hice en mi labor, incluyendo la fecha, hora, tipo de reporte y descripción del problema, para tener un historial de incidencias en mi trabajo y poder referirme a ellos si es necesario.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>15</td>
      <td>US15</td>
      <td>Gestión de Perfil de Gerente</td>
      <td>Como gerente, quiero visualizar y editar mi información personal (como nombre, correo electrónico, número de teléfono) para asegurarme de que mis datos estén correctos y actualizados en el sistema.</td>
      <td>1</td>
    </tr>
    <tr>
      <td>16</td>
      <td>US16</td>
      <td>Gestión de Perfil de Transportista</td>
      <td>Como transportista, quiero visualizar y editar mi información personal (como nombre, correo electrónico, número de teléfono, información de contacto de emergencia) para asegurarme de que mis datos estén correctos y actualizados en el sistema.</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
