# Plan de Migración — Confluence NAP

**Confluence:** https://nothingsense.atlassian.net/wiki/home
**Responsable:** Steven (CTO)
**Objetivo:** ~20 páginas en Confluence (no migrar los 63+ docs de GitHub, solo resúmenes ejecutivos con enlaces al original)

---

## Estructura del Espacio

```
📂 NAP — Plataforma de gestión y creación de contratos
│
├── 🏠 Home (dashboard del proyecto)
│
├── 📋 Sprint Activo
│   ├── Sprint Backlog
│   ├── Plan de Carga Jira
│   └── Ceremonias
│
├── 🏗️ Arquitectura y Desarrollo
│   ├── ERS — Requisitos del Sistema
│   ├── Stack Tecnológico
│   ├── Decisiones de Arquitectura (ADR)
│   └── Guías Técnicas
│       ├── Estándares Git y PR
│       ├── Manual Backend Lead
│       └── Manual Frontend Lead
│
├── 💼 Negocio y Estrategia
│   ├── Modelo de Negocio
│   ├── Pricing y Comisiones
│   ├── Análisis Competitivo
│   ├── Proyección Financiera
│   ├── OKRs Q3-Q4 2026
│   └── Go-To-Market
│
├── 📜 Legal
│   ├── Términos y Condiciones
│   ├── Política de Datos (Ley 1581)
│   └── Matriz de Riesgos
│
└── 👥 Equipo
    ├── Roles y Responsabilidades
    ├── Manual del CEO
    ├── Plan de Comunicaciones y DoD
    └── Guía de Consultores
```

---

## Páginas a Crear (20)

### Tanda 1 — Fundación (~30 min)

| # | Página | Contenido | Fuente GitHub |
|---|---|---|---|
| 1 | **Home** | Links rápidos a Jira/Vercel/Render/Supabase/GitHub, estado sprint, indicadores | Nueva |
| 2 | **Sprint Backlog** | 17 historias del Sprint 1, SP, asignados, estado | `backlog-sprint-01.md` + `plan-carga-jira.md` |
| 3 | **Plan de Carga Jira** | Épicas, subtareas, DoD, secuencia semanal | `plan-carga-jira.md` |
| 4 | **Roles y Responsabilidades** | Tabla del equipo (5 personas + consultores) | `01_Manual_Roles_y_Funciones.md` |

### Tanda 2 — Arquitectura (~30 min)

| # | Página | Contenido | Fuente GitHub |
|---|---|---|---|
| 5 | **Stack Tecnológico** | Tabla capa/tecnología/versión/ADR | `ADR_Stack_Tecnologico_NAP.md` (resumen) |
| 6 | **Decisiones de Arquitectura (ADR)** | 8 ADR en formato contexto→decisión→consecuencias | `ADR_Stack_Tecnologico_NAP.md` |
| 7 | **ERS — Requisitos** | Resumen ejecutivo + link al PDF/MD en GitHub | `ERS_NAP_IEEE830_v1.1.md` |
| 8 | **Guías Técnicas** | 3 subpáginas: Git, Backend Lead, Frontend Lead | Docs `05`, `09`, `10` |
| 9 | **Matriz de Riesgos** | RT-01 a RT-06, RL-01 a RL-06 | `07_Matriz_Gestion_de_Riesgos.md` |

### Tanda 3 — Negocio + Legal (~30 min)

| # | Página | Contenido | Fuente GitHub |
|---|---|---|---|
| 10 | **Modelo de Negocio** | CANVAS, Value Proposition, KPIs | `04_Modelo_de_Negocio.md` |
| 11 | **Pricing** | Spread, simulación, comisión dinámica | `15_Estructura_Matematica_Pricing.md` |
| 12 | **Go-To-Market** | Growth, ICP, pitch, outreach | `Plan_Growth_Lanzamiento.md` + `16_Guion_Ventas_B2B_y_Pitch.md` |
| 13 | **Proyección Financiera** | Gastos, OPEX, punto equilibrio | `20_Proyeccion_Financiera_y_Salarial.md` |
| 14 | **OKRs** | 5 objetivos, 14 KR | `OKRs_Q3_Q4_2026.md` |
| 15 | **Análisis Competitivo** | Competidores, barreras | `14_Matriz_Analisis_Competitivo.md` |
| 16 | **Términos y Condiciones** | Resumen + link a GitHub | `01_Terminos_y_Condiciones_NAP.md` |
| 17 | **Política de Datos** | Ley 1581 resumida | `02_Politica_Tratamiento_Datos_1581.md` |
| 18 | **Manual del CEO** | Rituales, Cashflow, Cap Table | `06_Manual_Operaciones_CEO.md` |
| 19 | **Plan de Comunicaciones y DoD** | Matriz, change management, DoD | `12_Plan_Gestion_Comunicaciones_y_Cambios.md` |
| 20 | **Ceremonias** | Plantilla acta + enlaces a actas | `plantilla-acta-reunion.md` |

---

## Qué NO Migrar (se queda solo en GitHub)

- Código fuente (backend, frontend)
- Contratos legales firmables (fundadores, consultores, NDA)
- Reportes diarios individuales (`daily-dev-*.md`)
- Plantillas de reporte e instructivos
- Índices del repositorio (`INDICE_MAESTRO.md`, `INDICE_SEGUIMIENTO.md`)
- Documentos sensibles de formalización (Cap Table detallado, Ruta legalización)
- Configuraciones locales (markdownlint)
- Wireframes de Figma (los .fig viven en Figma, referenciar desde Confluence)

---

## Instrucciones para Steven

```
1. Ir a https://nothingsense.atlassian.net/wiki/home
2. Crear espacio → "NAP — Plataforma de gestión y creación de contratos"
3. Seguir el orden de las tandas (1→2→3)
4. Cada página = resumen ejecutivo + bullet points clave + link al .md en GitHub
5. No copiar los 63 documentos completos; Confluence es para el día a día del equipo
6. Home debe tener: enlaces a Jira, Vercel, Render, Supabase, GitHub + estado del sprint
```
