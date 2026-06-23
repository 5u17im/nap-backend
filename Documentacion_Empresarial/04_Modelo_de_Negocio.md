# Modelo de Negocio e Innovación Comercial (Business Model)

**Empresa:** Nothing Sense
**Producto:** Plataforma NAP
**Versión:** 2.1 — Lienzo CANVAS + análisis complementarios de mercado, métricas y finanzas

---

> Las secciones 1 a 8 corresponden a los 9 bloques del Business Model Canvas (Osterwalder); las secciones 9 a 12 son análisis complementarios.

## 1. Segmentación de Clientes (*Target Markets*)

- **C2C (Economía Informal y Freelancers):** Trabajadores de oficios varios, diseñadores independientes, consultores y contratistas ocasionales que buscan garantía de pago.
- **B2B (Sector Corporativo):** Empresas y agencias Pymes que subcontratan constantemente personal o servicios y buscan agilizar la firma y el pago sin pesados trámites burocráticos.

---

## 2. Propuesta de Valor

NAP ofrece protección jurídica automatizada y resguardo financiero (*Escrow*) tanto para contratos corporativos de empresas (B2B) como para acuerdos rápidos de oficios y servicios informales (C2C). Resuelve el problema endémico del fraude, el impago y la informalidad laboral en Colombia al fungir como un tercero de confianza imparcial.

### 2.1. Perfil del Cliente (Customer Profile)

- **Pains:** Fraude e impago en acuerdos informales; desconfianza entre partes; procesos burocráticos para contratar; costo de abogados; riesgo de responsabilidad solidaria (B2B); facturación ilegal; pérdida de documentos contractuales.
- **Gains:** Garantía de pago (escrow); firma con validez legal; trazabilidad contractual; reducción de costos legales; agilidad en contratación; formalización sin rigidez.
- **Jobs:** Publicar una necesidad y encontrar profesional confiable; contratar un proveedor sin riesgo; cobrar un servicio sin depender de la palabra.

### 2.2. Mapa de Valor (Value Map)

- **Pain relievers:** Escrow retiene el pago hasta conformidad; amigable composición integrada (sin ir a abogado); KYC y reputación del profesional; facturación electrónica automática DIAN; hash de integridad del contrato firmado.
- **Gain creators:** Plantillas de contratos pre-validadas; split de pagos sin que NAP capte fondos; firma electrónica simple (rápida) y certificada (formal); comisión dinámica; panel de control B2B.
- **Productos y servicios:** Plataforma web NAP (marketplace + CLM); firma electrónica; escrow; gestión de disputas; facturación; reportes.

---

## 3. Canales de Distribución y Comunicación

- **Canal principal:** Aplicación web responsiva (webapp) accesible desde cualquier navegador, sin instalación, optimizada para móvil. La distribución inicial es 100% digital.
- **Adquisición B2B:** Equipo fundador con outreach directo (LinkedIn, referidos, redes empresariales) a Pymes de Montería, Valledupar y principales ciudades. Demos personalizadas vía Google Meet/WhatsApp.
- **Adquisición C2C:** Campañas en redes sociales (Instagram, TikTok, Facebook Ads) segmentadas por ubicación geográfica (inicio: Caribe colombiano) y por gremio (oficios varios, freelancers digitales).
- **Estrategia de adquisición bidireccional (huevo-gallina):** Captar empresas (B2B) primero para que ellas inviten a sus contratistas (efecto red B2B2C), construyendo masa crítica de oferta antes de la campaña C2C. Campaña C2C solo después de tener un catálogo base de profesionales registrados.
- **Onboarding:** Enlace de invitación directa desde empresas a sus contratistas. Código QR en locales físicos de empresas aliadas.
- **Post-venta:** Notificaciones vía WhatsApp Business API y correo electrónico. Centro de ayuda in-app con FAQ y chatbot.

---

## 4. Relaciones con los Clientes

