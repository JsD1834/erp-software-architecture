# 7. Vista de Despliegue (Deployment View)

## 7.1 Estrategia de Despliegue

La solución será desplegada sobre **Microsoft Azure**, utilizando servicios administrados que permitan una implementación sencilla, alta disponibilidad y facilidad de mantenimiento.

La arquitectura estará compuesta por tres componentes principales:

- Un servicio para alojar la aplicación web desarrollada en Angular.
- Un servicio para alojar la API REST desarrollada con ASP.NET Core.
- Un servicio administrado de PostgreSQL para el almacenamiento persistente de la información.

El siguiente diagrama muestra la distribución de los componentes dentro de la infraestructura de Azure.

---

## 7.2 Componentes del Despliegue

### Azure App Service (Frontend)

Hospeda la aplicación web desarrollada en **Angular**. Este servicio entrega la interfaz de usuario a través de HTTPS y permite que los usuarios interactúen con el sistema ERP desde un navegador web.

### Azure App Service (Backend)

Hospeda la **API REST desarrollada con ASP.NET Core (.NET 8)**. Es responsable de procesar las solicitudes del frontend, aplicar las reglas de negocio, gestionar la autenticación y comunicarse con la base de datos.

### Azure Database for PostgreSQL - Flexible Server

Servicio administrado encargado del almacenamiento persistente de la información del ERP. Proporciona alta disponibilidad, copias de seguridad automáticas, escalabilidad y seguridad administrada por Azure.

---

## 7.3 Flujo de Despliegue

1. El usuario accede al sistema mediante un navegador web.
2. Azure App Service entrega la aplicación Angular.
3. La aplicación Angular consume la API REST mediante HTTPS.
4. La API procesa la solicitud y realiza las operaciones correspondientes.
5. La API consulta o actualiza la información almacenada en Azure Database for PostgreSQL.
6. Finalmente, la respuesta es enviada al frontend para ser presentada al usuario.