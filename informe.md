
# Empresa de Construcción Civil y Presupuestos de Obras 

# “HOME EASY”
# (Grupo5)








### Matias Espinoza – Analista 
### Carlos Muñoz – Implementador
### Claudio Castillo – Evaluador
### Christopher Espinoza - Docente
 
# INDICE

• Objetivo del Informe

• Descripción del Proyecto

• Estructura del Informe

• Requisitos Funcionales

• Requisitos No Funcionales

## Diseño Seguro

• Arquitectura de la Aplicación

• Medidas de Seguridad Propuestas

## Plan de Implementación

• Análisis y requisitos

• Diseño

• Desarrollo

• Pruebas y Validación

• Despliegue

• Mantenimiento

## Asignación de Roles y Responsabilidades

• Roles Específicos del Equipo

• Responsabilidades de Cada Rol

## Conclusión

• Resumen del Informe

• Beneficios del Enfoque de Seguridad Propuesto

## Objetivo de informe

El objetivo de este informe es presentar un análisis detallado de los requisitos de seguridad, así como una propuesta de diseño seguro para una aplicación web que gestionará proyectos de construcción. Esta aplicación incluirá la elaboración de presupuestos, control de inventario de materiales, seguimiento de tareas y comunicación con clientes.

## Descripción del proyecto

Este proyecto se basa en el caso de estudio asignado al Grupo 5, compuesto por Matías Espinoza (Analista), Carlos Muñoz (Implementador) y Claudio Castillo (Evaluador). El propósito es desarrollar una aplicación web segura y eficiente para la gestión integral de proyectos de construcción.
  
<img src="imagenes/PAGINAHOME.png.jpg" />

<img src="imagenes/PAGINAINVENTARIO.png.jpg" />





## Estructura del informe

El informe se estructura en varias secciones clave: cronología del proyecto, diseño seguro, plan de implementación, asignación de roles y responsabilidades, y conclusión. Cada sección aborda aspectos específicos del desarrollo y seguridad de la aplicación.

## Requisitos funcionales

Todo analista de plataformas web es importante que recopile y analice una amplia gama de información para diseñar una plataforma que cumpla con los criterios de seguridad requeridos así también Comprender y alinear los objetivos y metas del proyecto con las necesidades de seguridad. Hay que asegurar que la plataforma cumpla con los estándares más altos de seguridad para proteger la información y los procesos críticos de la organización.

1.	Gestión de Proyectos:

Crear, editar y eliminar proyectos de construcción.

Asignar tareas y recursos a proyectos específicos.

2.	Elaboración de Presupuestos:

Crear, editar y eliminar presupuestos para proyectos.

3.	Control de Inventario:

Gestionar el inventario de materiales de construcción.

Registrar entradas y salidas de inventario.

4.	Comunicación con Clientes:

Enviar y recibir mensajes entre contratistas, clientes y proveedores.

Compartir documentos y planos de proyectos.

## Requisitos no funcionales

1.	Seguridad:

Autenticación y autorización de usuarios.

Protección de datos sensibles mediante cifrado.

Auditoría y registro de actividades de los usuarios.

2.	Rendimiento:

Tiempo de respuesta aceptable (< 2 segundos) para la mayoría de las operaciones.

Escalabilidad para manejar múltiples proyectos y usuarios simultáneamente.

3.	Usabilidad:

Interfaz de usuario intuitiva y fácil de usar.

Accesibilidad para personas con discapacidades.

4.	Mantenibilidad:

Código modular y bien documentado.

Capacidad de actualizar y mantener el sistema sin interrupciones significativas.

En esta parte del documento se tratará sobre una implementación lo más segura posible, la integración de prácticas de seguridad en el inicio del proyecto es importante, ya que esto puede prevenir vulnerabilidades y así poder identificar de manera temprana estas, esto se recomienda para poder detectar las falencias de forma prematura y no cuando ya está el proyecto casi finalizado.



# Diseño seguro

Se implementará el protocolo de comunicación https ya que esta tecnología utiliza SSL/TLS para cifrar los datos entre el usuario y el servidor, la información personal está protegida y no puede ser interceptada ni leída por terceros mientras transita por la red de internet
Una gestión segura de contraseñas, codificar para que sean textos más largos y complejos que incluyan mayúsculas, minúsculas, símbolos especiales y números como por ejemplo (ConsTruccion15@Civil), otra opción sería un generador de contraseñas.
Control de acceso restringido para usuarios, para que solo tengan acceso a ciertos recursos (ejemplo: control total para administrador de la página y restringido para usuarios)
Tener un sistema de filtración de correos electrónicos, como por ejemplo tener una lista negra actualizada de dominios y correos asociados a actividades de pishing.

