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
│   ├── plantilla-acta-reunion.md      ← Formato único para cualquier reunión
│   ├── plantilla-reporte-diario.md     ← Formato para daily de cada dev
│   └── plantilla-weekly-sync.md        ← Formato para sync semanal leads→CEO
├── sprint-XX/
│   ├── actas/                           ← Actas de ceremonias del sprint
│   │   ├── 01-planning-YYYY-MM-DD.md
│   │   ├── 02-daily-YYYY-MM-DD.md
│   │   ├── 03-daily-YYYY-MM-DD.md
│   │   └── ...
│   └── reportes/                        ← Reportes asíncronos del sprint
│       ├── daily-dev-steven.md
│       ├── daily-dev-eduardo.md
│       ├── daily-dev-dev1.md
│       ├── daily-dev-dev2.md
│       └── weekly-sync-leads.md
└── INDICE_SEGUIMIENTO.md              ← Este archivo
```

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
