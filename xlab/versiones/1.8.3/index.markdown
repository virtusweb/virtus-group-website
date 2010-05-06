---
layout: default
title: xLab versión 1.8.3
---

### xLab versión 1.8.3 (30/Abr/2009)

#### Caso 10430 - Hacer configurables la cantidad de resultados (Implementado)

En caso de que el usuario filtre la consulta por cualquier campo, el sistema 
desplegará todas los órdenes que cumplan con ese filtro. Si el usuario no mete 
ningún criterio de consulta entonces solo desplegará las primeras 100 órdenes 
(más recientes).

![10430](10430.jpg)

#### Caso 10489 - Agregar nuevos campos - rptCompanyReport.rpt - número de cuenta bancario, razón social y clave de compañía (Configurable)
Estos campos se pueden configurar en el reporte para ser utilizados a petición del usuario

![10489](10489.jpg)

#### Caso 10427 - Hacer que la vista previa ocupe toda la pantalla y empiece en 110%  (Implementado)
Se agregó funcionalidad a la pantalla de vista previa de reportes para poder seleccionar el % de zoom con el que se despliega el reporte.

![10427](10427.jpg)

#### Caso 10447 - Agregar campo de Número de Factura en reporte de pacientes por día (Configurable)
Se agregó el campo de número de factura en el reporte de pacientes por día dentro del subreporte de pago de saldos de otros días.

![10447](10447.jpg)

#### Caso 10458 - Desplegar orden en la pantalla de abonos aunque este consolidada (Implementado)
Para el caso de órdenes consolidadas se modificó el sistema para que permita desplegar y abonar en cuentas consolidadas usando tanto el paciente original de la orden como el paciente al que fue consolidada la orden.

![10458](10458.jpg)

#### Caso 6198 - Agregar un menú para seleccionar los motivos de la cancelación y un campo para observaciones (Implementado)	
Se hizo una adecuación para que el motivo de cancelación de una orden o estudio ya sea un dato requerido (obligatorio).

![6198](6198.jpg)

#### Caso 9679 - En  la pantalla de  consulta de  órdenes  de laboratorio que lleve  la empresa  y la edad (Implementado)
Se agregaron los campos de edad del paciente (en años) y la empresa a la pantalla de consulta de órdenes.

![9679](9679.jpg)

#### Caso 9651 - Agregar campos a la Pantalla de Impresión de Resultados (Implementado) 
Se modificaron las pantallas de impresión de resultados por área y por paciente para agregar los campos de edad del paciente y comentarios de la orden.

* Por Área de Trabajo

![9651](9651.jpg)

* Por Paciente

![9651_2](9651_2.jpg)

#### Caso 9874 - Arreglar filtro  en pantalla pruebas de laboratorios de referencia  (Implementado)
Se modificó la pantalla de consulta de pruebas por laboratorio de referencia para que si seleccionas un laboratorio de referencia únicamente te despliegue las pruebas que están configuradas para ese laboratorio.

![9874](9874.jpg)

#### Caso 10250 - Meter un campo en órdenes para saber si trajo orden del Laboratorio o no  (Configurable)
Se agregó un nuevo campo para marcar si el paciente trajo la orden del laboratorio (enviado por el médico) o llegó solo.

![10250](10250.jpg)

#### Caso 10384 - Agregar catálogo de microorganismos para pruebas de bacteriología (Implementado)
SE AGREGÓ LA SIGUIENTE FUNCIONALIDAD A LA PANTALLA DE CAPTURA DE RESULTADOS DE MICROBIOLOGÍA:
Para pruebas de bacteriología si se presiona la tecla FIN en la pantalla de captura de resultados, se despliega un catálogo de microorganismos que pueden ser buscados por nombre y código y seleccionar uno por medio de doble clic.
El catálogo de microorganismos se almacena en el catálogo general y puede ser actualizado por un usuario que tenga acceso a este catálogo.

![10384](10384.jpg)

#### Caso 10385 - Al capturar resultados que puedan ir rápidamente a un analito (Implementado>
Se agregó la siguiente funcionalidad en la pantalla de captura de resultados: por medio de la tecla inicio, permite ir rápidamente a un analito especifico ya sea por las primeras letras del nombre del analito o bien por el número de renglón.

![10385](10385.jpg)

#### Caso 10459 - Desplegar ordenes Facturadas (Implementado)
Se modificó la pantalla de abonos para desplegar todas las cuentas del paciente sin importar su estatus (PENDIENTE O FACTURADO).

![10459](10459.jpg)

#### Caso 10462 - Agregar número de  estudios solicitados  e  impresos en  reporte de  resultados (Configurable)
En el reporte de resultados se agregaron el número de estudios solicitados en la orden y el número de estudios impresos.

![10462](10462.jpg)

#### Caso 10420 - Agregar variable de configuración en hoja de trabajo para que no aparezcan asteriscos antes del número de orden (Configurable)
Se agregó una variable de configuración para definir si en la hoja de trabajo por área se debe imprimir o no un asterisco antes del número de orden para las órdenes urgentes. Actualmente con asterisco agrupa urgencias primero y consecutivo de orden (arriba urgencias y después las demás).
Con la variable se puede tener el consecutivo y adicionar un campo “S” que indica que es una urgencia

![10420](10420.jpg)

