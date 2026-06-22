# ADR-001: Stack Tecnológico de NAP

**Estado:** Aceptada
**Fecha:** Junio 2026
**Decisores:** Fredinson Solano (CEO), Steven Quiñones (Backend Lead), Eduardo Morales (Frontend Lead)
**Contexto:** El equipo debe iniciar el desarrollo del MVP de NAP y requiere decisiones tecnológicas firmes antes de escribir la primera línea de código.

---

## ADR-001.1 — Estilo Arquitectónico

**Decisión:** Monolito modular (package-by-feature)

| Opción | A favor | En contra |
|---|---|---|
| **Monolito modular** | Despliegue único, transacciones ACID entre módulos, simplicidad operativa. | Riesgo de acoplamiento si no se disciplinan límites. |
| Microservicios | Escalado independiente. | Sobrecarga operativa prematura para equipo pequeño. |

**Consecuencia:** Backend organizado por módulos (usuarios, perfiles, marketplace, contratos, pagos, firma, disputas, etc.) con API interna explícita entre ellos.

## ADR-001.2 — Backend

**Decisión:** Spring Boot (Java 17+)

| Opción | A favor | En contra |
|---|---|---|
| **Spring Boot** | Equipo domina Java; Spring Security para RBAC+MFA; transaccionalidad declarativa; ecosistema maduro. | Mayor consumo de memoria y cold starts en planes gratuitos. |
| NestJS / Express | Mismo lenguaje que frontend. | Equipo no lo domina; ecosistema transaccional menos maduro. |

**Stack interno:** Spring Data JPA / Hibernate, Spring Security + JWT + TOTP (MFA), SpringDoc (OpenAPI), JUnit 5 + Mockito + Testcontainers.

## ADR-001.3 — Base de Datos

**Decisión:** PostgreSQL 15+

| Opción | A favor | En contra |
|---|---|---|
| **PostgreSQL** | ACID, JSONB para versiones, numeric para importes, timestamptz para UTC, maduro. | Requiere diseño cuidadoso de índices. |
| MySQL | Amplia adopción. | Tipos avanzados menos ricos. |
| MongoDB | Flexibilidad de esquema. | Dominio relacional/transaccional. |

## ADR-001.4 — Frontend

**Decisión:** Angular (última LTS) + TypeScript

| Opción | A favor | En contra |
|---|---|---|
| **Angular** | Equipo lo domina; framework completo (router, forms, i18n); estructura opinada. | Curva de aprendizaje; bundles grandes. |
| React | Ecosistema flexible. | Menos opinado, requiere ensamblar librerías. |

**Stack interno:** Tailwind CSS (estilos), Angular CDK (componentes headless accesibles), Angular i18n, Lazy loading por módulos.

## ADR-001.5 — Infraestructura y Hosting

**Decisión:** Estrategia PaaS por capa

| Componente | Proveedor | Justificación |
|---|---|---|
| Base de datos | Supabase (PostgreSQL gestionado) | Plan gratuito con 500 MB, integración nativa Postgres. |
| Backend | Render | Despliegue por git push, contenedores, plan gratuito disponible. |
| Frontend | Vercel | Optimizado para Angular, CDN global, plan gratuito. |
| Archivos | Cloudflare R2 | 10 GB gratis permanentes, egreso gratuito, compatible S3. |

## ADR-001.6 — Autenticación y Autorización

**Decisión:** Spring Security (NO Supabase Auth)

| Opción | A favor | En contra |
|---|---|---|
| **Spring Security** | Sin techo de uso, control total RBAC+MFA, auditoría centralizada, sin lock-in. | Hay que implementar registro, recuperación, verificación. |
| Supabase Auth | Registro y OAuth listos. | Límite 50K MAU, identidad partida en dos sistemas. |

## ADR-001.7 — Pagos

**Decisión:** Split de Pagos vía pasarela (ePayco prioritario, MercadoPago como respaldo)

- **Modelo:** El dinero del cliente va directo a la pasarela. NAP nunca recibe los fondos (evita captación ilegal).
- **Dispersión:** La pasarela envía el pago al profesional y la comisión a NAP por separado.
- **Nequi:** Método de retiro prioritario para profesionales colombianos.
- **Facturación DIAN:** Integración con proveedor tecnológico autorizado (Alegra, Siigo, etc.).

## ADR-001.8 — Firma Electrónica

**Decisión:** Dual según tipo de contrato

| Tipo | Mecanismo | Proveedor |
|---|---|---|
| Contrato informal | Firma simple (OTP + Clickwrap + registro de auditoría) | Motor propio |
| Contrato formal | Firma digital certificada | Proveedor local colombiano (Autentic, Certicámara), DocuSign como plan B |

---

## Requisitos relacionados

RNF-005 (responsivo), RNF-006 (normatividad colombiana), RNF-009 (fiabilidad), RNF-013 (RBAC), RNF-015 (modularidad), RNF-016 (portabilidad), RNF-019 (escalabilidad), RNF-025 (idempotencia), RN-010 (MFA), RN-014 (moneda COP).

## Historial de cambios

| Versión | Fecha | Cambio |
|---|---|---|
| 1.0 | Junio 2026 | Definición inicial del stack tecnológico. |
