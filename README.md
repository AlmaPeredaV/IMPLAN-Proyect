# Sistema de ingresos 

## Nombre del proyecto
Desarrollar un sistema de gestión de ingresos para el Instituto Municipal de Planeación (IMPLAN)

## Descripción
Desarrollar un sistema web que permita realizar la captura de nuevos ingresos, imprimmir los recibos y generar reportes mensuales de las ventas realizadas.

## Objetivos
- Objetivo general

Desarrollar un sistema de gestión de ingresos y cobros que permita el registro, control y consulta de operaciones financieras, mejorando la eficiencia administrativa y reduciendo errores en el manejo de la información.

- Objetivos específicos

    - Analizar los procesos actuales de registro de ingresos.

    - Diseñar la estructura del sistema.
      
    - Implementar un módulo de autenticación de usuarios.
      
    - Desarrollar un módulo de registro de cobros.
      
    - Crear un sistema de consulta y visualización de datos.
      
    - Generar reportes básicos de ingresos.
      
    - Validar el funcionamiento del sistema mediante pruebas.


## Delimitación
- Alcance
  
El presente proyecto contempla el desarrollo de un sistema de gestión de ingresos que permitirá:

- Registrar usuarios del sistema.
  
- Registrar ingresos o pagos realizados.
  
- Consultar historial de cobros.
  
- Generar reportes de ingresos mensuales.
  
- Validar acceso mediante autenticación.
  
- Implementar una interfaz amigable para la captura y visualización de datos.

El sistema se desarrollará como un sistema web, considerando funcionalidades esenciales para el control de ingresos dentro del periodo de estadía.

- Limitaciones
  
El desarrollo del proyecto presenta las siguientes limitantes:

- Limitación en el uso de herramientas avanzadas o licencias de software.
  
- Dependencia de la información disponible para el diseño del sistema.
  
- No se contempla inversión en infraestructura adicional.
  
- El desarrollo se realizará dentro del periodo establecido de estadía.
  
- El sistema será implementado en un entorno institucional.
  
- Dependencia de autorizaciones para acceso a información real.
  
- Adaptación del sistema a los procesos actuales de la organización.

## Requerimientos funcionales

Inicio de sesión

- El sistema deberá permitir el inicio de sesión de los usuarios registrados mediante correo electrónico y contraseña. El sistema deberá validar las credenciales y permitir el acceso según el rol asignado: Administrador o Cajero.
  
Gestión de usuarios

- El sistema deberá permitir al Administrador registrar, consultar, editar y eliminar usuarios. Para cada usuario se deberán capturar los siguientes datos: nombre, apellido paterno, apellido materno, puesto, correo electrónico, contraseña y rol.

Asignación de roles

- El sistema deberá permitir al Administrador asignar un rol a cada usuario. El rol Administrador tendrá acceso completo al sistema, mientras que el rol Cajero solo podrá registrar cobros, consultar movimientos y generar reportes.

Registro de cobros

- El sistema deberá permitir al Cajero registrar un cobro ingresando los siguientes datos: contribuyente, concepto de pago, monto, tipo de pago, fecha, folio y empleado que realiza el cobro.

Validación de cobros

- El sistema deberá validar que el monto del cobro sea mayor a cero, que el folio no esté duplicado y que todos los campos obligatorios estén completos antes de guardar el registro.

Generación de recibos

- El sistema deberá generar automáticamente un recibo digital después de registrar un cobro. El recibo deberá mostrar folio, fecha, contribuyente, concepto, monto, tipo de pago y empleado responsable.

Consulta de recibos

- El sistema deberá permitir consultar los recibos registrados mediante filtros como fecha, folio, contribuyente, concepto o tipo de pago.

Generación de reportes

- El sistema deberá permitir generar reportes de ingresos por día, mes o año. El reporte deberá mostrar los cobros registrados, el total de ingresos y los datos principales de cada recibo.

Descarga de reportes

- El sistema deberá permitir descargar los reportes generados en formato PDF o Excel para su almacenamiento o impresión.

Panel de control

- El sistema deberá mostrar un panel de control con información resumida, como total de ingresos, movimientos recientes, cantidad de recibos registrados y estadísticas por periodo.

Gestión de catálogos

- El sistema deberá permitir registrar, consultar, editar y eliminar catálogos como conceptos de pago, tipos de pago, cargos y cantidades.

Cierre de sesión

- El sistema deberá permitir cerrar la sesión del usuario de forma segura, evitando que otra persona acceda al sistema sin autenticación.


