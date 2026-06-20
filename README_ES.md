# AI Product Management Playbook

![AI](https://img.shields.io/badge/AI-Product%20Management-blue)
![Product Management](https://img.shields.io/badge/Product-Management-green)
![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![License](https://img.shields.io/badge/license-MIT-green)

Idioma: Español | English version available at: [README.md](README.md)

---

## Tabla de Contenidos

- [Descripción General](#descripción-general)
- [Estructura del Repositorio](#estructura-del-repositorio)
- [Manejo de Idiomas](#manejo-de-idiomas)
- [Estructura de los Prompts](#estructura-de-los-prompts)
- [Cómo Usar Este Repositorio](#cómo-usar-este-repositorio)
- [Estándares de Documentación](#estándares-de-documentación)
- [Evolución Futura](#evolución-futura)
- [Convención de Commits](#convención-de-commits)
- [Disclaimer](#disclaimer)
- [Inspiración y Recursos](#inspiración-y-recursos)
- [Licencia](#licencia)

---

## Descripción General

Este repositorio es un playbook público de Product Management asistido por IA.

Está diseñado para organizar prompts reutilizables, workflows, plantillas, ejemplos y documentación de soporte para el trabajo práctico de Product Management.

El objetivo es ofrecer un toolkit estructurado y evolutivo que ayude a Product Managers a utilizar IA de forma más consistente en actividades comunes como:

- resúmenes de reuniones
- documentación de producto
- análisis de requerimientos
- generación de PRD
- priorización de roadmap
- estructuración de workflows
- automatización operativa
- futuros agentes de producto asistidos por IA

Más que una colección de prompts, este repositorio busca funcionar como un playbook práctico para aplicar IA a tareas de Product Management de forma repetible y mantenible.

El contenido se desarrolla a partir de experiencia real en Product Management, refinamiento iterativo de prompts y estándares de documentación estructurada.

---

## Estructura del Repositorio

El repositorio está organizado alrededor de herramientas y workflows reutilizables para Product Management.

```text
pm-ai-playbook/
├── README.md
├── README_ES.md
├── LICENSE
├── prompts/
│   ├── general/
│   └── advanced/
│       ├── meeting-minutes/
│       ├── analysis/
│       ├── documentation/
│       └── prioritization/
├── templates/
├── workflows/
├── examples/
└── docs/
```

### prompts

Contiene prompts reutilizables de IA para casos de uso de Product Management.

Los prompts se organizan en dos niveles principales:

- **general/**: prompts standalone diseñados para reutilización directa y flexible.
- **advanced/**: prompts más estructurados que pueden requerir contexto adicional, plantillas, reglas de validación, mayor control de salida o lógica multi-step.

### templates

Contiene plantillas reutilizables de soporte utilizadas por prompts o workflows.

Los ejemplos pueden incluir formatos de reuniones, plantillas de PRD, matrices de priorización u otros artefactos estructurados de producto.

### workflows

Documenta procesos multi-step que combinan prompts, plantillas, ejemplos o criterios de validación para resolver tareas más amplias de Product Management.

### examples

Contiene entradas y salidas de ejemplo utilizadas para probar, validar y demostrar cómo deben usarse los prompts o workflows.

### docs

Contiene documentación interna sobre estructura del repositorio, estándares de prompts, criterios de calidad y principios de diseño.

---

## Manejo de Idiomas

Los prompts de este repositorio se escriben principalmente en inglés para mantener consistencia, mantenibilidad y compatibilidad con la mayoría de herramientas de IA.

Sin embargo, los prompts deben soportar entradas y salidas en múltiples idiomas.

Regla general:

- Entrada en español → salida en español
- Entrada en inglés → salida en inglés

Si se proporciona una plantilla o un formato documental predefinido, el idioma y la estructura original de la plantilla deben mantenerse sin cambios, salvo que el prompt indique explícitamente lo contrario.

Esto permite reutilizar los prompts en diferentes entornos de trabajo sin mantener versiones separadas para cada idioma.

---

## Estructura de los Prompts

Los prompts de este repositorio deben seguir una estructura consistente para mejorar claridad, reutilización y mantenimiento.

La estructura estándar de prompts se define en `docs/prompt-template.md`.

Un prompt normalmente debe incluir:

- Prompt Title
- Purpose
- When to Use
- Inputs
- Language Handling
- Prompt Instructions
- Output Format
- Validation
- Change Log

Esta estructura ayuda a que los prompts sean entendibles, reutilizables y más fáciles de mejorar con el tiempo.

---

## Cómo Usar Este Repositorio

Un flujo típico de uso es:

1. Identificar la tarea de Product Management que se quiere apoyar con IA.
2. Ir a la carpeta correspondiente dentro de `prompts/`.
3. Definir si la tarea requiere un prompt general o un prompt avanzado.
4. Copiar el prompt y proporcionar las entradas requeridas.
5. Utilizar cualquier plantilla de soporte si es necesario.
6. Revisar la salida contra las reglas de validación incluidas en el prompt.
7. Mejorar o adaptar el prompt solo cuando el caso de uso lo requiera.

Los prompts generales son útiles cuando la tarea es flexible y no requiere formato estricto ni plantillas externas.

Los prompts avanzados son útiles cuando la tarea requiere mayor control, una estructura predefinida, validación más fuerte o integración dentro de un workflow más amplio.

---

## Estándares de Documentación

Los estándares y la gobernanza del repositorio se documentan en la carpeta `docs/`.

Los documentos clave incluyen:

- `docs/repository-structure.md` — estructura oficial del repositorio y propósito de cada carpeta.
- `docs/prompt-template.md` — estructura estándar para prompts.
- `docs/prompt-design-principles.md` — principios para crear prompts claros y reutilizables.
- `docs/prompt-quality-checklist.md` — checklist para revisar prompts antes de agregarlos o actualizarlos.

La carpeta `docs/` debe tratarse como el punto de referencia para mantener la consistencia del repositorio a medida que crece.

---

## Evolución Futura

Se espera que este repositorio evolucione más allá de prompts individuales.

Futuras mejoras pueden incluir:

- prompts reutilizables adicionales
- workflows avanzados de Product Management
- ejemplos prácticos basados en entradas realistas
- plantillas reutilizables para artefactos de producto
- frameworks de producto adaptados para trabajo asistido por IA
- agentes estructurados de IA para tareas de Product Management

Los agentes se consideran un área futura de expansión.

Más adelante podrán incluirse en este repositorio si se mantienen estrechamente conectados con prompts y workflows. Si se vuelven más técnicos, configurables o pesados en implementación, podrán gestionarse en un repositorio separado.

El objetivo a largo plazo es construir un playbook práctico de Product Management asistido por IA que pueda ser usado, revisado y extendido por otras personas.

---

## Convención de Commits

Este repositorio utiliza Conventional Commits para mantener un historial de cambios legible y mantenible.

Tipos comunes de commit:

- `feat` — nuevo prompt, workflow, plantilla o contenido funcional.
- `fix` — corrección de un problema.
- `docs` — actualización de documentación.
- `refactor` — mejora estructural sin cambiar la intención principal.
- `chore` — trabajo de mantenimiento.

Ejemplos:

```text
feat: add meeting summary prompt
docs: update repository structure
refactor: improve prompt template
chore: rename repository references
```

---

## Disclaimer

Este repositorio no pretende atribuirse la autoría de todos los conceptos, frameworks o metodologías referenciadas.

El contenido combina:

- experiencia práctica en Product Management
- prácticas ampliamente conocidas de producto y delivery
- workflows asistidos por IA
- refinamiento iterativo de prompts
- aprendizaje público de la comunidad de producto e IA

El propósito de este repositorio es organizar herramientas prácticas de trabajo, no reclamar propiedad sobre conceptos que ya forman parte del ecosistema general de Product Management o inteligencia artificial.

Las personas usuarias deben revisar y adaptar todas las salidas generadas a partir de estos prompts antes de usarlas en contextos profesionales, operativos o críticos para el negocio.

---

## Inspiración y Recursos

Este repositorio fue parcialmente inspirado por recursos útiles de la comunidad de Product Management e IA.

Una referencia relevante es:

https://github.com/deanpeters/product-manager-prompts/

Podrán agregarse referencias adicionales a medida que el playbook evolucione.

---

## Licencia

Este proyecto está publicado bajo la licencia MIT.

Consulta el archivo [LICENSE](LICENSE) para más información.
