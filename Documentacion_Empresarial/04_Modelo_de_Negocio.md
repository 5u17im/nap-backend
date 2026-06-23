# Modelo de Negocio e Innovación Comercial (Business Model)

**Empresa:** Nothing Sense
**Producto:** Plataforma NAP
**Versión:** 2.0 — Actualizado con lienzo CANVAS completo

---

## 1. Propuesta de Valor

NAP ofrece protección jurídica automatizada y resguardo financiero (*Escrow*) tanto para contratos corporativos de empresas (B2B) como para acuerdos rápidos de oficios y servicios informales (C2C). Resuelve el problema endémico del fraude, el impago y la informalidad laboral en Colombia al fungir como un tercero de confianza imparcial.

### 1.1. Perfil del Cliente (Customer Profile)

- **Pains:** Fraude e impago en acuerdos informales; desconfianza entre partes; procesos burocráticos para contratar; costo de abogados; riesgo de responsabilidad solidaria (B2B); facturación ilegal; pérdida de documentos contractuales.
- **Gains:** Garantía de pago (escrow); firma con validez legal; trazabilidad contractual; reducción de costos legales; agilidad en contratación; formalización sin rigidez.
- **Jobs:** Publicar una necesidad y encontrar profesional confiable; contratar un proveedor sin riesgo; cobrar un servicio sin depender de la palabra.

### 1.2. Mapa de Valor (Value Map)

- **Pain relievers:** Escrow retiene el pago hasta conformidad; amigable composición integrada (sin ir a abogado); KYC y reputación del profesional; facturación electrónica automática DIAN; hash de integridad del contrato firmado.
- **Gain creators:** Plantillas de contratos pre-validadas; split de pagos sin que NAP capte fondos; firma electrónica simple (rápida) y certificada (formal); comisión dinámica; panel de control B2B.
- **Productos y servicios:** Plataforma web NAP (marketplace + CLM); firma electrónica; escrow; gestión de disputas; facturación; reportes.

---

## 2. Segmentación de Clientes (*Target Markets*)

- **C2C (Economía Informal y Freelancers):** Trabajadores de oficios varios, diseñadores independientes, consultores y contratistas ocasionales que buscan garantía de pago.
- **B2B (Sector Corporativo):** Empresas y agencias Pymes que subcontratan constantemente personal o servicios y buscan agilizar la firma y el pago sin pesados trámites burocráticos.

---

## 3. Canales de Distribución y Comunicación

- **Canal principal:** Aplicación web responsiva (webapp) accesible desde cualquier navegador, sin instalación, optimizada para móvil. La distribución inicial es 100% digital.
- **Adquisición B2B:** Equipo fundador con outreach directo (LinkedIn, referidos, redes empresariales) a Pymes de Montería, Valledupar y principales ciudades. Demos personalizadas vía Google Meet/WhatsApp.
- **Adquisición C2C:** Campañas en redes sociales (Instagram, TikTok, Facebook Ads) segmentadas por ubicación geográfica (inicio: Caribe colombiano) y por gremio (oficios varios, freelancers digitales).
- **Onboarding:** Enlace de invitación directa desde empresas a sus contratistas (efecto red B2B2C). Código QR en locales físicos de empresas aliadas.
- **Post-venta:** Notificaciones vía WhatsApp Business API y correo electrónico. Centro de ayuda in-app con FAQ y chatbot.

---

## 4. Relaciones con los Clientes

- **C2C (Cliente individual y Profesional):** Autoservicio asistido por chat en vivo, con opción de escalar a mediador humano en disputas. Expectativa de resolución de disputas en menos de 72 horas hábiles. Programa de referidos.
- **B2B (Empresas):** Account Manager dedicado (inicialmente el CEO) para onboarding, capacitación y soporte prioritario. Revisiones trimestrales de uso y ahorro. Contrato SLA con tiempo de respuesta.
- **Retención:** Programa de fidelidad con comisión reducida para usuarios recurrentes. Gamificación con insignias de "Cliente Confiable" y "Profesional Verificado".

---

## 5. Fuentes de Ingresos (Monetización)

| Producto/Servicio | Precio | Destinatario | Notas |
|---|---|---|---|
| Comisión por transacción informal | 10% del valor del acuerdo (tasa dinámica decreciente para montos mayores) | Retenida del pago al profesional | Configurable vía RF-060 |
| Penalidad por disputa de mala fe | 5% adicional sobre el valor en disputa | Parte perdedora que actuó de mala fe | RN-016 |
| Suscripción B2B Premium (futura) | $150.000 — $500.000 COP/mes según tamaño de empresa | Empresa contratante | Firmas ilimitadas, reportes DIAN, white label |
| Verificación de antecedentes (futura) | $20.000 — $50.000 COP por verificación | Empresa (opcional) | Validación judicial y de referencias |