## Capas de la Aplicación:
Presentación: Interfaz de usuario basada en web.

Lógica de Negocio: Procesamiento y reglas de negocio.

Acceso a Datos: Gestión de bases de datos y almacenamiento de datos.

## Medidas de seguridad propuestas
1.	Autenticación y Autorización:
	Roles y permisos definidos para clientes y administradores.

2.	Protección de Datos:
	Cambio de contraseñas cada 30dias con requisitos de 7 caracteres y con uso de mayúsculas, minúsculas, dígitos numéricos y símbolo.

3.	Control de Acceso:
	Implementación de controles de acceso basados en roles (RBAC).
	Verificación de permisos antes de acceder a recursos sensibles.

4.	Validación de Datos:
	Validación de entradas del usuario en el cliente y el servidor.
	Prevención de inyecciones SQL mediante el uso de consultas parametrizadas.

5.	Pruebas de Seguridad:
	Pruebas de penetración para identificar y mitigar vulnerabilidades.
	Escaneo regular de vulnerabilidades y parches de seguridad.

6.	Auditoría y Monitoreo:
	Registro detallado de actividades del usuario y eventos del sistema.
	Monitoreo en tiempo real y alertas de seguridad.
    Validación de datos de entrada, como por ejemplo que nombre de usuario tenga mínimo 5 caracteres y máximo 20, el correo valide el “@” y la contraseña acepte un mínimo de 8 caracteres

Como por ejemplo:
<p align="center">
<img src="./imagenes/imagen1.jpg">
</p>



Parámetros para consulta SQL para mejorar seguridad y eficiencia de la consulta de la base de datos, para tratar de evitar inyección SQL

como por ejemplo:
<p align="center">
<img src="./imagenes/imagen2.jpg">
</p>

# Plan de implementación 
## Análisis y requisitos
•   Reunión inicial para definir y documentar requisitos de seguridad.

•   Entrevistas con partes interesadas para entender necesidades 
específicas.

## Diseño
•	Diseño de la arquitectura segura de la aplicación.

•	Elaboración de diagramas de flujo y casos de uso.

## Desarrollo
•	Implementación del código siguiendo prácticas de codificación segura.

•	Revisión y auditoría de código por pares.

## Pruebas y validacion
•	Ejecución de pruebas unitarias y de integración.

•	Pruebas de seguridad y validación de requisitos.

## Despliegue
•	Configuración del entorno de producción seguro.

•	Despliegue gradual y monitoreo post-implementación.

## Mantenimiento
•	Actualizaciones regulares y parches de seguridad.

•	Monitoreo continuo y respuesta a incidentes.

## Responsabilidades de cada rol:
## Analista:
•	Realizar el análisis de requisitos del caso de estudio.

•	Identificar los requisitos de seguridad funcionales y no funcionales.

•	Colaborar en la elaboración del diseño seguro.

## Implementador:
•	Proponer y desarrollar la solución segura en la implementación.

•	Aplicar técnicas de codificación seguras.

•	Documentar el proceso de implementación y prácticas seguras utilizadas.

## Evaluador:
•	Revisar y validar el diseño y la implementación desde la perspectiva de seguridad.

•	Realizar pruebas de seguridad exhaustivas.

•	Documentar las pruebas realizadas y los resultados obtenidos.


## Medidas de seguridad implementadas
En el diseño de la aplicación "HOME EASY", se han propuesto diversas medidas de seguridad para garantizar la protección integral de datos y la confiabilidad operativa. Una de las principales medidas incluidas es la implementación del protocolo HTTPS, utilizando SSL/TLS para cifrar la comunicación entre usuarios y el servidor. Esto asegura que los datos sensibles, como información personal y detalles de proyectos, estén protegidos contra accesos no autorizados y ataques de interceptación.

Además, se ha diseñado un sistema de gestión de contraseñas robusto, que promueve el uso de contraseñas complejas y la rotación periódica de las mismas. Esto incluye requisitos estrictos como la inclusión de caracteres alfanuméricos, símbolos especiales y una longitud mínima, asegurando que las credenciales de acceso sean difíciles de vulnerar mediante fuerza bruta u otros métodos de ataque.

Para controlar el acceso a recursos sensibles dentro de la aplicación, se ha implementado un modelo de control de acceso basado en roles (RBAC). Este enfoque permite asignar permisos específicos a usuarios y administradores según sus funciones dentro del sistema, asegurando que solo tengan acceso a la información y funcionalidades necesarias para realizar sus tareas autorizadas.

