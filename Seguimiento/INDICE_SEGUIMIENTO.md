# Índice de Seguimiento — Reportes y Actas

**Propósito:** Registro cronológico de todas las comunicaciones formales del equipo NAP.

---

## Sprints

| Sprint | Fechas | Planning | Dailies | Review | Retro | Weekly Sync |
|---|---|---|---|---|---|---|
| Sprint 01 | [Fecha inicio — Fecha fin] | — | — | — | — | — |

*Leyenda: ✅ Completado · 🔄 En curso · — Pendiente*

---

## Estructura de carpetas

```
Seguimiento/
├── templates/
│   ├── plantilla-acta-reunion.md        ← Formato único para cualquier reunión
│   ├── plantilla-reporte-diario.md      ← Formato para daily de cada dev
│   ├── instructivo-reporte-diario.md    ← Guía para llenar el reporte diario
│   └── plantilla-weekly-sync.md         ← Formato para sync semanal leads→CEO
├── sprint-01/
│   ├── backlog-sprint-01.md              ← Backlog del Sprint 1 (26 US, 9 épicas)
│   ├── actas/                            ← Actas de ceremonias del Sprint 1
│   └── reportes/                         ← Reportes asíncronos del Sprint 1
│       ├── daily-dev-steven.md           ← CTO / Backend Lead
│       ├── daily-dev-eduardo.md          ← Frontend Lead
│       ├── daily-dev-alcides.md          ← Backend Developer
│       ├── daily-dev-andres.md           ← Frontend Developer
│       ├── daily-ceo-fredinson.md        ← CEO
│       └── weekly-sync-leads.md
├── sprint-XX/                            ← Plantilla para sprints futuros
└── INDICE_SEGUIMIENTO.md               ← Este archivo
```

### Instructivo asociado

- `templates/instructivo-reporte-diario.md` — Guía paso a paso para que los devs entiendan el formato, cuándo y cómo reportar. Léelo antes del primer daily del sprint.

## Convenciones de nombrado

- **Actas:** `[número-secuencial]-[ceremonia]-[YYYY-MM-DD].md`
  - Ej: `01-planning-2026-07-01.md`, `02-daily-2026-07-02.md`
- **Reportes diarios:** `daily-dev-[nombre].md` (un archivo por persona por sprint)
- **Sync semanal:** `weekly-sync-leads.md` (entradas por fecha dentro del archivo)

## Referencias cruzadas

- Los formatos y estándares de los reportes están definidos en:
  - `Documentacion_Empresarial/05_Manual_Buenas_Practicas_y_Formatos_Dev.md` (Daily, Cierre de Tareas)
  - `Documentacion_Empresarial/12_Plan_Gestion_Comunicaciones_y_Cambios.md` (Matriz de comunicaciones, DoD)
  - `Documentacion_Empresarial/06_Manual_Operaciones_CEO.md` (Rituales semanales del CEO)