Modelo Freemium a evaluar: primer acuerdo sin comisión para nuevos usuarios; onboarding gratuito B2B por 30 días.

---

## 6. Recursos Clave

- **Físicos/Infraestructura:** Servidores en Render (backend), Vercel (frontend), Supabase (PostgreSQL), Cloudflare R2 (almacenamiento documental). Sin inversión en hardware propio.
- **Intelectuales:** Plataforma de software (código fuente NAP + ERS + ADR + modelo de datos), biblioteca de plantillas de contratos validadas legalmente, algoritmo de matching y reputación, base de datos de profesionales verificados.
- **Humanos:** Equipo fundador multidisciplinario (CEO comercial/legal, CTO técnico, Frontend Lead UX). Asesores externos: abogada (derecho contractual), contador (facturación DIAN, impuestos).
- **Red de aliados:** Integraciones API con pasarela de pago, proveedor de firma electrónica y proveedor tecnológico DIAN.
- **Financieros:** Bootstrapping inicial; capital semilla futuro de fondos de tecnología colombianos (iNNpulsa, Apps.co) o ángeles inversionistas.

---

## 7. Actividades Clave

1. **Desarrollo y mejora continua:** Implementación de funcionalidades por orden de prioridad (RF), mantenimiento de plataforma, corrección de errores. Cumplimiento de la hoja de ruta definida en ERS.
2. **Moderación y prevención de fraude:** Validación KYC, monitoreo de transacciones sospechosas, detección de patrones de disputa de mala fe. Auditoría de firmas.
3. **Gestión de disputas (amigable composición):** Mediación humana para conflictos entre partes, revisión de evidencias, decisión vinculante sobre escrow.
4. **Adquisición bidireccional:** Captar empresas (B2B) y, simultáneamente, profesionales/contratistas (C2C). Estrategia del problema huevo-gallina mitigada por el plan de lanzamiento gradual (B2B primero).
5. **Cumplimiento legal y tributario:** Facturación electrónica DIAN, gestión de datos personales (Ley 1581), actualización de términos y condiciones, hash y custodia de contratos para validez probatoria.
6. **Marketing y crecimiento:** Content marketing (guías de contratación segura), SEO local, campañas en redes, programa de referidos.

---

## 8. Aliados Clave (*Key Partners*)

| Aliado | Rol | Relación |
|---|---|---|
| Pasarela de pago (ePayco / MercadoPago) | Procesamiento de pagos, split de pagos, escrow técnico | API contractual, comisión por transacción |
| Proveedor de firma electrónica (Autentic / Certicámara) | Firma digital certificada para contratos formales; sello de tiempo y hash | API con costos bajo demanda |
| Proveedor tecnológico DIAN (Alegra / Siigo / Facturadora.com) | Generación y envío de facturación electrónica por comisiones NAP | API REST; costo por factura emitida |
| Despacho de abogados | Validación legal de plantillas de contratos, asesoría en disputas complejas | Honorarios fijos mensuales + por caso |
| Contador externo | Declaraciones tributarias, régimen simple, planeación fiscal | Honorarios mensuales |
| Almacenamiento cloud (Supabase, Cloudflare, Render) | Infraestructura tecnológica | SaaS; planes gratuitos/pagos |
| Futuros: Fintechs de crédito | Adelantos de pago a contratistas (evolución mes 10+) | Revenue share o comisión por préstamo |

---

## 9. Análisis de Mercado

### 9.1. Tamaño de Mercado

- **TAM (Total Addressable Market):** Mercado colombiano de servicios informales + contratación corporativa Pyme (estimado en ~$15 billones COP/año en contratos de bajo y medio monto).
- **SAM (Serviceable Addressable Market):** Servicios digitalizables con escrow + firma (trabajos de oficio, freelancers digitales, subcontratación Pyme) estimado en ~$2 billones COP.
- **SOM (Serviceable Obtainable Market):** Captura del 0.5%-1% del SAM en año 2 (meta: $10.000 — $20.000 millones COP en GMV anual).

### 9.2. Tendencias del Entorno

- Crecimiento del teletrabajo en Colombia (Ley 2121 de 2021).
- Expansión de la economía de plataformas y bancarización (Nequi, Daviplata).
- Obligatoriedad de facturación electrónica DIAN.

### 9.3. Panorama Competitivo