## Requerimientos no funcionales

Seguridad

- El sistema deberá proteger el acceso mediante autenticación con JWT y contraseñas encriptadas.

Control de acceso

- El sistema deberá restringir las funciones disponibles de acuerdo con el rol del usuario

Rendimiento

- El sistema deberá responder las consultas y registros en un tiempo máximo de 2 segundos en condiciones normales de uso.

Disponibilidad

- El sistema deberá estar disponible durante el horario laboral de la dependencia.

Integridad de datos

- El sistema deberá evitar registros duplicados, pérdida de información o inconsistencias en los cobros.

Usabilidad

- El sistema deberá contar con una interfaz clara, sencilla y fácil de utilizar para el personal administrativo.

Compatibilidad

- El sistema deberá funcionar correctamente en navegadores web modernos como Google Chrome, Microsoft Edge y Mozilla Firefox.

Mantenibilidad

- El sistema deberá estar desarrollado con una estructura organizada que permita realizar futuras modificaciones o ampliaciones.



## Metodología de desarrollo de software

Para el desarrollo del sistema web de gestión de ingresos del Instituto Municipal de Planeación (IMPLAN), se utilizará la metodología Scrum, basada en un enfoque iterativo e incremental.

Esta metodología permitirá desarrollar el sistema en ciclos cortos, facilitando la entrega continua de funcionalidades como el registro de pagos, generación de recibos y consulta de ingresos, así como la incorporación de mejoras basadas en la retroalimentación del personal administrativo.

## Fases del desarrollo del sistema

### Planificación y Análisis de Requerimientos

- Definición del problema:

gestión manual de cobros y riesgo de pérdida de información.

- Identificación de objetivos del sistema:
  
  digitalizar y optimizar el control de ingresos.
  
- Levantamiento de requerimientos mediante:
  
  - Entrevistas con personal administrativo.
  - Observación del proceso actual.
  - Análisis de documentos físicos.
    
- Identificación de requerimientos funcionales y no funcionales.
  
- Selección de tecnologías:

MySQL, Spring Boot, JavaScript y autenticación JWT.

### Diseño del Sistema

- Definición de la arquitectura del sistema:
  
   - Backend con Spring Boot.
   - Frontend con JavaScript.
   - Base de datos MySQL.

- Diseño de módulos principales:

   - Gestión de usuarios
   - Gestión de cobros
   - Generación de recibos
   - Reportes y panel de control
  
- Diseño del modelo de datos para evitar duplicidad e inconsistencias.
  
- Definición de roles y permisos (administrador y cajero).

### Desarrollo e Implementación

- Desarrollo del sistema de autenticación con JWT.
  
- Implementación del CRUD de usuarios.
  
- Desarrollo del módulo de registro de pagos.
  
- Implementación de la generación automática de recibos digitales.
  
- Desarrollo de consultas de historial de ingresos.
  
- Implementación de reportes (diarios, mensuales y anuales).
  
- Integración de todos los módulos en una aplicación web funcional.

### Pruebas y Validación

- Pruebas funcionales de cada módulo:
  
   - Registro de pagos
   - Generación de recibos
   - Consulta de ingresos
   - Validación de seguridad (acceso por roles).
   
- Pruebas de integridad de datos (evitar duplicados o pérdidas).
  
- Evaluación del sistema con usuarios administrativos del IMPLAN.
  
- Corrección de errores detectados.

### Despliegue y Mantenimiento

- Implementación del sistema en un entorno real dentro del IMPLAN.
  
- Capacitación básica a los usuarios del sistema.
  
- Monitoreo del funcionamiento del sistema.

## Modelo Scrum

- Diagramas UML
  
![Diagramas](https://github.com/AlmaPeredaV/IMPLAN-Proyect/blob/main/Diagramas_UML.md)

- Base de datos

![Base de datos](https://github.com/AlmaPeredaV/IMPLAN-Proyect/blob/main/base%20de%20datos.md)

- Diseño

![Diseño administrador](https://github.com/AlmaPeredaV/IMPLAN-Proyect/blob/main/dise%C3%B1o.md)

![Diseño usuario](https://github.com/AlmaPeredaV/IMPLAN-Proyect/blob/main/dise%C3%B1o2.md)

- Tablero

![Calendario](https://github.com/users/AlmaPeredaV/projects/1/views/4)

![Kanban](https://github.com/users/AlmaPeredaV/projects/1/views/1)
## Fase de desarrollo

## Pruebas y resultados
