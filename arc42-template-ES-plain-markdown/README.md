# ERP Software Architecture

## Descripción

Este repositorio contiene la documentación de arquitectura del **Módulo de Compras** de un sistema **ERP (Enterprise Resource Planning)**, desarrollada como parte del taller de documentación utilizando la plantilla **arc42**.

La arquitectura propuesta está basada en una aplicación web con:

- **Frontend:** Angular (SPA)
- **Backend:** ASP.NET Core (.NET 8 Web API)
- **Base de Datos:** PostgreSQL
- **Plataforma de despliegue:** Microsoft Azure

La documentación describe los objetivos del sistema, las decisiones arquitectónicas, el contexto, la estructura de la solución, los diagramas de arquitectura y el glosario de términos del dominio.

---

## Documentación

| Documento | Descripción |
|-----------|-------------|
| [01. Introducción y Objetivos](./01_introduction_and_goals.md) | Presenta el objetivo del sistema y los principales requisitos de negocio del módulo. |
| [02. Restricciones de Arquitectura](./02_architecture_constraints.md) | Describe las tecnologías y restricciones que condicionan la arquitectura. |
| [03. Alcance y Contexto](./03_system_scope_and_context.md) | Incluye el diagrama de contexto (C1) y el alcance del sistema. |
| [05. Vista de Bloques de Construcción](./05_building_block_view.md) | Presenta el diagrama de contenedores (C2) y la responsabilidad de cada contenedor. |
| [06. Vista de Ejecución](./06_runtime_view.md) | Describe el flujo de ejecución para el registro de una entrega de mercancía. |
| [07. Vista de Despliegue](./07_deployment_view.md) | Muestra la arquitectura de despliegue propuesta sobre Microsoft Azure. |
| [10. Glosario](./10_glossary.md) | Define los principales conceptos del dominio y términos técnicos utilizados en la documentación. |

---

## Tecnologías

- Angular
- ASP.NET Core (.NET 8)
- PostgreSQL
- REST API
- Microsoft Azure
- PlantUML
- Markdown
- arc42

---

## Estructura del Proyecto

```text
ERP-SOFTWARE-ARCHITECTURE/
│
├── images/
├── docs/
├── 01_introduction_and_goals.md
├── 02_architecture_constraints.md
├── 03_system_scope_and_context.md
├── 05_building_block_view.md
├── 06_runtime_view.md
├── 07_deployment_view.md
├── 10_glossary.md
├── README.md
└── diagrams/
```

---

## Autor

**José Danilo Santos Serrato**

Taller 2 de arquitectura de software utilizando la plantilla **arc42**.