| Competidor | Fortaleza NAP | Debilidad NAP |
|---|---|---|
| **Informal (acuerdo verbal / WhatsApp)** | NAP ofrece escrow + firma + trazabilidad | Barrera de adopción: el usuario informal no pide garantía hasta que sufre fraude |
| **DocuSign / Signaturit** | NAP integra pago + escrow + marketplace | DocuSign es solo firma; no compite en CLM completo |
| **Truora** | NAP no es solo verificación; es transacción completa | Truora tiene KYC más robusto |
| **Workana / Freelancer** | NAP tiene enfoque local colombiano + contratos formales + escrow real | Ellos tienen red instalada de oferta/demanda |
| **Contratación tradicional / bolsa de empleo** | NAP automatiza y baja costos | Costumbre y confianza en lo tradicional |

**Ventaja competitiva sostenible:** Integración vertical (matching → contrato → firma → pago → escrow → disputa) en un solo producto localizado para Colombia, con respaldo legal y split de pagos que mitiga riesgo regulatorio.

---

## 10. Estructura de Costos

- **Costos fijos operativos:** Infraestructura cloud (servidores, base de datos, almacenamiento), dominio web, herramientas SaaS (Jira, Slack).
- **Costos variables:** Comisiones de la pasarela de pago, pauta publicitaria digital (CAC), honorarios bajo demanda (abogada, contador, marketing), costos de APIs de firma electrónica y facturación DIAN.
- **Costos de personal:** Progresivos según la fase (fundadores sin salario en fases iniciales, salarios progresivos post-lanzamiento).
- **Provisiones:** Fondo para reembolsos por disputas y contracargos.

---

## 11. Métricas Clave (KPIs)

| KPI | Meta Año 1 | Meta Año 2 |
|---|---|---|
| Usuarios registrados | [Por definir] | [Por definir] |
| Contratos/acuerdos creados | [Por definir] | [Por definir] |
| GMV (Gross Merchandise Value) | [Por definir] | [Por definir] |
| Ingreso neto por comisiones | [Por definir] | [Por definir] |
| Tasa de conversión (registro → 1er contrato) | [Por definir] | [Por definir] |
| Tasa de disputas sobre contratos | [Por definir] | [Por definir] |
| NPS (Net Promoter Score) | [Por definir] | [Por definir] |
| Churn mensual B2B | [Por definir] | [Por definir] |
| CAC (Customer Acquisition Cost) | [Por definir] | [Por definir] |
| LTV (Life Time Value) | [Por definir] | [Por definir] |

---

## 12. Proyección Financiera

**Supuestos:** Equipo de 3 fundadores. Comisión promedio referencial 10%. Pasarela cobra ~3% + costo fijo por transacción.

| Concepto | Mes 1-3 | Mes 4-6 | Mes 7-9 | Mes 10-12 |
|---|---|---|---|---|
| **Ingresos** | | | | |
| Comisiones | [Por definir] | [Por definir] | [Por definir] | [Por definir] |
| Suscripciones B2B | — | — | — | [Por definir] |
| Penalidades | [Por definir] | [Por definir] | [Por definir] | [Por definir] |
| **Total Ingresos** | **[Por definir]** | **[Por definir]** | **[Por definir]** | **[Por definir]** |
| **Costos** | | | | |
| Infraestructura cloud | [Por definir] | [Por definir] | [Por definir] | [Por definir] |
| Comisiones de pasarela | [Por definir] | [Por definir] | [Por definir] | [Por definir] |
| Honorarios (abogada+contador) | [Por definir] | [Por definir] | [Por definir] | [Por definir] |
| Marketing digital (CAC) | [Por definir] | [Por definir] | [Por definir] | [Por definir] |
| **Total Costos** | **[Por definir]** | **[Por definir]** | **[Por definir]** | **[Por definir]** |
| **Resultado Neto** | **[Por definir]** | **[Por definir]** | **[Por definir]** | **[Por definir]** |

Punto de equilibrio esperado: [Por definir].
Necesidad de capital estimada: [Por definir]. Fuentes: bootstrapping, iNNpulsa, ángeles regionales.

> Nota: Esta proyección es ilustrativa. Debe refinarse con un modelo financiero en hoja de cálculo con escenarios optimista, realista y pesimista.

---

## 13. Proyección Futura (Post-Mes 10)

Para escalar el *Business Value*, se plantean las siguientes implementaciones futuras:

- **Suscripciones B2B Premium:** Membresías mensuales a empresas (SaaS) que requieran firmas ilimitadas, reportes tributarios automatizados y personalización corporativa (White Label).
- **Adelantos de Pago (Crédito):** Alianzas futuras con *Fintechs* para financiar a los contratistas mientras el dinero está asegurado en Escrow.
- **Verificación de Antecedentes (*Background Checks*):** Cobro por validaciones profundas de identidad y pasado judicial para contratación empresarial de alto perfil.
- **Expansión geográfica:** Nuevas ciudades de Colombia (Barranquilla, Bogotá, Medellín) y eventualmente mercado latinoamericano.
