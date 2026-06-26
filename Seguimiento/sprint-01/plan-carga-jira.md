# Plan de Carga — Jira Proyecto NAP

**Proyecto:** NAP — Plataforma de gestión y creación de contratos
**URL:** https://nothingsense.atlassian.net/jira/software/projects/NAP/boards/
**Responsable de carga:** Steven (CTO)
**Metodología:** Scrum (Company-Managed)

---

## 1. Configuración del Proyecto

| Concepto | Valor |
|---|---|
| Nombre | NAP — Plataforma de gestión y creación de contratos |
| Clave | **NAP** |
| Tipo | **Scrum (company-managed)** |
| Tablero | Pendiente \| En curso \| En revisión \| Hecho |
| Story Points | Fibonacci: 1, 2, 3, 5, 8, 13 |
| Sprint 1 | 18 Jun — 18 Jul 2026 |

---

## 2. Épicas a Crear (9)

| Épica | Nombre | RFs |
|---|---|---|
| E-1 | Identidad y Acceso (Core) | RF-001, RF-002, RF-004, RF-007 |
| E-2 | Verificación de Identidad (KYC) | RF-003 |
| E-3 | Perfiles | RF-009, RF-010 |
| E-4 | Contratos Formales (B2B) | RF-025, RF-026, RF-027, RF-029, RF-032 |
| E-5 | Firma Electrónica | RF-033, RF-034, RF-035 |
| E-6 | Marketplace (C2C) | RF-014, RF-016, RF-018 |
| E-7 | Acuerdos Informales (C2C) | RF-020, RF-021, RF-022, RF-024 |
| E-8 | Pagos y Custodia (Escrow) | RF-037, RF-038 |
| E-9 | Administración | RF-056, RF-059 |

---

## 3. Sprint 1 — 17 Historias

| # | ID | Historia | SP | Asignado | Épica | Depende de |
|---|---|---|---|---|---|---|
| 1 | NAP-01 | Registro individual (correo+contraseña) | 5 | Steven | E-1 | — |
| 2 | NAP-02 | Registro empresa (NIT+rep.legal) | 5 | Alcides | E-1 | — |
| 3 | NAP-03 | Login con bloqueo tras fallos | 3 | Steven | E-1 | — |
| 4 | NAP-04 | Roles y permisos RBAC | 5 | Steven | E-1 | NAP-01, NAP-02 |
| 5 | NAP-25 | Admin: gestionar cuentas | 5 | Alcides + Andrés | E-9 | NAP-04 |
| 6 | NAP-26 | Log de auditoría | 3 | Alcides | E-9 | NAP-04 |
| 7 | NAP-05 | KYC: cargar documentos | 8 | Alcides + Eduardo | E-2 | NAP-01, NAP-02 |
| 8 | NAP-06 | Perfil profesional | 5 | Alcides + Andrés | E-3 | NAP-01 |
| 9 | NAP-07 | Perfil empresa | 3 | Andrés | E-3 | NAP-02 |
| 10 | NAP-08 | Biblioteca plantillas | 3 | Eduardo + Andrés | E-4 | NAP-04, NAP-05 |
| 11 | NAP-09 | Editor de cláusulas | 8 | Eduardo + Steven | E-4 | NAP-08 |
| 12 | NAP-10 | Versionado + negociación | 8 | Steven + Alcides | E-4 | NAP-09 |
| 13 | NAP-11 | Ciclo de vida del contrato | 5 | Steven | E-4 | NAP-10 |
| 14 | NAP-12 | Repositorio documental | 5 | Alcides | E-4 | NAP-11 |
| **15** | **NAP-13** | Firma electrónica con MFA | **8** | **Steven + Eduardo** | E-5 | NAP-11, NAP-05 |
| **16** | **NAP-14** | Sello tiempo + hash | **5** | **Alcides** | E-5 | NAP-13 |
| **17** | **NAP-15** | Auditoría de firma | **3** | **Alcides** | E-5 | NAP-13 |

> **Total SP:** 79 (tentativo). **Recomendación:** NAP-13, NAP-14 y NAP-15 marcarlos como *stretch goal* y evaluar en la Daily si entran. Sin ellos: 63 SP.

---

## 4. Asignaciones por Persona

### Steven (CTO / Backend Lead)
NAP-01, NAP-03, NAP-04, NAP-09 (BE), NAP-10 (BE), NAP-11, NAP-13 (BE)

### Alcides (Backend Dev)
NAP-02, NAP-05 (BE), NAP-06 (BE), NAP-10 (BE), NAP-12, NAP-14, NAP-15, NAP-25 (BE), NAP-26

### Eduardo (Frontend Lead)
NAP-05 (FE), NAP-08 (FE), NAP-09 (FE), NAP-13 (FE)

### Andrés (Frontend Dev)
NAP-06 (FE), NAP-07, NAP-25 (FE)

---

## 5. Secuencia Semanal Recomendada

```
Semana 1 (18-30 Jun)
  Steven: NAP-01, NAP-02, NAP-03, NAP-04   ← base auth (crítica, sin distracciones)
  Andrés: UI de NAP-01, NAP-02, NAP-03      ← en paralelo
  Alcides: NAP-25, NAP-26, NAP-05 (BE)      ← independiente

Semana 2-3 (1-11 Jul)
  Steven: NAP-08 (BE), NAP-09 (BE), NAP-11  ← corazón B2B
  Alcides: NAP-10 (BE), NAP-12              ← versionado + docs
  Eduardo: UI NAP-08, NAP-09, NAP-05 (FE)   ← UI compleja
  Andrés: UI NAP-06, NAP-07, NAP-25 (FE)    ← UI media

Semana 4 (14-18 Jul)
  Steven + Eduardo: NAP-13 (firma)          ← stretch goal
  Alcides: NAP-14, NAP-15                   ← sellado + auditoría
```

