# Modelo Financiero Corporativo — Nothing Sense

**Versión:** 1.0
**Junio 2026**

---

## 1. Costos de Constitución y Formalización

| Concepto | Valor estimado | Notas |
|---|---|---|
| Registro Cámara de Comercio (S.A.S.) | $150.000 - $300.000 | Varía por ingresos reportados. Mínimo 0% de ingresos → tarifa mínima. |
| Autenticación y registro libros contables | $50.000 - $100.000 | |
| NIT (DIAN) — RUT | $0 | Gratuito. |
| Firma electrónica (certificado) para representante legal | $150.000 - $250.000 | Anual. Ej: Certicámara, Autentic. |
| Registro de marca (SIC) — 1 clase | $900.000 aprox. | Trámite opcional en Q3. |
| **Subtotal constitución** | **$350.000 - $500.000** | Sin incluir marca. |

---

## 2. Costos Operativos Mensuales

### Infraestructura tecnológica

| Concepto | Beta (gratis) | Producción (estimado) |
|---|---|---|
| Supabase (PostgreSQL) | $0 (500 MB, se pausa inactivo) | $25/mes (plan Pro) |
| Render (backend) | $0 (cold starts) | $7-25/mes (plan Starter) |
| Vercel (frontend) | $0 | $0 con plan Hobby |
| Cloudflare R2 (archivos) | $0 (10 GB gratis) | $0 hasta 10 GB |
| Dominio nothingsense.co | $0 | ~$40/año (~$3.3/mes) |
| **Subtotal infraestructura** | **~$0/mes** | **~$35-55/mes** |

### Gastos administrativos

| Concepto | Mensual |
|---|---|
| Contador (outsourcing) | $150.000 |
| Abogada (outsourcing) | $150.000 |
| Conectividad, planes de datos y equipos | $50.000 |
| Marketing / Redes | $0 (gestión directa) |
| Imprevistos | $100.000 |
| **Subtotal administrativo** | **$450.000** |

> *Costos de contador y abogada pueden aumentar con el tiempo cuando se requieran servicios más complejos.*

### Proyección de caja mensual (beta)

| Rubro | Valor |
|---|---|
| **Costos infraestructura** | $0 - $55 USD |
| **Costos administrativos** | $450.000 COP |
| **Costo total mensual estimado** | **~$450.000 COP** (en beta gratuita) |

---

## 3. Runway y Bootstrap

### Situación actual

- **Cap Table:** Fredinson (45.5%), Steven (30%), Eduardo (15%), Pool (9.5%).
- **Inversión inicial:** Aporte de los fundadores (bootstrapping). No hay inversionistas externos.
- **Política salarial:** Sin salarios hasta alcanzar Tramo 2 (rentabilidad operativa). Los fundadores viven de ahorros/ingresos externos.

### Escenarios

| Escenario | Ingresos mensuales | Tiempo para alcanzarlo |
|---|---|---|
| **Beta (sin ingresos)** | $0 | Q3 2026 |
| **Lanzamiento público** | $200.000 - $1.000.000 (comisiones + suscripciones) | Q4 2026 |
| **Punto de equilibrio (sin salarios)** | ~$450.000/mes (cubre gastos operativos) | ~Q1 2027 |
| **Punto de equilibrio (con salarios mínimos)** | ~$3.000.000 - $4.000.000/mes | ~Q2 2027 |

---

## 4. Cuentas por pagar diferidas (opcional)

| Concepto | Valor | Prioridad | Cuándo |
|---|---|---|---|
| Registro de marca SIC | ~$900.000 | Media | Q3 2026 |
| Certificado de firma electrónica | ~$200.000 | Alta | Antes de lanzar firma certificada |
| Plan pago Render (sin cold starts) | ~$25 USD | Alta | Al lanzar producción |
| Gastos notariales varios | ~$200.000 | Media | Si se requiere |

---

## 5. Notas y Riesgos

1. **Sin salarios:** El equipo no recibe remuneración hasta que la empresa genere ingresos suficientes. Esto es un riesgo de retención si el MVP se alarga más de 9-12 meses. **Trigger sugerido:** si en Q1 2027 no hay ingresos recurrentes, evaluar financiamiento externo o reducir alcance del equipo.
2. **Costos en USD:** La infraestructura (Render, Supabase, R2) se paga en dólares. El TRM afecta el costo real en COP.
3. **Contador y abogada:** Son costos fijos incluso sin ingresos. Son necesarios para cumplimiento legal.
4. **Fondo de emergencia:** Se recomienda mantener un colchón de 3 meses de gastos operativos (~$1.35M COP) antes de cualquier gasto no esencial.
5. **Break-even real:** El punto de equilibrio sin salarios (~$450K/mes) es alcanzable temprano, pero no es sostenible. El break-even realista con salarios mínimos para los fundadores está entre $3M y $4M mensuales.