- **C2C (Cliente individual y Profesional):** Autoservicio asistido por chat en vivo, con opción de escalar a mediador humano en disputas. Expectativa de resolución de disputas en menos de 72 horas hábiles. Programa de referidos.
- **B2B (Empresas):** Account Manager dedicado (inicialmente el CEO) para onboarding, capacitación y soporte prioritario. Revisiones trimestrales de uso y ahorro. Contrato SLA con tiempo de respuesta.
- **Retención:** Programa de fidelidad con comisión reducida para usuarios recurrentes. Gamificación con insignias de "Cliente Confiable" y "Profesional Verificado".

---

## 5. Fuentes de Ingresos (Monetización)

### 5.1. Modelo Actual (Decidido)

| Producto/Servicio | Precio | Destinatario | Notas |
|---|---|---|---|
| Comisión por transacción informal | 10% del valor del acuerdo (tasa dinámica decreciente) | Retenida del pago al profesional | Configurable vía RF-060 (requisito funcional del producto) |
| Penalidad por disputa de mala fe | 5% adicional sobre el valor en disputa | Parte perdedora que actuó de mala fe | Regla de negocio RN-016 |

> **Desglose de comisión dinámica (referencia):** 10% para montos menores a $1M COP, 8% para montos entre $1M y $5M COP, 6% para montos superiores a $5M COP. Valores configurables mediante RF-060.
>
> **IVA:** Todos los precios están antes de IVA (tarifa del 19% aplicable según el régimen tributario de NAP).

### 5.2. Modelo Futuro (Post-Mes 10)

| Producto/Servicio | Precio estimado | Destinatario | Notas |
|---|---|---|---|
| Suscripción B2B Premium | $150.000 - $500.000 COP/mes según tamaño de empresa | Empresa contratante | Firmas ilimitadas, reportes DIAN, white label |
| Verificación de antecedentes | $20.000 - $50.000 COP por verificación | Empresa (opcional) | Validación judicial y de referencias |

### 5.3. Experimentos de Crecimiento a Evaluar

- Primer acuerdo sin comisión para nuevos usuarios (reducción de barrera de entrada).
- Onboarding gratuito B2B por 30 días (prueba sin compromiso).

---

## 6. Estructura de Costos

- **Costos fijos operativos:** Infraestructura cloud (servidores, base de datos, almacenamiento), dominio web, herramientas SaaS (Jira, Slack). Estimación MVP en etapa beta: ~$0/mes en planes gratuitos (Render, Supabase, Vercel, Cloudflare R2) — con limitaciones como *cold starts* y almacenamiento reducido. Escalamiento a producción con usuarios reales: ~$50-150/mes en planes pagos según volumen.
- **Costos variables:** Comisiones de la pasarela de pago (~3% + costo fijo por transacción), pauta publicitaria digital (CAC), honorarios bajo demanda (abogada, contador, marketing), costos de APIs de firma electrónica y facturación DIAN.
- **Costos de personal:** Fundadores sin salario en fases iniciales; salarios progresivos post-lanzamiento.
- **Provisiones:** Fondo para reembolsos por disputas y contracargos.

---

## 7. Recursos Clave

- **Físicos/Infraestructura:** Servidores en Render (backend), Vercel (frontend), Supabase (PostgreSQL), Cloudflare R2 (almacenamiento documental). Sin inversión en hardware propio.
- **Intelectuales:** Plataforma de software (código fuente NAP + ERS + ADR + modelo de datos), biblioteca de plantillas de contratos validadas legalmente, algoritmo de matching y reputación, base de datos de profesionales verificados.
- **Humanos:** Equipo fundador multidisciplinario (CEO comercial/legal, CTO técnico, Frontend Lead UX). Asesores externos: abogada (derecho contractual), contador (facturación DIAN, impuestos).
- **Red de aliados:** Integraciones API con pasarela de pago, proveedor de firma electrónica y proveedor tecnológico DIAN.
- **Financieros:** Bootstrapping inicial; capital semilla futuro de fondos de tecnología colombianos (iNNpulsa, Apps.co) o ángeles inversionistas.

---

## 8. Actividades Clave