Otra medida crítica es la validación exhaustiva de datos de entrada en ambos lados, cliente y servidor, para prevenir vulnerabilidades como las inyecciones SQL. Este enfoque ayuda a mitigar riesgos desde el principio del desarrollo, asegurando que los datos manipulados por la aplicación sean válidos y seguros en todo momento.

Para garantizar la efectividad de estas medidas, se llevarán a cabo pruebas continuas de seguridad, incluyendo pruebas de penetración y escaneo regular de vulnerabilidades. Esto no solo permite identificar posibles puntos débiles en el sistema, sino que también facilita la implementación oportuna de parches de seguridad y actualizaciones necesarias para mantener la aplicación protegida contra las últimas amenazas cibernéticas.

## Revisión del Diseño:
  Usando principalmente la ayuda de la herramienta de escaneo NESSUS se pudo  realizar una exitosa  prueba de ciberseguridad en la empresa usando el siguiente plan:

1. Arquitectura de Seguridad:
   - Se logro revisar la arquitectura general de la aplicación web para asegurar de que sigue prácticas recomendadas en seguridad web.

   - Verifique la separación adecuada entre el front-end y el back-end para minimizar el riesgo de ataques como XSS (Cross-Site Scripting) y CSRF (Cross-Site Request Forgery).

2. Autenticación y Autorización:
   - Confirmar que los mecanismos de autenticación (inicio de sesión) sean robustos y estén protegidos contra ataques de fuerza bruta y diccionario.

   - Revisar los controles de autorización para asegurar que los usuarios solo tengan acceso a las funciones y datos que les corresponden.


3. Protección de Datos Sensibles:
   - Asegurar de que la información sensible, como datos de pago y datos personales de los usuarios, esté cifrada durante la transmisión y el almacenamiento.

   - Implementar políticas de manejo de datos para cumplir con regulaciones de privacidad (como GDPR, CCPA).

4. Seguridad del Cliente:
   - Verificar que la interfaz de usuario no sea vulnerable a ataques como manipulación de URL, inyección de código o redirecciones no autorizadas.

5. Seguridad de APIs:
   - Asegurar que si la página web utiliza APIs para integrarse con sistemas externos, y de que estas APIs estén protegidas contra accesos no autorizados y abusos.

   

 ## Revisión de la Implementación:

1. Pruebas de Penetración:
   - Realizar pruebas de penetración para identificar vulnerabilidades en la aplicación web. Esto puede incluir escaneos de vulnerabilidades automatizados y pruebas manuales.

2. Código Seguro:
   - Revisar el código fuente para asegurarte de que se sigan las mejores prácticas de desarrollo seguro, como la validación adecuada de entradas, la prevención de inyecciones SQL y la sanitización de datos.

3. Actualizaciones y Parches
   - Asegurar de que todos los componentes de software utilizados (sistema operativo, servidor web, frameworks, bibliotecas) estén actualizados con las últimas correcciones de seguridad.

4. Monitoreo y Registro
   - Implementar mecanismos de monitoreo para detectar actividad sospechosa y eventos de seguridad.

   - Configurar registros (logs) detallados de la actividad del sistema para facilitar la auditoría y la respuesta ante incidentes.

## Validación y Auditoría:

1. Auditoría de Seguridad:
   - Considerar contratar a expertos externos para realizar una auditoría de seguridad independiente.

   - Realizar auditorías internas periódicas para asegurarme de que se mantienen los estándares de seguridad.

2. Pruebas de Continuidad del Negocio:
   - Probrar los planes de continuidad del negocio y de recuperación ante desastres para garantizar que la página web pueda recuperarse rápidamente de incidentes de seguridad.

3. Formación y Concientización:
   - Capacitar a los empleados y desarrolladores sobre las mejores prácticas de seguridad y la importancia de proteger los datos de los usuarios.

Implementar estas prácticas ayudará a mejorar la seguridad de la página web que ofrece servicios de venta de hormigón y materiales para la construcción, reduciendo así el riesgo de vulnerabilidades y protegiendo la información confidencial de los usuarios y la empresa.

Finalmente, se enfatiza la importancia de la educación y capacitación continua de usuarios y personal técnico. Programas de concienciación en seguridad aseguran que todos los usuarios comprendan y apliquen las mejores prácticas de seguridad en sus interacciones diarias con la aplicación, fortaleciendo aún más la protección global del sistema.

# Conclusión 
Resumen de informe
El análisis y diseño presentado en este informe proporciona una base sólida para el desarrollo seguro de una aplicación web
 para la gestión de proyectos de construcción. Al implementar las medidas de seguridad propuestas y seguir un plan de implementación
riguroso, se garantiza que la aplicación será segura, eficiente y confiable para todos los usuarios.
