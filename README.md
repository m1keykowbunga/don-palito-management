# :spades: 🚦 💹 REPOSITORIO DE GESTIÓN: 
## Proyecto Don Palito JR

Este directorio está diseñado para **gestionar y vigilar el flujo de desarrollo** del proyecto **Don Palito JR**.

**Este NO es un repositorio de código fuente.** Su propósito principal es alojar la configuración, las plantillas y la documentación necesaria para asegurar un desarrollo trazable, estandarizado y de alta calidad.

---

## 🎯 Misión del Repositorio

Nuestra misión principal es implementar una metodología **Scrumban** efectiva, garantizando que todo el trabajo (tanto Web como Móvil) esté:

1.  **Trazable:** Cada tarea se vincula directamente a un requisito formal (IEEE 830).
2.  **Estandarizado:** Uso obligatorio de plantillas para Bug, Feature y Spike.
3.  **Verificado:** Implementación de la Integración Continua (CI) obligatoria antes de la revisión humana.

---

## ⚙️ Estructura de Gobernanza

La gestión del proyecto se basa en la carpeta **`.github/`**, que activa las siguientes herramientas:

| Directorio / Archivo | Función Principal | Rol en el Flujo de Trabajo |
| :--- | :--- | :--- |
| **`.github/ISSUE_TEMPLATE/`** | **Flujo de Tareas** | Activa las plantillas (`adm-Task`, `Bug`, `Spike`, `feature-Task`) en la pestaña **Issues**. |
| **`.github/PULL_REQUEST_TEMPLATE.md`** | **Control de Calidad (DoD)** | Activa el Checklist de *Definition of Done* en cada revisión de código. |
| **`.github/workflows/ci.yml`** | **Automatización** | Ejecuta las pruebas paralelas de las plataformas **Web (JS)** y **Móvil (RN/Android)**. |

---

## 🤖 Tecnologías Principales del Proyecto (Don Palito JR)

El proyecto integra múltiples tecnologías, separadas en repositorios distintos para un desarrollo modular.

| Área | Tecnología / Entorno | Descripción | Repositorio Relacionado |
| :--- | :--- | :--- | :--- |
| **Frontend Web** | HTML, CSS, JavaScript, React | Plataforma web de **e-commerce principal**, incluyendo el catálogo de productos y el panel de administrador. | `don-palito-web` |
| **Frontend Móvil** | React Native, Android Studio | Aplicación móvil enfocada en la **gestión de pedidos, inventario** y **trazabilidad de entregas** (Logística). | `don-palito-mobile` |
| **Backend / Servidor** | FastAPI (Python) | **API REST principal** para la lógica de negocio, manejo de *stock*, carrito de compras, autenticación y base de datos. | `don-palito-api` |

---


### 🗂️ Estructura de Directorios del Repositorio de Gestión 

| Tipo | Directorio/Archivo | Propósito (Comentarios) |
| :--- | :--- | :--- |
| **Repositorio** | `📦 Repositorio-Documentacion-IPATD` | Raíz del repositorio de gobernanza y gestión. |
| **General** | `📄 README.md` | Descripción general del repositorio (este archivo). |
| **General** | `📄 CONTRIBUTING.md` | Guía de contribución y estándares de documentación. |
| **Gestión** | `📁 .github/` | Contiene toda la configuración del flujo de trabajo de GitHub (Kanban/CI). |
| **Documentación** | `📁 docs/` | Carpeta principal para toda la documentación formal del proyecto. |
| **Docs** | `├── 📁 mobile/` | Documentación técnica específica del módulo móvil (React Native / Android Studio). |
| **Docs** | `├── 📁 web/` | Documentación técnica específica del módulo web (React + e-commerce). |
| **Docs** | `├── 📁 backend/` | Documentación técnica específica del *backend* (FastAPI). |
| **Docs** | `├── 📁 arquitectura/` | Diagramas, modelos UML, y estructura del sistema (ADRs, PlantUML). |
| **Docs** | `├── 📁 requisitos/` | Listado y detalle de requisitos funcionales y no funcionales (IEEE 830 / SRS). |
| **Docs** | `├── 📁 testing/` | Planes, casos de prueba y reportes de pruebas (QA). |
| **Docs** | `└── 📁 mantenimiento/` | Documentos de soporte y mantenimiento del sistema. |

---

