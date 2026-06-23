# Retroalimentación del Equipo Agéntico — Documentación Nothing Sense

**Fecha:** 22/06/2026
**Propósito:** Feedback consolidado de los agentes de revisión (Marketing, Legal, Consultoría General, Diseño) para evaluación del CEO.

---

## Resumen de Estados

| Documento | Estado | Prioridad cambios |
|---|---|---|
| ICP Perfil Cliente Ideal | ✅ Aprobado con observaciones | Media |
| One-Pager B2B | ✅ Aprobado con observaciones | Baja |
| Pitch Deck | ✅ Aprobado con observaciones | **Alta** |
| Plan de Growth | ✅ Aprobado con observaciones | **Alta** |
| Manual de Marca | ⚠️ Requiere cambios | **Alta** |
| Código de Conducta | ✅ Aprobado con observaciones | **Alta** |
| OKRs Q3-Q4 2026 | ✅ Aprobado con observaciones | **Alta** |
| Modelo Financiero Corporativo | ✅ Aprobado con observaciones | Media |
| Plan Gerencial | ✅ Aprobado con observaciones | Media |
| Landing Page (brief Eduardo) | ✅ Aprobado con observaciones | Media |
| Brief General CEO | ✅ Aprobado con observaciones | Media |

---

## Detalle por Documento

### ICP Perfil Cliente Ideal
**Prioridad:** Media
1. Segmento 4 (desarrollo de software a la medida) diluye el enfoque B2B/C2C de NAP. Si Nothing Sense ofrece ambos, separar completamente las comunicaciones.
2. Target 5-100 empleados es muy amplio para MVP. Sugieren concentrar primeros 3 meses en empresas de 5-30 empleados de la Costa Caribe.
3. Falta criterio de "intensidad de contratación" (ej. >3 contratistas/mes).

### One-Pager B2B
**Prioridad:** Baja
1. "Pagar solo comisión por uso, sin costo fijo" contradice la suscripción B2B desde $150.000/mes. Corregir a "sin costo por usuario adicional" o "sin costo de implementación".
2. Sin caso de uso concreto. Conseguir un beta tester, documentar resultado y agregarlo.
3. Umbrales de comisión dinámica (10%→6-8%) sin explicación. Aclarar si es por monto del contrato.

### Pitch Deck
**Prioridad:** Alta
1. Dato "70% de transacciones informales" marcado como *ilustrativo* — en un pitch deck resta credibilidad. Buscar fuente DANE/Fedesarrollo o citar como estimación interna.
2. Diapositiva de Mercado sin cifras TAM/SAM concretas. Necesitan al menos un número.
3. Diferenciación "todo en uno" es una feature, no un moat competitivo. ¿Qué protege a NAP de que DocuSign agregue marketplace o que Holmes agregue contratos?

### Plan de Growth / Lanzamiento
**Prioridad:** Alta
1. Falta estrategia de contenido para redes (LinkedIn/Instagram) desde ahora, no al lanzamiento. Sin presupuesto de pauta, el equipo debe publicar 3-4 veces/semana.
2. No hay métricas de activación/retención. "Tasa conversión landing→registro" no mide si el producto funciona. Sugieren agregar: % registros que completan KYC, % que crean un contrato, % que completan una transacción.
3. Plan depende 100% del CEO para adquisición B2B (cuello de botella). Documentar script de outreach para que al menos 2 personas puedan ejecutarlo.

### Manual de Marca
**Prioridad:** Alta — **Requiere cambios**
1. Colores, tipografía y logo están en "pendiente". Sin identidad visual definida, el manual no sirve para producción. Bloqueante para frontend, pitch deck y comunicaciones externas.
2. Tono de voz es excelente pero choca con frases vagas. Ser coherentes con la promesa "sin rodeos" también en la documentación interna.
3. Faltan ejemplos concretos de copy para redes y landing page.

