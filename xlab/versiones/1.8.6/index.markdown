---
layout: default
title: xLab versión 1.8.6
---

### xLab versión 1.8.6 (30/Ago/2009)

#### Caso 11247 - Consolidar cuentas de una  compañía a un paciente de  otra  compañía diferente al de las  cuentas  a consolidar. (Implementado)
Se requiere que al momento de  consolidar se congelen las cuentas, porque  cuando se  consolidan las cuentas de  una compañía (empresa1) a un paciente de  otra  compañía(empresa2), como se crea  una  nueva cuenta se guardan los  beneficios de la  nueva cuenta y no los  beneficios de las  cuentas  originales.
Por el momento se  agrego un warning para avisar que el paciente es de otra compañía diferente a la de las cuentas.

![11247](11247.jpg)

#### Caso 9667 - Generar  directo  resultado  web  a PDF con formato  de laboratorio y marca de  agua informativo. (Configurable)
Se agrego  una nueva pantalla  para seleccionar  que  ordenes  quieren  liberar  a  Internet

![9667](9667.jpg)

De las  ordenes  seleccionadas  se  crea un archivo  en formato PDF  el cuál es una copia  exacta de  su  resultado con una  leyenda  que indica que el resultado es  informativo.

![9667_2](9667_2.jpg)

* RESULTADOS EN EL SISTEMA XLAB

![9667_3](9667_3.jpg)

* RESULTADOS EN INTERNET (LABONLINE)

![9667_4](9667_4.jpg)

Adicionalmente  al archivo liberado  por  Internet se crea un respaldo de manera automática de  dichos archivos en formato pdf en una  carpeta  que el cliente seleccione para una  mejor administración de las ordenes  liberadas  para su consulta  en Internet.

![9667_5](9667_5.jpg)

En el sitio labonline se liberan únicamente  aquellas  órdenes que  fueron liberadas  mediante la pantalla  de Liberar Resultados  a  Internet.

![9667_6](9667_6.jpg)

#### Caso 11324 - Error al modificar una orden, se marca como urgente pero no se respeta. (Reparado)
Cuando se modifica una orden a status urgente, no lo guardaba como tal, por lo que en los reportes Hoja de trabajo por área y Reporte de estudios urgentes; No se reflejaba el cambio.

![11324](11324.jpg)

#### Caso 11063 - Mostrar columna de sensibilidad en la pantalla de captura. (Implementado)
En la versión anterior se tenía que desplazar con el scroll o las flechas en la pantalla de captura para ver la columna de sensibilidad.

![11063](11063.jpg)

#### Caso 11083 - No aparece el status en el seguimiento de órdenes. (Implementado)
En la pantalla de seguimiento de ordenes aparecían en blanco los status de las ordenes.

![11083](11083.jpg)

#### Caso 9682 - Usar contenedor de  prueba, no de perfil en la etiqueta. (Configurable)
En la  etiqueta  aparecía el tubo o envase del perfil, ahora aparece el tubo o envase de las pruebas individuales que forman parte  del perfil.
En este caso desglosa el tubo o envase de la química sanguínea  y el tubo o envase de la biometría.

![9682](9682.jpg)

#### Caso 9666 - Agregar botón en pantalla de impresión de orden para envío directo a PDF (Configurable)
Botón en la pantalla de  impresión de Resultados que  genera  automáticamente el resultado en  formato PDF.

![9666](9666.jpg)

Los archivos generados en formato PDF se guardan de manera automática en una  carpeta  que el cliente seleccione.

![9666_2](9666_2.jpg)

#### Caso 9648 - Botón Siguiente en la Pantalla de Captura de Resultados (Implementado)
Se agrego un botón para salvar el resultado capturado y de inmediato abrir el próximo a capturar, sin necesidad de salir de la pantalla de captura.

![9648](9648.jpg)

#### Caso 11359 - Corregir la edad que se presenta en la pantalla de impresión (Implementado)
Ahora en todas las pantalla de impresión de resultados, sea por área o paciente muestran la edad de la orden.

![11359](11359.jpg)

#### Caso 11315 - Error al cuadrar los totales en el reporte de Estudios Efectuados (Configurable)
Cuando se  detallan  perfiles  no  cuadra  el número de pacientes, estudios y totales, porque no hay manera de desglosar el precio por estudio individual, ya que el precio que se muestra es el precio del perfil, por otro lado se arreglo el reporte para que  agrupe por paciente y luego por estudio.

* Cuando se desglosa el perfil  desaparecen las columnas de importe total, y  pacientes.

![11315](11315.jpg)

* Cuando no se  desglosa  el perfil el reporte  detalla estudios, pacientes e  importes.

![11315_2](11315_2.jpg)

#### Caso 11407 - Permitir meter  una fecha de toma de muestra  que sea anterior  a la fecha de la orden (Implementado)
El sistema  permite registrar una  fecha de toma de muestras anterior  a la fecha de orden, apareciendo en el reporte de  resultados la fecha de toma de muestra y en el seguimiento de ordenes  ambas fechas la de orden y la de toma de muestra.

![11407](11407.jpg)

#### Caso 11504 - No está tomando la empresa de la orden en el reporte de  prestaciones  no facturadas (Implementado)
Para  el reporte  de prestaciones  no facturadas no está  mostrando en el reporte la empresa  con la que fue  generada  la orden, si no que mostraba la empresa que tenía el paciente  en el registro.

#### Caso 8360 - Tarda mucho y a veces  se queda  trabado el reporte de Servicios  por Cliente (Implementado)
Se optimizo el reporte  para  desplegar los  datos de manera más rápida y que no se quede trabado el sistema.

#### Caso 9678 - Agregar  filtro en la impresión para  que filtre  por  sucursal (Implementado)
En la pantalla de  impresión de  resultados por paciente e impresión de  resultados por área  se  agrego un filtro por  sucursal.

![9678](9678.jpg)

#### Caso 9671 - Agregar  botón en el catálogo de empresas para agregar una leyenda  en el resultado (Implementado)
Esta  funcionalidad  permite  agregar una leyenda  en el  resultado, para las empresas y ordenes  que así lo indiquen.
Se agrego en al  catálogo de empresas una pestaña  para  agregar una leyenda en los resultados

![9671](9671.jpg)

En la pantalla de orden a paciente  externo, se agrego un como para seleccionar  si para la orden  desea agregar  la leyenda  de la empresa.

![9671_2](9671_2.jpg)

En el resultado se   agrega  la  leyenda.

![9671_3](9671_3.jpg)

#### Caso 11639 - Que no permita poner 0 en la edad  del paciente en la pantalla registro de pacientes (Implementado)
Cuando ponen edad 0 el sistema pone un warning  para evitar errores  al capturar la edad.

![11639](11639.jpg)

Caso 11660 - Al modificar la orden actualizar el campo de la edad (Implementado)
Para actualizar la edad del paciente sobre alguna orden en específico

Paso1: Modificar la edad en el registro de pacientes

![11660](11660.jpg)

Paso2: Entrar a modificación de ordenes, buscar la orden, agregar le comentario y guardar

![11660_2](11660_2.jpg)





