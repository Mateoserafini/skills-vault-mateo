# 🚀 Stack Skills Template (.agents/skills)

Plantilla modular y estandarizada de **Skills para Antigravity / Claude Agentic Workflows**, optimizada específicamente para proyectos con stack **React, TypeScript, Node.js, Express, MongoDB y SQL**.

Esta plantilla permite dotar a los agentes de IA de directrices técnicas de alto nivel, patrones de diseño probados y reglas estrictas de desarrollo para acelerar el ciclo de vida del software manteniendo la máxima calidad de código.

---

## 📁 Estructura del Repositorio

```text
stack-skills-template/
├── .agents/
│   └── skills/
│       ├── api-design-principles/
│       ├── bash-pro/
│       ├── code-refactoring-refactor-clean/
│       ├── database-architect/
│       ├── frontend-developer/
│       ├── nodejs-backend-patterns/
│       ├── seo-meta-optimizer/
│       ├── sql-pro/
│       ├── tailwind-design-system/
│       ├── typescript-pro/
│       └── ui-ux-pro-max/
└── README.md
```

---

## 🗂️ Índice y Clasificación de las 11 Skills

Las 11 skills incluidas se dividen en 4 categorías estratégicas:

| Categoría | Skill | Descripción Breve |
| :--- | :--- | :--- |
| **Frontend / UI** | `frontend-developer` | Arquitectura moderna en React y TypeScript, hooks y manejo de estado. |
| **Frontend / UI** | `ui-ux-pro-max` | Inteligencia de diseño UI/UX completa (sistemas de color, tipografía, accesibilidad, GSAP y heurísticas). |
| **Frontend / UI** | `tailwind-design-system` | Sistemas de diseño atómicos con Tailwind CSS, dark mode y tokens consistentes. |
| **Frontend / UI** | `seo-meta-optimizer` | Optimización técnica de SEO, Open Graph, meta tags y Core Web Vitals. |
| **Backend / API** | `nodejs-backend-patterns` | Patrones de arquitectura limpia, middlewares, servicios y gestión asíncrona en Node.js y Express. |
| **Backend / API** | `api-design-principles` | Especificación y diseño de APIs RESTful robustas, contratos HTTP semánticos y validación. |
| **Backend / API** | `typescript-pro` | Tipado estático avanzado, contratos de datos API/BD, genéricos y seguridad en tipos sin `any`. |
| **Base de Datos** | `database-architect` | Modelado y diseño de datos relacionales y documentales (MongoDB con Mongoose y SQL). |
| **Base de Datos** | `sql-pro` | Consultas SQL de alto rendimiento, índices, transacciones ACID y migraciones. |
| **Utilitarios** | `code-refactoring-refactor-clean` | Clean Code, principios SOLID, desacoplamiento y detección de code smells. |
| **Utilitarios** | `bash-pro` | Automatización de scripts de terminal, tooling de entorno y pipelines. |

---

## ⚙️ Resumen Funcional Aplicado a tu Stack

### 1. Frontend & UI (React + Tailwind + TypeScript)
- **`frontend-developer`**: Guía al agente en la creación de componentes modulares en React, separación de lógica de presentación mediante Custom Hooks, optimización de re-renderizados con `useMemo`/`useCallback` y control estricto del ciclo de vida del componente.
- **`ui-ux-pro-max`**: Proporciona al agente un catálogo exhaustivo de 119 reglas de UX, 79 estilos visuales, paletas de colores armónicas y estándares WCAG de accesibilidad (contraste 4.5:1, navegación por teclado, áreas táctiles de 44px). Garantiza que las interfaces creadas no luzcan como plantillas genéricas.
- **`tailwind-design-system`**: Estandariza el uso de Tailwind CSS evitando clases caóticas o arbitrarias. Establece jerarquías de espaciado, variantes responsivas (`sm`, `md`, `lg`), tokens semánticos de color y soporte de tema oscuro (`dark:`).
- **`seo-meta-optimizer`**: Asegura que cada vista en React cuente con la jerarquía semántica correcta (un solo `<h1>`, etiquetas `meta`, Open Graph, Twitter Cards y atributos `alt` en imágenes) para indexación y visibilidad web óptima.