1. **Desarrollo y mejora continua:** Implementación de funcionalidades por orden de prioridad (requisitos funcionales RF, según la ERS), mantenimiento de plataforma, corrección de errores.
2. **Moderación y prevención de fraude:** Validación KYC, monitoreo de transacciones sospechosas, detección de patrones de disputa de mala fe. Auditoría de firmas.
3. **Gestión de disputas (amigable composición):** Mediación humana para conflictos entre partes, revisión de evidencias, decisión vinculante sobre escrow.
4. **Cumplimiento legal y tributario:** Facturación electrónica DIAN, gestión de datos personales (Ley 1581), actualización de términos y condiciones, hash y custodia de contratos para validez probatoria.
5. **Marketing y crecimiento:** Marketing de contenidos (guías de contratación segura), SEO local, campañas en redes, programa de referidos.

---

## 9. Aliados Clave (*Key Partners*)

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

## 10. Análisis de Mercado

### 10.1. Tamaño de Mercado

- **TAM (Total Addressable Market):** Mercado colombiano de servicios informales + contratación corporativa Pyme (estimado en ~$15 billones COP/año en contratos de bajo y medio monto).
- **SAM (Serviceable Addressable Market):** Servicios digitalizables con escrow + firma (trabajos de oficio, freelancers digitales, subcontratación Pyme) estimado en ~$2 billones COP.
- **SOM (Serviceable Obtainable Market):** Captura del 0.5-1% del SAM en año 2 (meta: $10.000 - $20.000 millones COP en GMV anual).

### 10.2. Tendencias del Entorno

- Crecimiento del teletrabajo en Colombia (Ley 2121 de 2021).
- Expansión de la economía de plataformas y bancarización (Nequi, Daviplata).
- Obligatoriedad de facturación electrónica DIAN.

### 10.3. Panorama Competitivo

| Competidor | Ventaja de NAP | Riesgo / Barrera |
|---|---|---|
| **Informal (acuerdo verbal / WhatsApp)** | NAP ofrece escrow + firma + trazabilidad | Barrera de adopción: el usuario informal no exige garantía hasta que sufre fraude |
| **DocuSign / Signaturit** | NAP integra pago + escrow + marketplace | DocuSign es solo firma; no compite en CLM completo |
| **Truora** | NAP no es solo verificación; es transacción completa | Truora tiene KYC más robusto y red instalada |
| **Workana / Freelancer** | NAP tiene enfoque local colombiano + contratos formales + escrow real | Red de oferta/demanda instalada menor que la de competidores globales |
| **Contratación tradicional / bolsa de empleo** | NAP automatiza y reduce costos | Costumbre y confianza en lo tradicional |

**Ventaja competitiva sostenible:** Integración vertical (matching, contrato, firma, pago, escrow, disputa) en un solo producto localizado para Colombia, con respaldo legal y split de pagos que mitiga riesgo regulatorio de captación de fondos.

---

## 11. Métricas Clave (KPIs)

Métricas a definir por el equipo en sesión de planeación:

- Usuarios registrados
- Contratos/acuerdos creados
- GMV (Gross Merchandise Value)
- Ingreso neto por comisiones
- Tasa de conversión (registro a primer contrato)
- Tasa de disputas sobre contratos
- NPS (Net Promoter Score)
- Churn mensual B2B
- CAC (Customer Acquisition Cost)
- LTV (Life Time Value)

---

## 12. Proyección Financiera

**Supuestos:** Equipo de 3 fundadores. Comisión promedio referencial 10%. Pasarela cobra ~3% + costo fijo por transacción. Infraestructura MVP en etapa beta usando planes gratuitos (~$0/mes con limitaciones de *cold starts* y almacenamiento reducido).

| Concepto | Mes 1-3 | Mes 4-6 | Mes 7-9 | Mes 10-12 |
|---|---|---|---|---|
| **Ingresos** | | | | |
| Comisiones | [Por definir] | [Por definir] | [Por definir] | [Por definir] |
| Suscripciones B2B | — | — | — | [Por definir] |
| Penalidades | [Por definir] | [Por definir] | [Por definir] | [Por definir] |
| **Total Ingresos** | **[Por definir]** | **[Por definir]** | **[Por definir]** | **[Por definir]** |
| **Costos** | | | | |
| Infraestructura cloud | ~$0 (free tiers) | ~$0 (free tiers) | ~$50/mes | ~$150/mes |
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