---

## 6. Sub-tareas Técnicas Sugeridas por Historia

Usar como checklist de sub-tareas al crear cada historia en Jira:

| Historia | Sub-tareas técnicas |
|---|---|
| **NAP-01/02/03** | `[BE] Entidad User+Role en PostgreSQL` · `[BE] Endpoint POST /auth/register` · `[BE] POST /auth/login + JWT + rate limit` · `[FE] IU-01: formularios registro/login` · `[FE] AuthService + interceptor JWT` |
| **NAP-04** | `[BE] Esquema RBAC: role, user_role, permission` · `[BE] Spring Security filter chain` · `[BE] Endpoint PUT /users/{id}/role` |
| **NAP-05** | `[BE] Bucket Cloudflare R2 + policy` · `[BE] POST /kyc/upload` · `[BE] Entidad KYC + status` · `[FE] IU-02: carga docs + preview` |
| **NAP-08** | `[BE] Entidad Template + categorías` · `[BE] GET /templates` · `[FE] IU-09: selector plantilla` |
| **NAP-09** | `[BE] PUT /contracts/{id}/clauses` · `[FE] IU-09: editor cláusulas` (MVP: texto plano, no WYSIWYG) · `[FE] Drag & drop bloques` |
| **NAP-10** | `[BE] Tabla contract_version + diff` · `[BE] Estado "en negociación"` · `[FE] Timeline versiones + diff visual` |
| **NAP-11** | `[BE] State machine (enum + transiciones)` · `[BE] ContractLifecycleService` · `[FE] Badge estado + timeline` |
| **NAP-12** | `[BE] FileService (R2 S3 client)` · `[BE] Entidad Document + versionId` · `[BE] Presigned URLs` |
| **NAP-13** | `[BE] Integración proveedor firma (mock primero)` · `[BE] MFA: TOTP` · `[FE] IU-10: flujo firma (revisar→firmar)` |
| **NAP-25** | `[BE] GET/PUT/DELETE /admin/users` · `[FE] IU-14: tabla usuarios + acciones` |
| **NAP-26** | `[BE] Middleware auditoría + tabla audit_log` |

---

## 7. Definition of Done (DoD) Técnica

Cada historia requiere **todo esto** para pasar a "Hecho":

| # | Criterio | Quién |
|---|---|---|
| 1 | Código backend con tests unitarios (JUnit, cobertura ≥70% lógica) | Dev |
| 2 | Código frontend con test de componente (Jasmine/Karma) | Dev |
| 3 | API documentada (OpenAPI/Swagger) | Dev |
| 4 | Migración SQL versionada (Flyway) aplicada | Dev |
| 5 | Integración con Supabase verificada (no depende de entorno local) | Dev |
| 6 | Responsive en móvil + escritorio (si tiene FE) | FE Dev |
| 7 | Sin warnings de compilación ni lint | Dev |
| 8 | PR aprobado por otro miembro del equipo | Peer |
| 9 | Smoke test en ambiente preview (Render + Vercel) | Dev |
| 10 | Criterios de aceptación del backlog cumplidos | Dev + PO |

---

## 8. Instrucciones Paso a Paso para Steven

```
PASO 1 — Crear proyecto
  https://nothingsense.atlassian.net → Projects → Create project
  Elegir: Scrum (company-managed)
  Name: "NAP — Plataforma de gestión y creación de contratos"
  Key: NAP (se genera solo)

PASO 2 — Configurar tablero
  Board → Configure → Columnas: Pendiente | En curso | En revisión | Hecho

PASO 3 — Crear 9 épicas
  Backlog → Create issue → Tipo: Epic
  Una por una con nombre corto ej. "E-1: Identidad y Acceso"

PASO 4 — Crear 17 historias del Sprint 1
  Create issue → Tipo: Story
  Asignar Epic Link, Summary, Description (criterios aceptación), Story Points, Sprint 1

PASO 5 — Asignar responsables
  Asignee según tabla de la sección 4
  Historias mixtas (BE+FE): crear subtareas separadas

PASO 6 — Dar permisos a Fredinson y al equipo
  Project settings → People → Add people

PASO 7 — Sprint Planning
  Recorrer las 17 historias, ajustar SP, confirmar orden y asignaciones
```

---

## 9. Resumen para la Daily

| Concepto | Valor |
|---|---|
| Equipo | 4 devs (Steven, Alcides, Eduardo, Andrés) |
| Sprint 1 | 18 Jun — 18 Jul (31 días) |
| Historias | 17 (NAP-01 a NAP-15 + NAP-25, NAP-26) |
| SP total | 79 (63 sin stretch goals) |
| Prioridad #1 | Semana 1: NAP-01→NAP-04 (base auth) sin distracciones |
| Stretch | NAP-13, NAP-14, NAP-15 (firma electrónica) |
| Backlog futuro | Marketplace (NAP-16/17/18) y Acuerdos Informales (NAP-19/20/21/22) para Sprint 2 |
