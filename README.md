
# Sistema de Monitoreo Fotovoltaico

**Propuesta de análisis y diseño de un sistema de monitoreo para panel solar mediante instrumentación de sensores y controladores.**

Universidad Técnica Federico Santa María – Sede Concepción  
Taller de Electricidad

## 1. Descripción del proyecto

Este repositorio contiene el software desarrollado para la propuesta de diseño de un sistema de monitoreo de una instalación fotovoltaica.

El sistema permite representar y procesar variables ambientales relacionadas con el funcionamiento de una planta solar, con el propósito de facilitar el análisis de su rendimiento y las posibles pérdidas de eficiencia.

El desarrollo contempla la utilización de un PLC Siemens, módulos de adquisición de señales analógicas y una interfaz de monitoreo.

## 2. Equipamiento utilizado

### Equipamiento de automatización

- Acoplador de bus Helmholz TB20 PROFIBUS-DP Slave (600-151-1AA11).
- Módulo Helmholz TB20 de 4 entradas analógicas de corriente (600-250-4AD01).
- PLC Siemens.
- Fuente de alimentación de 24 VDC.

### Elementos del simulador de señales

- 1 protoboard.
- 4 potenciómetros de 10 kΩ.
- 4 resistencias de 1 kΩ.
- Cableado de conexión.
- Fuente de alimentación de 24 VDC.

## 3. Variables simuladas

Para las pruebas de funcionamiento se utilizan cuatro señales analógicas de corriente de 4–20 mA, correspondientes a las siguientes variables:

| Canal | Variable representada |

| 1 | Irradiancia solar |
| 2 | Temperatura del módulo fotovoltaico |
| 3 | Temperatura ambiente |
| 4 | Suciedad superficial (Soiling) |

Las señales son generadas mediante potenciómetros, permitiendo modificar las entradas analógicas y observar la respuesta del sistema de monitoreo.

El procesamiento y la interpretación de las señales se encuentran implementados en los bloques de programación del PLC.

## 4. Montaje del simulador de señales

El simulador utiliza cuatro canales independientes, implementados mediante potenciómetros de 10 kΩ y resistencias de 1 kΩ.

El circuito se alimenta mediante una fuente de 24 VDC y permite generar señales regulables para las cuatro entradas analógicas del módulo Helmholz TB20.

La conexión de los canales se realiza hacia las entradas de corriente del módulo de adquisición, utilizando un canal para cada variable representada.

## 5. Descarga y puesta en marcha

### Requisitos

- Sistema operativo Windows.
- Siemens TIA Portal V19.
- Equipamiento de automatización compatible con la configuración del proyecto.
- Módulos Helmholz TB20 correspondientes.

### Recuperación del proyecto

1. Descargar el archivo `PROYECTO_FINALll.zap19` desde este repositorio.
2. Abrir Siemens TIA Portal V19.
3. Seleccionar la opción **Retrieve (Recuperar proyecto)**.
4. Seleccionar el archivo descargado.
5. Indicar la carpeta de destino.
6. Esperar a que finalice la recuperación.
7. Abrir el proyecto para revisar su programación y configuración.

### Funcionamiento

Para realizar las pruebas se debe disponer del equipamiento de automatización y del simulador de señales.

Una vez verificadas las conexiones y la configuración del sistema:

1. Poner en funcionamiento el sistema de automatización.
2. Modificar los potenciómetros para variar las señales de entrada.
3. Observar la adquisición y procesamiento de las variables.
4. Verificar la respuesta del sistema de monitoreo mediante la interfaz desarrollada.

## 6. Alcances y limitaciones

El presente desarrollo corresponde a una propuesta de diseño validada mediante simulación.

Las señales utilizadas durante las pruebas son generadas mediante potenciómetros, representando las variables que en una implementación real serían obtenidas mediante sensores físicos.

Por lo tanto, el proyecto no contempla la adquisición directa de datos desde el panel fotovoltaico.

La instalación de sensores reales, la integración definitiva con la planta fotovoltaica y la validación experimental del sistema corresponden a etapas posteriores, fuera del alcance del presente trabajo.

## 7. Disponibilidad del software

El proyecto original se encuentra disponible en este repositorio de GitHub para su descarga, revisión y eventual continuidad por parte del personal encargado del laboratorio.

**Archivo:** `PROYECTO_FINALll.zap19`  
**Software de desarrollo:** Siemens TIA Portal V19.


La incorporación de sensores físicos, la adquisición de datos reales desde la instalación fotovoltaica y la implementación definitiva del sistema quedan fuera del alcance de este trabajo.

## 7. Disponibilidad

El proyecto se encuentra disponible para su descarga y revisión en este repositorio de GitHub.