#### Caso 10407 - Que de un resultado numérico necesitan que automáticamente se convierta en texto como POSITIVO (Implementado)
Se agregó funcionalidad en el catálogo de pruebas y pantallas de captura de resultados para poder configurar analitos tipo formula que puedan regresar un texto en base a una condición. Por ejemplo que en base al valor numérico de otro analito nos pueda regresar "POSITIVO" O "NEGATIVO". 
En el catálogo de pruebas este nuevo tipo de analito debe configurarse como formula texto o FORMTEXT y utilizar la siguiente instrucción: 
IF(&lt;&lt;analito1&gt;&gt; condición, "texto si es verdadera la condición", "texto si es falsa").  

Por ejemplo IF(&lt;&lt;PH&gt;&gt; &gt; 7, "POSITIVO", "NEGATIVO")

![10407](10407.jpg)

#### Caso 10298 - Botón de Hojas de trabajo no funciona (Solucionado)
En la pantalla de Impresión de documentos de trabajo, al utilizar el botón de imprimir ordenes podía sucedes que no sucediera nada, de no estar configurado para utilizar las hojas de trabajo por área o paciente, despliega un aviso.

![10298](10298.jpg)

#### Caso 9754 - Que no se  pueda  abonar  a  una  cuenta más de  lo que debe  (Implementado)
Se modificó la pantalla de abonos para que si se quiere abonar más de lo que se debe te mandé un mensaje de advertencia por si se trata de algún error.

![9754](9754.jpg)

#### Caso 8329 - Agregar el nombre completo del usuario que genera la orden a lab de referencia (Configurable)
Se agregó el nombre completo del usuario que genera la orden al lab de referencia
* Se puede configurar en el reporte a petición del cliente

![8329](8329.jpg)

#### Caso 8219 - Agregar campos en reporte de resultados urgentes (Configurable)
Para el reporte de resultados urgentes se agregaron 2 nuevos campos: fecha de recepción de la orden y fecha de impresión para poder saber el tiempo de atención y el nivel de cumplimiento de las órdenes urgentes.
* Se puede configurar en el reporte a petición del cliente

![8219](8219.jpg)

#### Caso 8328 - Agregar edad y sexo del Paciente en la impresión de órdenes a Lab. de Referencia (Configurable)
Se agregaron los campos de edad y sexo en el reporte de orden de trabajo a lab. de referencia.
* Se puede configurar en el reporte a petición del cliente

![8328](8328.jpg)

#### Caso 10251 - En el reporte de médicos dividir las órdenes que trajeron orden de Laboratorio y las que no (Configurable)
Se agregó funcionalidad al reporte de médicos para poder dividir las órdenes en las que el paciente trajo la orden del laboratorio (es decir el médico envió al paciente) y las órdenes en las que el paciente no la trajo.
* Se puede configurar en el reporte a petición del cliente

#### Caso 10467 - Agregar  la cantidad con letra  al presupuesto (Configurable)
* Se puede configurar en el reporte a petición del cliente

#### Caso 10341 - Que en la consulta de  ordenes  web se  pueda teclear el cuarto (Implementado)
Se agregó funcionalidad para que te permita editar el campo de cuarto en la pantalla de órdenes web.

#### Caso 9688 - Generar orden de maquila de todas las sucursales y de todos los laboratorios de referencia a la misma vez (Implementado)
Se agregó nueva funcionalidad a la pantalla de órdenes a laboratorios de referencia para poder seleccionar que se enviarán de todas las sucursales y hacia todos los laboratorios de referencia de una misma vez.
 	
#### Caso 10332 - Aparecen ordenes  ya pagadas en la pantalla de pagos de empresas para las  consolidadas (Implementado)
Se agregó un campo en la pantalla de pagos por empresa para desplegar el total de pagos de crédito (cobranzas) para que lo tome en cuenta en el saldo de la empresa. 

#### Caso 10364 – Variable de Configuración Terminal Server para poner la sesión como prefijo en el nombre del reporte  (Solucionado)
Soluciona el problema de Impresión de reportes (Etiquetas, ordenes, etc) des configurados por cambio de numero de sesión en Terminal Server

#### Caso 10409 - Error en la pantalla de captura de Resultados al darle clic en algún analito se regresa al inicio (Solucionado)
Sucedía que al querer capturar un resultado la pantalla regresaba al inicio, complicando la captura de resultados. 

#### Caso 10078 - No les permite meter el cargo extra por urgencia en la pantalla de modificación de órdenes (Solucionado)
No les permite meter el cargo extra por urgencia en la pantalla de modificación de órdenes 

#### Caso 10336 - Ordenes WEB deja  en blanco usuario y contraseña de pacientes  ya registrados (Solucionado)

#### Caso 10363 - Bug en la Impresión de Etiquetas  (Solucionado)  
Al presionar la esquina se seleccionan todas las pruebas y se pueden imprimir en conjunto, sin tener que hacerlo una por una.

![10363](10363.jpg)

#### Caso 10433 - Reporte de estudios  fuera de rango no toma en cuenta  los perfiles (Solucionado)   
En el reporte de estudios fuera de rango omitía los perfiles, actualmente los presenta sin problemas.

* Funcionalidad Nueva en filtros de Impresión

![10433](10433.jpg)

1 Esta activado por default, presenta las ordenes con todos sus estudios listos para imprimir, al desactivarlo presenta todos los resultados como lo hacia anteriormente.

2 Permite filtrar por espera de impresión, espera de entrega, entregados y todos.

3 Se puede configurar que en el reporte de resultados, imprima el usuario que autorizo la impresión.
