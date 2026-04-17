# Sistema de ingresos 

## Descripción
Desarrollar un sistema web que permita realizar la captura de nuevos ingresos, imprimmir los recibos y generar reportes mensuales de las ventas realizadas.

## Objetivos
-Objetivo general

Desarrollar un sistema de gestión de ingresos y cobros que permita el registro, control y consulta de operaciones financieras, mejorando la eficiencia administrativa y reduciendo errores en el manejo de la información.

-Objetivos específicos

•	Analizar los procesos actuales de registro de ingresos.

•	Diseñar la estructura del sistema.

•	Implementar un módulo de autenticación de usuarios.

•	Desarrollar un módulo de registro de cobros.

•	Crear un sistema de consulta y visualización de datos.

•	Generar reportes básicos de ingresos.

•	Validar el funcionamiento del sistema mediante pruebas.


## Delimitación
- Alcance
  
El presente proyecto contempla el desarrollo de un sistema de gestión de ingresos que permitirá:

•	Registrar usuarios del sistema.

•	Registrar ingresos o pagos realizados.

•	Consultar historial de cobros.

•	Generar reportes de ingresos mensuales.

•	Validar acceso mediante autenticación.

•	Implementar una interfaz amigable para la captura y visualización de datos.

•	Pendiente (Implementar un sistema de facturación.)

El sistema se desarrollará como un sistema web, considerando funcionalidades esenciales para el control de ingresos dentro del periodo de estadía.

- Limitaciones
  
El desarrollo del proyecto presenta las siguientes limitantes:

•	Limitación en el uso de herramientas avanzadas o licencias de software.

•	Dependencia de la información disponible para el diseño del sistema.

•	No se contempla inversión en infraestructura adicional.

•	El desarrollo se realizará dentro del periodo establecido de estadía.

•	El sistema será implementado en un entorno institucional.

•	Dependencia de autorizaciones para acceso a información real.

•	Adaptación del sistema a los procesos actuales de la organización.

## Requerimientos funcionales

- Gestión de usuarios
  
•	El sistema deberá permitir el registro de usuarios (administrador y cajero). 

•	El sistema deberá permitir el inicio de sesión mediante autenticación segura (JWT). 

•	El sistema deberá permitir la gestión de usuarios (crear, editar, eliminar) por parte del administrador. 

•	El sistema deberá asignar roles y permisos según el tipo de usuario.

- Gestión de cobros
  
•	El sistema deberá permitir el registro de pagos realizados. 

•	El sistema deberá almacenar información del pago (fecha, monto, tipo de ingreso, contribuyente, descripción). 

•	El sistema deberá permitir la clasificación de los ingresos por tipo. 

•	El sistema deberá evitar la duplicación de registros de pago. 

- Generación de recibos
  
•	El sistema deberá generar recibos digitales automáticamente al registrar un pago. 

•	El sistema deberá permitir la descarga o impresión de recibos. 

•	El sistema deberá incluir en el recibo los datos del contribuyente, monto, fecha y concepto. 

- Consulta y control de ingresos
  
•	El sistema deberá permitir la consulta del historial de pagos. 

•	El sistema deberá permitir la búsqueda de pagos por fecha, contribuyente o tipo de ingreso. 

•	El sistema deberá mostrar el historial completo de ingresos registrados. 

- Reportes
  
•	El sistema deberá generar reportes de ingresos (diarios, mensuales, anuales). 

•	El sistema deberá permitir la exportación de reportes (PDF o Excel). 

•	El sistema deberá mostrar estadísticas básicas de ingresos. 

- Panel de control
  
•	El sistema deberá mostrar un panel con indicadores clave (total de ingresos, pagos recientes, etc.). 

•	El sistema deberá actualizar la información del panel en tiempo real o bajo demanda


## Requerimientos no funcionales

- Seguridad
  
•	El sistema deberá garantizar la confidencialidad de la información mediante autenticación con JWT. 

•	El sistema deberá encriptar las contraseñas de los usuarios. 

•	El sistema deberá restringir el acceso según roles (administrador y cajero).

- Rendimiento
  
•	El sistema deberá responder a consultas en un tiempo menor a 2 segundos. 

•	El sistema deberá soportar múltiples usuarios simultáneos sin degradación significativa.

- Disponibilidad
  
•	El sistema deberá estar disponible durante el horario laboral sin interrupciones. 

•	El sistema deberá contar con mecanismos de respaldo (backups) periódicos.

- Usabilidad
  
•	El sistema deberá contar con una interfaz intuitiva y fácil de usar. 

•	El sistema deberá ser accesible desde navegadores web modernos.

- Integridad de datos

•	El sistema deberá evitar la pérdida de información. 

•	El sistema deberá mantener consistencia en los datos almacenados.

- Escalabilidad
  
•	El sistema deberá permitir futuras mejoras o ampliaciones sin afectar su funcionamiento.

- Mantenibilidad
  
•	El sistema deberá estar desarrollado con código estructurado y documentado.


## Metodología de desarrollo de software

## Fases del desarrollo del sistema

## Modelo Scrum

- Diagramas UML
  
![uml](https://github.com/AlmaPeredaV/IMPLAN-Proyect/blob/main/Diagramas_UML.md)

- Diseño
- Tablero
## Fase de desarrollo

## Pruebas y resultados