## 📋 Gestión de tareas y Kanban

El **tablero Kanban de GitHub** es la herramienta principal para gestionar las tareas asociadas a los requisitos.  
Cada **requisito funcional o módulo** se representa mediante una **Issue**, la cual atraviesa las siguientes etapas:

| Columna del Tablero | Color de GitHub Projects | Descripción |
| :--- | :--- | :--- |
| 🟢 **Backlog** | _Verde_ | Requisitos, ideas o tareas que están pendientes de definición y priorización. |
| 🔵 **Ready** | _Azul_ | Tareas priorizadas y listas para ser tomadas por un desarrollador. |
| 🟡 **In Progress** | _Amarillo_ | Tareas en desarrollo activo o en proceso de análisis/implementación. |
| 🟣 **In Review** | _Morado_ | Tareas completadas que esperan **validación técnica** (Pull Request) o **revisión funcional**. |
| 🟠 **Done** | _Naranja_ | Requisitos o tareas finalizadas, implementadas y aprobadas. El ciclo está cerrado. ||

### 🔖 Convención de etiquetas (labels)

| Etiqueta | Descripción |
|-----------|--------------|
| `frontend-web` | Tareas relacionadas con la interfaz web. |
| `frontend-mobile` | Tareas del módulo móvil. |
| `backend` | Desarrollo o integración del servidor. |
| `documentacion` | Actualización o creación de documentación. |
| `alta-prioridad` | Requisito crítico o dependiente de otros. |
| `bajo-esfuerzo` | Tareas simples o de baja complejidad. |

---

## 🧠 Metodología de trabajo

El desarrollo del proyecto se rige bajo los principios de **Scrum**, utilizando iteraciones cortas (sprints) y priorización mediante **Planning Poker**.

Cada historia o requisito es evaluado con base en su:

- **Nivel de esfuerzo** (Bajo, Medio, Alto)  
- **Puntos de historia (Story Points)**  
- **Rol responsable** (Backend, Frontend Web, Móvil, Liderazgo/PO)

Estos valores se reflejan en la hoja de **Priorización y Dificultad**, y son usados para estimar tiempos y planificar sprints.

---

## 🧾 Lineamientos para la documentación

Cada subdirectorio dentro de `/docs` debe contener:

1. **README.md** específico para su módulo (por ejemplo, `/docs/backend/README.md`).  
2. **Documentos técnicos** (diagramas, esquemas, manuales o reportes).  
3. **Formato estandarizado** de documentación en Markdown o PDF.  
4. **Historial de cambios** o actualizaciones relevantes.

---

## 🤝 Contribución y roles

Cada integrante del equipo debe:

1. Crear su rama de trabajo (`feature/<nombre_modulo>`).  
2. Asociar cada commit a la issue correspondiente.  
3. Mover la tarjeta en el tablero Kanban según el progreso.  
4. Mantener actualizada la documentación del módulo en `/docs`.

---
## 🏁  Cómo Empezar a Trabajar

1.  **Crear Tareas:** Ve a la pestaña **Issues** y usa el menú desplegable para seleccionar la plantilla adecuada.
2.  **Verificación:** Todo Pull Request (PR) debe pasar las pruebas automáticas del **`ci.yml`** (estado en **verde**) antes de solicitar la revisión de un compañero.

¡Bienvenido a la gestión profesional de Don Palito!

## 🏗️ Ejemplo de flujo de trabajo

1. **Crear Issue:**  
   “Implementar autenticación en FastAPI (RF-05)”.

2. **Asignar etiquetas:**  
   `backend`, `alta-prioridad`, `medio-esfuerzo`.

3. **Mover al Kanban:**  
   De “Por hacer” → “En progreso”.

4. **Desarrollar y documentar:**  
   Registrar avances en `/docs/backend/RF-05_Autenticacion.md`.

5. **Solicitar revisión:**  
   Mover a “En revisión” y abrir un Pull Request.

---

## 📌 Objetivo final

Este repositorio busca **mantener la trazabilidad total** entre los requisitos, el código y la documentación del proyecto IPATD, asegurando que cada módulo tecnológico evolucione de manera coherente y controlada dentro de una misma estructura estandarizada.

---

**Autor:** Equipo de Desarrollo IPATD  
**Metodología:** Scrum + Kanban (GitHub Projects)  
**Última actualización:** Octubre 2025