### 2. Backend & APIs (Node.js + Express + TypeScript)
- **`nodejs-backend-patterns`**: Modela la arquitectura backend en capas desacopladas (Controllers -> Services -> Repositories/Models). Estandariza el manejo centralizado de errores con middlewares globales, control de promesas asíncronas y logging estructurado.
- **`api-design-principles`**: Define contratos de endpoints REST limpios: uso estricto de verbos HTTP (`GET`, `POST`, `PUT`, `PATCH`, `DELETE`), códigos de estado semánticos (`200`, `201`, `400`, `401`, `403`, `404`, `500`), paginación consistente (`cursor` o `offset/limit`) y validación de esquemas (e.g. Zod o Joi).
- **`typescript-pro`**: Eleva la robustez técnica en todo el stack. Guía la definición de tipos discriminados, DTOs de solicitud/respuesta compartidos entre cliente y servidor, inferencia de tipos sobre modelos de base de datos y erradicación del uso de `any`.

### 3. Persistencia & Datos (MongoDB + SQL)
- **`database-architect`**: Ayuda a definir cuándo desnormalizar en esquemas de colecciones de MongoDB (Mongoose) para alto rendimiento de lectura, o cómo estructurar relaciones normalizadas en esquemas SQL (1:N, N:M), claves foráneas y restricciones de integridad.
- **`sql-pro`**: Se enfoca en la optimización de queries SQL complejas, creación estratégica de índices (`B-Tree`, compuestos), prevención de bloqueos, gestión de transacciones atómicas (`BEGIN...COMMIT`) y redacción de scripts de migración confiables.

### 4. Calidad & Tooling
- **`code-refactoring-refactor-clean`**: Aplica refactorización segura y continua según principios SOLID y Clean Architecture. Detecta funciones excesivamente largas, acoplamiento alto o deuda técnica y propone desgloses limpios sin alterar la funcionalidad externa.
- **`bash-pro`**: Automatiza tareas repetitivas en terminal: scripts de inicialización de base de datos, preparación de variables de entorno `.env`, comprobaciones previas a commit (`pre-commit`) y comandos de despliegue local o CI/CD.

---

## 📥 Integración en Nuevos Proyectos

Puedes integrar esta suite de skills en cualquier proyecto nuevo mediante cualquiera de los siguientes métodos:

### Método 1: Como Submódulo de Git (Recomendado para sincronización centralizada)
Si subes este repositorio a tu GitHub (por ejemplo: `https://github.com/TU_USUARIO/stack-skills-template.git`), puedes vincular las skills directamente a la carpeta `.agents/skills` de cualquier proyecto existente:

```bash
# 1. Dentro de la raíz de tu nuevo proyecto (que ya debe ser un repositorio Git):
git submodule add https://github.com/TU_USUARIO/stack-skills-template.git .agents/skills

# 2. Inicializar y actualizar el submódulo:
git submodule update --init --recursive
```

*Cuando hagas mejoras a tus skills en la plantilla central, podrás actualizarlas en tus proyectos con:*
```bash
git submodule update --remote --merge
```

---

### Método 2: Clonado Directo y Copia Local (Para personalización independiente por proyecto)
Si prefieres que cada proyecto tenga su copia aislada sin ataduras a Git:

#### En Windows (PowerShell):
```powershell
# Clona temporalmente en tu proyecto
git clone --depth 1 https://github.com/TU_USUARIO/stack-skills-template.git temp-skills

# Copia la carpeta .agents a la raíz de tu proyecto
Copy-Item -Recurse -Force temp-skills\.agents .

# Elimina el clon temporal
Remove-Item -Recurse -Force temp-skills
```

#### En Linux / macOS / Git Bash:
```bash
git clone --depth 1 https://github.com/TU_USUARIO/stack-skills-template.git temp-skills
cp -r temp-skills/.agents .
rm -rf temp-skills
```

---

## 🗑️ Cómo Desactivar o Eliminar Skills en un Proyecto

El motor de Antigravity descubre automáticamente las skills inspeccionando la carpeta `.agents/skills/`.

> **Regla de modularidad:** Para desactivar o eliminar una skill de un proyecto específico, **basta con borrar su carpeta individual**.

Por ejemplo, si un proyecto no utiliza SQL o no requiere scripts de terminal, simplemente elimina esas carpetas:

```powershell
# Ejemplo en PowerShell para desactivar sql-pro y bash-pro:
Remove-Item -Recurse -Force .agents\skills\sql-pro
Remove-Item -Recurse -Force .agents\skills\bash-pro
```

```bash
# Ejemplo en Bash:
rm -rf .agents/skills/sql-pro
rm -rf .agents/skills/bash-pro
```

Una vez eliminada la carpeta, el agente dejará de cargar sus instrucciones y directrices en futuras interacciones, sin afectar en absoluto a las demás skills activas.
