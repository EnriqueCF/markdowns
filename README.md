---
title: Nuevo fichero de información para el Consorcio
keywords:
description: Solución para generación de informaciones para el Consorcio
isapp: true
createdate: 2018-10-23
modifieddate: 2018-10-23
---
## Datos generales - Nuevo fichero de información para el Consorcio
### Contexto Proyecto
* **Nombre de la aplicación**: Nuevo fichero de información para el Consorcio
* **URL a la aplicación**: _pendiente_
* **Team project que lo contiene**:_pendiente_
* **Versión actual**: 0.0
* **Monitorización**: No
* **Descripción**: Proceso automatizado para la generación mensualmente de un fichero que contiene pólizas, movimientos y recibos. El fichero se enviará para el Consorcio de Compensación de Seguros.
* **Usuarios**: responsables de negocio
* **Naturaleza de los usuarios**: interno
* **Responsable SCA**: Pelao Devesa, Xavier (Sistema)
* **Tipo de aplicación**: _pendiente_
* **Piezas**: Frontend(Angular), Backend(OracleDB), ETL (PowerCenter/Control-M) y Transferencia(SFTP Corporativo).

### Introducción

El **Consorcio de Compensación de Seguros** ve la necesidad de que las entidades aseguradoras remitan al Consorcio, junto a la declaración de los recargos, información complementaria de las pólizas respecto a las que se han ingresados los recargos, los capitales asegurado o la localización de los riesgos.

Este proyecto busca implantar un **proceso automatizado** para la generación mensualmente  de un fichero que contiene pólizas, movimientos y recibos. El fichero se enviará para el Consorcio de Compensación de Seguros mensualmente y el plazo de presentación de los recargos será dentro de los veinte primeros días del mes siguiente del periodo de liquidación.

La creación de un nuevo (y único) fichero a nivel de “póliza – movimiento – recibo” con la información complementaria que solicita el. El fichero deberá incorporar la información de todas las aplicaciones de pólizas.

Una vez se disponga del fichero único, se tendrá que enviar en un **“repositorio”** del Consorcio (más adelante el CCS proporcionara más información sobre el nuevo aplicativo) en el caso que dicho aplicativo genere algún tipo de indicen encía o detecte cualquier error en fechas o contenido, se tendrá que poder modificar los errores y volver a cargar y enviar la información.

La filosofía del nuevo sistema de declaración a través del Fichero de Información Complementaria, es la de poder informar de los recargos de manera individualizada por póliza.
La evolución de la póliza a lo largo de su ciclo, tanto dentro de su periodo de vigencia, como en futuras renovaciones, va teniendo variaciones que suponen cambios en los capitales, garantías cubiertas y en los recargos correspondientes, bien en los que giran sobre los capitales o bien en los que giran sobre la prima. En cualquier caso, lo que el sistema requiere, es poder recopilar esa evolución que afecta a los componentes económicos de la póliza para disponer de una coherencia entre los riesgos cubiertos y los recargos cobrados.

Asimismo, ayudará al Consorcio a establecer con mayor calidad técnica las futuras tarifas de recargos.