### Código de Conducta
**Prioridad:** Alta (legal)
1. **Cesión de PI para contratistas independientes:** La frase "toda PI creada para Nothing Sense pertenece a Nothing Sense S.A.S." no es automática para contratistas. Se requiere **contrato de cesión de derechos de autor** por separado. Sin él, el código de Alcides y Andrés podría pertenecer a ellos.
2. **Pérdida de derechos de voto como sanción:** Inviable si no está pactado en los estatutos o en el Acuerdo de Accionistas. Remitir exclusivamente al Acuerdo de Accionistas.
3. **Confidencialidad poscontractual sin plazo:** "Incluso después de dejar la empresa" sin límite puede ser cuestionado. Sugieren fijar 2-3 años desde la desvinculación.

### OKRs Q3-Q4 2026
**Prioridad:** Alta
1. **KR 4.1 sobrecargado.** Tener todos los módulos (contratos formales, firma, reputación, disputas) para diciembre con el equipo actual es muy agresivo. Sugieren priorizar contratos formales + firma y mover reputación/disputas a Q1 2027.
2. **KR 5.2 (2 suscripciones B2B)** depende de que contratos formales esté listo. Mover a finales de Q4 / principios de Q1 2027, o redefinir como "cartas de intención B2B".
3. **Objetivo 6 (preparar próximo proyecto)** distrae el foco. Sugieren eliminar o mover a Q1 2027.

### Modelo Financiero Corporativo
**Prioridad:** Media
1. Riesgo de retención del equipo con salario $0 no cuantificado. Sugieren incluir trigger: si en Q1 2027 no hay ingresos, evaluar financiamiento externo.
2. Falta gasto en conectividad/equipo (~$50K/mes adicional).
3. Break-even de $400K/mes asume salario $0. Calcular break-even realista con salarios mínimos (~$3-4M/mes).

### Plan Gerencial
**Prioridad:** Media
1. WP-5.0 (Integraciones, 3 sem.) subestima la complejidad de Split de Pagos + firma certificada + DIAN. Sugieren 5-6 semanas o dividir en WP-5.1 (pagos) y WP-5.2 (firma+DIAN).
2. Riesgo de concentración en consultores externos (abogada ex-pareja, contador amigo). Documentar procesos y tener plan B.
3. Falta buffer de holgura en el cronograma (24 semanas sin margen).

### Landing Page (brief Eduardo)
**Prioridad:** Media
1. Paleta de colores sin definir (Manual de Marca la tiene pendiente). Eduardo decidirá.
2. Emojis como iconos (`🔍 📝 🔒 ✍️`) no son accesibles. Reemplazar por Heroicons o Lucide.
3. Mecanismo de envío del formulario de contacto no especificado (Formspree / EmailJS / backend propio). Decidir antes de codificar.

### Brief General CEO
**Prioridad:** Media
1. Paleta de colores bloqueante — poner fecha límite para que se decida o delegar en Eduardo.
2. Datos de contacto del CEO necesarios para 3 documentos (One-Pager, Pitch Deck, Landing).

---

## Acciones Requeridas del CEO

| Prioridad | Acción | Documento(s) afectados |
|---|---|---|
| **Alta** | Definir logo, colores y tipografía (o ratificar propuesta de Eduardo) | Manual de Marca, Landing Page, Pitch Deck |
| **Alta** | Resolver cesión de PI para contratistas independientes (Alcides, Andrés) | Código de Conducta + contratos individuales |
| **Alta** | Ajustar alcance Q4: priorizar módulos core, mover reputación/disputas | OKRs |
| **Alta** | Reforzar moat competitivo y cifras de mercado en Pitch Deck | Pitch Deck |
| **Media** | Definir umbrales de comisión dinámica | One-Pager, Modelo de Negocio |
| **Media** | Decidir mecanismo de formulario de contacto | Landing Page (Eduardo) |
| **Media** | Compartir datos de contacto para documentos | One-Pager, Pitch Deck, Landing |
