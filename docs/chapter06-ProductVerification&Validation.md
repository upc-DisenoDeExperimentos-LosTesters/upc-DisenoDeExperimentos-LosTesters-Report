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
