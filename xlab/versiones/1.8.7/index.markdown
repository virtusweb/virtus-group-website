---
layout: default
title: xLab versión 1.8.7
---

### xLab versión 1.8.7 (31/Ene/2010)

#### Caso 11706 - Agregar el campo credencial (companycardnum) en el reporte de pacientes por  día. (Configurable)
Se requiere que el campo credencial  que se registra en la pantalla registro de pacientes se agregue en el reporte de pacientes  por día.

![11706](11706.jpg)

#### Caso 11690 - En el catálogo de pruebas de laboratorio de referencia quitar candado para eliminar pruebas aunque ya tengan ordenes de maquila. (Implementado)
Se agrego la funcionalidad para quitar el candado que no permitía eliminar pruebas a laboratorios de referencia si ya existían ordenes, el sistema ahora manda un mensaje y  permite eliminar la referencia de la prueba al laboratorio de referencia.

![11690](11690.jpg)

#### Caso 11411 - Agregar combo de pruebas y análitos en pantallas de emisión de reportes de estudios y medias de resultados. (Implementado)
Dentro de los  reportes estadísticas por análito y medias de resultados se inserto un combo en los filtros pruebas y análitos.

![11411](11411.jpg)

![11411_2](11411_2.jpg)

#### Caso 11844 - Que tome el área de la prueba en el reporte hoja de trabajo por área y no que tome el área del análito de la prueba. (Configurable)
Actualmente el reporte de hoja de trabajo por área  genera el reporte por área del análito y con este  cambio el reporte se generara por área de la prueba

#### Caso 11731 - En la pantalla consulta de órdenes pendientes por área  presentar la información en forma de gráfica  de pay (Implementado)

Se agrego una nueva pantalla de consulta que despliega todas las órdenes pendientes por área, mostrando gráficamente las órdenes en el estatus en que se encuentran

![11731](11731.jpg)

![11731_2](11731_2.jpg)

#### Caso 11981 - Mandar una advertencia en la pantalla de órdenes por empresa cuando la empresa no tenga crédito. (Implementado)
Se agrego un aviso de responsabilidad del usuario cuando no hay crédito, además se agrego en la pantalla de órdenes el saldo a favor con el que pudiere contar en ese momento la empresa que no tiene crédito.

![11981](11981.jpg)

#### Caso 12050 - Agregar valores de referencia al reporte de resultados histórico (Configurable)
En el reporte de resultados histórico ya puede contener o no, los valores de referencia por prueba

![12050](12050.jpg)

#### Caso 12045 - Poder deshabilitar una prueba a laboratorio de referencia (Configurable)
Esta opción le permite deshabilitar la prueba al laboratorio de referencia, únicamente se generara la orden al laboratorio si usted la marca  como activa

![12045](12045.jpg)

Para activar o desactivar la prueba de clic sobre el botón modificar como se indica en la siguiente pantalla

![12045_2](12045_2.jpg)
