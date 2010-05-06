---
layout: default
title: xLab versión 1.8.4
---

### xLab versión 1.8.4 (30/May/2009)

#### Caso 10073 - Reporte de saldos detallados por compañía (Configurable)
En el reporte de saldos detallados por compañía se agregaron dos nuevos campos: Fecha de Factura y Días de Crédito de la Compañía.
Estos campos servirán para poder ver si alguna de las cuentas ha rebasado los días de crédito pactados con la empresa y se puede considerar como saldo vencido.

![100773](100773.jpg)

#### Caso 10669 - Agregar campo de comentario de Orden en reporte de pacientes por día (Configurable)
Se agrego un campo que puede mostrar el comentario de la orden en el reporte de pacientes por día

![10669](10669.jpg)

#### Caso 10705 - Agregar filtro por número de factura en la consulta de cuentas por empresa (Implementado)
Se agregó la siguiente funcionalidad en la pantalla de consulta de cuentas por empresa: Agregar filtro por número de factura.

![10705](10705.jpg)

#### Caso 10418 - Cambio en el cálculo de tiempo de entrega (Configurable)
Cambio en el cálculo de tiempos de entrega de las órdenes internas para que no tome en cuenta los domingos.

#### Caso 10751 - La primera vez que se abre la pantalla de órdenes o modificación si las marcamos como urgente le hace mal el cargo (Solucionado)
Cuando se abría por primera vez la pantalla de modificación de órdenes, al cargar un estudio como urgente, cargaba un 10% extra, aunque la prueba no fuese configurada con cargo adicional.

#### Caso 10761 - Problema en el reporte de principales clientes se queda pasmado (Solucionado)
Al generar el reporte de principales clientes en algunos días se quedaba congelada la aplicación y teníamos que salirnos del sistema.

#### Caso 10814 -  Error en la impresión de resultados cuando los analítos son calculados por fórmula (Solucionado)
Al realizar la impresión de resultados desde la ruta Resultados ) Impresión ) Por Ordenes de Paciente, el problema que se presentaba era que los analítos para los resultados que eran calculados por fórmula no los imprimía.

#### Caso 10665 - Impresión duplicada (Solucionado)
Se arreglo la pantalla de órdenes  por compañía para que no duplique la orden de laboratorio

#### Caso 10691 - Muestra el análito  aunque  venga vacío el testresult (para  pruebas  con resultado  secundario) (Solucionado)
Muestra el análito aunque no contenga un resultado, solo aplica para las pruebas con resultado secundario.

#### Caso 10690 - No está trabajando bien el foliador de ordenes cuando tienen periodo de reinicio ="D" (Solucionado)
El foliador "D", de reinicio diario tenia, no funcionaba correctamente, está solucionado

#### Caso 10565 - Separar los campos de Edad en GroupResult - Areaworksheet - LabRecept - Lablabel - Hiplabel (Configurable)
Permite se parar los D M y A de la edad, en caso de que se desee usar solo uno de estos datos.

#### Caso 10664 -No se puede refacturar en ceros ordenes que fueron canceladas después de facturar (Solucionado)
Cuando se cancelaba una orden facturada, no se podía matar la factura, actualmente ya se puede nuevamente refacturar en ceros para cancelar la factura.

#### Caso 10668 -Aumento de espacio en la pantalla de captura de datos (Implementado)
En la pantalla de captura de datos en las pruebas tipo texto libre, al escribir creaba un scroll bar en la parte de abajo para escribir continuamente a la derecha por lo que dificultaba la lectura.

