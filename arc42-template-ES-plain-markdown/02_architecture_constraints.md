# 2. Restricciones de Arquitectura

## 2.1 Restricciones Tecnológicas

Para el desarrollo del sistema ERP se definieron las siguientes decisiones tecnológicas, las cuales establecen las restricciones de la arquitectura del proyecto.

### Backend

El backend será desarrollado utilizando **.NET 8** con **ASP.NET Core Web API**, implementando una arquitectura por capas que facilite el mantenimiento, la escalabilidad y la integración con otros módulos del ERP.

### Frontend

La interfaz de usuario será desarrollada como una **Single Page Application (SPA)** utilizando **Angular**, permitiendo una experiencia de usuario dinámica, una comunicación eficiente mediante APIs REST y una estructura modular para el crecimiento del sistema.

### Base de Datos

Se utilizará **PostgreSQL** como sistema gestor de bases de datos relacional debido a su alto rendimiento, estabilidad, soporte para transacciones y facilidad de despliegue tanto en entornos locales como en la nube. Además, representa una alternativa de bajo costo ideal para un Producto Mínimo Viable (MVP), permitiendo escalar el sistema conforme aumenten las necesidades del negocio.

---

## 2.2 Restricciones de Arquitectura

- La comunicación entre el frontend y el backend se realizará mediante servicios **REST** sobre **HTTPS**.
- La persistencia de la información se gestionará exclusivamente mediante PostgreSQL.
- El sistema deberá ser modular para facilitar la incorporación de nuevos módulos del ERP en futuras versiones.
- La arquitectura deberá permitir la integración con servicios externos, como facturación electrónica y sistemas de afiliados.
- La solución deberá ser desplegable tanto en entornos locales como en proveedores de nube pública.

---

## 2.3 Restricciones de Desarrollo

- Se utilizará **Git** como sistema de control de versiones.
- El desarrollo seguirá una metodología ágil basada en Scrum.
- El código deberá cumplir estándares de buenas prácticas, favoreciendo la mantenibilidad y reutilización.
- Las APIs deberán documentarse mediante OpenAPI (Swagger).