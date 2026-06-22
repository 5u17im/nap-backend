# Diccionario de Términos — Proyecto NAP

**Propósito:** Referencia única para todos los términos, siglas, códigos y nombres utilizados en la documentación del proyecto. Organizado por categorías para consulta rápida.

**Empresa:** Nothing Sense (en formación)
**Plataforma:** NAP

---

## 1. Acrónimos y Siglas Técnicas

| Término | Significado | Definición |
|---|---|---|
| **ADR** | Architecture Decision Record | Registro de una decisión de arquitectura con contexto, opciones evaluadas y consecuencias. Formato MADR, alineado con ISO/IEC/IEEE 42010. |
| **API** | Application Programming Interface | Interfaz de programación para comunicación entre sistemas (pasarela de pago, firma, etc.). |
| **B2B** | Business to Business | Modelo corporativo: empresas que contratan profesionales a través de la plataforma. |
| **C2C** | Customer to Customer | Modelo informal: cliente individual contrata a un profesional para una necesidad puntual. |
| **CAC** | Customer Acquisition Cost | Costo de adquisición de cliente (métrica financiera). |
| **CLM** | Contract Lifecycle Management | Gestión del ciclo de vida del contrato: borrador, revisión, aprobación, firma, vigencia, renovación, terminación. |
| **CU** | Caso de Uso | Descripción de una interacción entre un actor y el sistema para lograr un objetivo. |
| **DIAN** | Dirección de Impuestos y Aduanas Nacionales | Autoridad tributaria de Colombia. Facturación electrónica obligatoria para las comisiones de NAP. |
| **DoD** | Definition of Done | Definición de cuándo una tarea se considera "terminada" (criterios de aceptación del equipo). |
| **ERS** | Especificación de Requisitos de Software | Documento maestro con todos los requisitos funcionales y no funcionales (IEEE 830). |
| **FCF** | Free Cash Flow | Flujo de Caja Libre Positivo (hito financiero para empezar a pagar salarios). |
| **HTTPS** | Hypertext Transfer Protocol Secure | Protocolo de comunicación cifrado con TLS. |
| **IEEE** | Institute of Electrical and Electronics Engineers | Entidad que publica el estándar 830 para especificación de requisitos. |
| **IU** | Interfaz de Usuario | Código de pantalla del sistema (IU-01 a IU-14). |
| **JSONB** | JSON Binary | Tipo de dato PostgreSQL para almacenar JSON en formato binario (versiones de contratos). |
| **JWT** | JSON Web Token | Estándar de token de autenticación para APIs. |
| **KYC** | Know Your Customer | Proceso de verificación de identidad del usuario (carga y validación de documentos). |
| **MADR** | Markdown Architectural Decision Records | Formato en Markdown para documentar ADRs. |
| **MFA** | Multi-Factor Authentication | Autenticación de múltiples factores (ej. contraseña + código TOTP). |
| **MVP** | Minimum Viable Product | Producto Mínimo Viable: primera versión funcional de la plataforma. |
| **NDA** | Non-Disclosure Agreement | Acuerdo de confidencialidad. |
| **NIT** | Número de Identificación Tributaria | Identificación fiscal de empresas en Colombia. |
| **OCR** | Optical Character Recognition | Reconocimiento óptico de caracteres (para validar PILA en el futuro). |
| **OTP** | One-Time Password | Contraseña de un solo uso (firma electrónica simple). |
| **OWASP** | Open Web Application Security Project | Guía de mitigación de vulnerabilidades web. |
| **PILA** | Planilla Integrada de Liquidación de Aportes | Sistema de pago de seguridad social en Colombia (evolución futura). |
| **PMBOK** | Project Management Body of Knowledge | Estándar de gestión de proyectos. |
| **QA** | Quality Assurance | Aseguramiento de calidad (pruebas). |
| **RBAC** | Role-Based Access Control | Control de acceso basado en roles (cliente, profesional, empresa, admin, mediador). |
| **RF** | Requisito Funcional | Función o comportamiento que el sistema debe ofrecer (RF-001 a RF-060). |
| **RL** | Riesgo Legal | Identificador de riesgos legales/financieros (RL-01 a RL-06). |
| **RN** | Regla de Negocio | Política o restricción del dominio (RN-001 a RN-017). |
| **RNF** | Requisito No Funcional | Cualidad o restricción del sistema (RNF-001 a RNF-029). |
| **RT** | Riesgo Técnico | Identificador de riesgos técnicos/operacionales (RT-01 a RT-06). |
| **S.A.S.** | Sociedad por Acciones Simplificada | Tipo societario colombiano elegido para formalizar Nothing Sense. |
| **SLA** | Service Level Agreement | Acuerdo de nivel de servicio (ej. soporte a beta testers). |
| **SP** | Story Points | Unidad de estimación de esfuerzo en Scrum. |
| **T&C** | Terms and Conditions | Términos y condiciones de uso de la plataforma. |
| **TLS** | Transport Layer Security | Protocolo de cifrado para comunicaciones seguras. |
| **UAT** | User Acceptance Testing | Pruebas de aceptación de usuario (beta testers). |
| **UML** | Unified Modeling Language | Lenguaje de modelado unificado para diagramas de software. |
| **UTC** | Coordinated Universal Time | Zona horaria de referencia para marcas de tiempo en el sistema. |
| **WCAG** | Web Content Accessibility Guidelines | Pautas de accesibilidad web (meta: nivel AA). |

---

## 2. Roles del Equipo

| Nombre | Rol | Descripción |
|---|---|---|
| **Fredinson Solano** | CEO / Scrum Master | Fundador. Control estratégico, Regla de Cascadas, gestión del equipo, backlog y ceremonias Scrum. |
| **Steven Quiñones** | CTO / Backend Lead | Arquitectura tecnológica, backend Spring Boot, base de datos, integraciones (pagos, firma), decisiones de stack. |
| **Eduardo** | Frontend Lead | Desarrollo frontend Angular, wireframes en Figma (pendiente), diseño UI/UX, experiencia de usuario. |
| **Alcides** | Backend Developer | Desarrollo backend (Spring Boot, APIs, lógica de negocio). |
| **Andrés** | Frontend Developer | Desarrollo frontend (Angular, componentes, estilos Tailwind). |

---

## 3. Actores del Sistema (ERS)

| Actor | Sigla | Descripción |
|---|---|---|
| **Cliente individual** | CLI | Persona que publica una necesidad y contrata a un profesional. |
| **Profesional / Prestador** | PRO | Persona que ofrece servicios y se postula a necesidades. |
| **Usuario corporativo (empresa)** | EMP | Organización que gestiona contratos formales. |
| **Administrador** | ADM | Personal de la plataforma que la opera, configura y supervisa. |
| **Mediador** | MED | Rol que gestiona y resuelve disputas entre las partes. |
| **Pasarela de pago** | PAY | Sistema externo que procesa pagos (ePayco, Nequi). |
| **Proveedor de firma** | SIG | Sistema externo de firma electrónica certificada. |

---

## 4. Códigos de Requisitos

### 4.1 Requisitos Funcionales (RF-001 a RF-060)

| Código | Nombre | Prioridad | Módulo |
|---|---|---|---|
| **RF-001** | Registro de usuario individual | Alta | Usuarios |
| **RF-002** | Registro de usuario corporativo | Alta | Usuarios |
| **RF-003** | Verificación de identidad (KYC) | Alta | Usuarios |
| **RF-004** | Inicio de sesión | Alta | Usuarios |
| **RF-005** | Recuperación de contraseña | Media | Usuarios |
| **RF-006** | Autenticación multifactor (MFA) | Media | Usuarios |
| **RF-007** | Gestión de roles y permisos | Alta | Usuarios |
| **RF-008** | Cierre y suspensión de cuenta | Media | Usuarios |
| **RF-009** | Perfil profesional | Alta | Perfiles |
| **RF-010** | Perfil de empresa | Alta | Perfiles |
| **RF-011** | Catálogo de servicios y habilidades | Media | Perfiles |
| **RF-012** | Visualización pública de perfiles | Media | Perfiles |
| **RF-013** | Gestión de disponibilidad | Baja | Perfiles |
| **RF-014** | Publicación de necesidad | Alta | Marketplace |
| **RF-015** | Publicación de oferta de servicio | Media | Marketplace |
| **RF-016** | Búsqueda con filtros | Alta | Marketplace |
| **RF-017** | Emparejamiento y recomendaciones | Media | Marketplace |
| **RF-018** | Postulaciones y propuestas | Alta | Marketplace |
| **RF-019** | Mensajería interna | Media | Marketplace |
| **RF-020** | Generación desde plantilla simplificada | Alta | Contratos informales |
| **RF-021** | Definición de alcance, precio y plazo | Alta | Contratos informales |
| **RF-022** | Aceptación rápida del acuerdo | Alta | Contratos informales |
| **RF-023** | Seguimiento del estado | Media | Contratos informales |
| **RF-024** | Confirmación de cumplimiento | Alta | Contratos informales |
| **RF-025** | Biblioteca de plantillas formales | Alta | Contratos formales |
| **RF-026** | Editor de cláusulas y términos | Alta | Contratos formales |
| **RF-027** | Negociación y control de versiones | Alta | Contratos formales |
| **RF-028** | Flujo de aprobación multinivel | Media | Contratos formales |
| **RF-029** | Ciclo de vida del contrato | Alta | Contratos formales |
| **RF-030** | Alertas de vencimiento y renovación | Media | Contratos formales |
| **RF-031** | Gestión de hitos y obligaciones | Media | Contratos formales |
| **RF-032** | Repositorio documental con versionado | Alta | Contratos formales |
| **RF-033** | Firma electrónica de contratos | Alta | Firma |
| **RF-034** | Validación e integridad (hash) | Alta | Firma |
| **RF-035** | Registro de auditoría de la firma | Alta | Firma |
| **RF-036** | Múltiples firmantes | Media | Firma |
| **RF-037** | Registro de métodos de pago | Alta | Pagos |
| **RF-038** | Procesamiento de pagos | Alta | Pagos |
| **RF-039** | Custodia de fondos (escrow) | Media | Pagos |
| **RF-040** | Liberación por hitos o cumplimiento | Media | Pagos |
| **RF-041** | Facturación y comprobantes | Media | Pagos |
| **RF-042** | Historial de transacciones | Media | Pagos |
| **RF-043** | Calificación mutua | Media | Reputación |
| **RF-044** | Reseñas y comentarios | Baja | Reputación |
| **RF-045** | Cálculo de reputación | Media | Reputación |
| **RF-046** | Notificaciones en la aplicación | Media | Notificaciones |
| **RF-047** | Notificaciones por correo electrónico | Media | Notificaciones |
| **RF-048** | Preferencias de notificación | Baja | Notificaciones |
| **RF-049** | Apertura de disputa | Media | Disputas |
| **RF-050** | Gestión y mediación de disputas | Media | Disputas |
| **RF-051** | Registro de evidencias | Baja | Disputas |
| **RF-052** | Panel de control del usuario | Media | Reportes |
| **RF-053** | Reportes de contratos | Media | Reportes |
| **RF-054** | Indicadores corporativos | Baja | Reportes |
| **RF-055** | Exportación de reportes | Baja | Reportes |
| **RF-056** | Gestión de usuarios (admin) | Alta | Administración |
| **RF-057** | Gestión de plantillas y categorías | Media | Administración |
| **RF-058** | Moderación de contenido | Media | Administración |
| **RF-059** | Monitoreo y auditoría | Alta | Administración |
| **RF-060** | Configuración de parámetros | Media | Administración |

### 4.2 Requisitos No Funcionales (RNF-001 a RNF-029)

| Código | Nombre | Prioridad |
|---|---|---|
| **RNF-001** | Tiempo de respuesta (< 3s, 95%) | Alta |
| **RNF-002** | Usuarios concurrentes (5.000) | Alta |
| **RNF-003** | Capacidad transaccional | Alta |
| **RNF-004** | Tiempo de carga (< 2s) | Media |
| **RNF-005** | Aplicación web responsiva | Alta |
| **RNF-006** | Cumplimiento normativo (Ley 527, Ley 1581) | Alta |
| **RNF-007** | Estándares de desarrollo | Media |
| **RNF-008** | Navegadores soportados (Chrome, Firefox, Edge, Safari) | Media |
| **RNF-009** | Fiabilidad (integridad y consistencia) | Alta |
| **RNF-010** | Disponibilidad (≥ 99,5% mensual) | Alta |
| **RNF-011** | Cifrado en tránsito (TLS) | Alta |
| **RNF-012** | Protección de datos sensibles (hash, cifrado en reposo) | Alta |
| **RNF-013** | Control de acceso (RBAC, mínimo privilegio) | Alta |
| **RNF-014** | Mitigación OWASP Top 10 | Alta |
| **RNF-015** | Mantenibilidad (arquitectura modular) | Media |
| **RNF-016** | Portabilidad (despliegue en nube) | Media |
| **RNF-017** | Usabilidad e idioma (español) | Alta |
| **RNF-018** | Accesibilidad (WCAG 2.1 AA) | Media |
| **RNF-019** | Escalabilidad horizontal | Media |
| **RNF-020** | Privacidad y tratamiento de datos | Alta |
| **RNF-021** | Respaldo y recuperación ante desastres | Alta |
| **RNF-022** | Retención y archivo legal | Alta |
| **RNF-023** | Internacionalización (futuro) | Baja |
| **RNF-024** | Capacidad de almacenamiento | Media |
| **RNF-025** | Idempotencia de pagos | Alta |
| **RNF-026** | Observabilidad (trazas, métricas, logs) | Media |
| **RNF-027** | Retención de registros (auditoría) | Media |
| **RNF-028** | Límite de archivos adjuntos | Media |
| **RNF-029** | Zona horaria (UTC + presentación local) | Media |

### 4.3 Reglas de Negocio (RN-001 a RN-017)

| Código | Descripción |
|---|---|
| **RN-001** | KYC aprobado antes de firmar cualquier contrato. |
| **RN-002** | Aceptación de términos de uso y política de datos para registrarse. |
| **RN-003** | Comisión dinámica (~10% base, ajustable por promociones y tamaño). |
| **RN-004** | Fondos en custodia solo se liberan al confirmar cumplimiento o vencer plazo. |
| **RN-005** | Disputa activa congela la liberación de fondos. |
| **RN-006** | Contrato formal vigente solo cuando todas las partes firman. |
| **RN-007** | Autoconfirmación del acuerdo a los 3 días si el cliente no actúa. |
| **RN-008** | Reputación = promedio de calificaciones, visible solo con mínimo de valoraciones. |
| **RN-009** | Contratos visibles solo para las partes, mediador o admin. |
| **RN-010** | MFA obligatorio en firma y pagos. |
| **RN-011** | Usuario suspendido no puede publicar, postularse, firmar ni recibir pagos. |
| **RN-012** | Cada cambio aceptado genera nueva versión; versiones firmadas son inmutables. |
| **RN-013** | Contrato firmado no se elimina; se conserva el período legal. |
| **RN-014** | Moneda: COP. Importes no negativos. |
| **RN-015** | Cancelación sin penalidad antes de iniciar; en curso se rige por lo pactado. |
| **RN-016** | Disputa de mala fe: retención extra del 5% + suspensión temporal. |
| **RN-017** | Escrow y reputación aplican solo dentro de NAP; sin responsabilidad por transacciones externas. |

---

## 5. Códigos de Pantallas (Interfaz de Usuario)

| Código | Pantalla | Actores |
|---|---|---|
| **IU-01** | Registro / Inicio de sesión | Todos |
| **IU-02** | Verificación de identidad (KYC) | Cliente, Profesional, Empresa |
| **IU-03** | Panel de control (dashboard) | Cliente, Profesional, Empresa |
| **IU-04** | Perfil | Profesional, Empresa |
| **IU-05** | Publicar necesidad | Cliente |
| **IU-06** | Explorar / Buscar | Cliente, Profesional |
| **IU-07** | Detalle de necesidad y propuestas | Cliente, Profesional |
| **IU-08** | Mensajería interna | Cliente, Profesional, Empresa |
| **IU-09** | Editor de contrato | Cliente, Profesional, Empresa |
| **IU-10** | Firma electrónica | Cliente, Profesional, Empresa |
| **IU-11** | Pagos y custodia | Cliente, Profesional, Empresa |
| **IU-12** | Disputas | Cliente, Profesional, Empresa, Mediador |
| **IU-13** | Reportes | Empresa, Administrador |
| **IU-14** | Panel de administración | Administrador |

---

## 6. Códigos de Riesgos (Matriz de Gestión de Riesgos)

| Código | Descripción | Tipo |
|---|---|---|
| **RT-01** | Caída de pasarela de pagos (Nequi/ePayco) | Técnico |
| **RT-02** | Fuga de talento clave | Técnico |
| **RT-03** | Vulnerabilidad de ciberseguridad (fuga de datos) | Técnico |
| **RT-04** | Subestimación de tiempos de desarrollo | Técnico |
| **RT-05** | Fallas de integración Front/Back | Técnico |
| **RT-06** | Sobrecarga de servidores (picos de tráfico) | Técnico |
| **RL-01** | Demanda por pérdida de fondos | Legal |
| **RL-02** | Agotamiento de caja (Burn Rate) | Financiero |
| **RL-03** | Congelamiento de fondos por pasarela | Legal |
| **RL-04** | Demandas laborales por contratistas | Legal |
| **RL-05** | Fraudes por suplantación de identidad | Legal |
| **RL-06** | Baja adopción de usuarios en lanzamiento | Comercial |

---

## 7. Casos de Uso (CU-01 a CU-10)

| Código | Nombre | Actor principal |
|---|---|---|
| **CU-01** | Registrarse y verificar identidad | Cliente / Profesional / Empresa |
| **CU-02** | Publicar una necesidad | Cliente |
| **CU-03** | Postularse a una necesidad | Profesional |
| **CU-04** | Generar y cerrar acuerdo informal | Cliente / Profesional |
| **CU-05** | Crear y negociar contrato formal | Empresa / Profesional |
| **CU-06** | Firmar un contrato | Cliente / Profesional / Empresa |
| **CU-07** | Realizar y liberar un pago | Cliente |
| **CU-08** | Calificar a la otra parte | Cliente / Profesional |
| **CU-09** | Gestionar una disputa | Cliente / Profesional |
| **CU-10** | Administrar la plataforma | Administrador |

---

## 8. Decisiones de Arquitectura (ADR)

| Código | Decisión | Estado |
|---|---|---|
| **ADR-001.1** | Monolito modular (package-by-feature) | Aceptada |
| **ADR-001.2** | Spring Boot (Java 17+) | Aceptada |
| **ADR-001.3** | PostgreSQL 15+ | Aceptada |
| **ADR-001.4** | Angular (última LTS) + TypeScript | Aceptada |
| **ADR-001.5** | Tailwind CSS | Aceptada |
| **ADR-001.6** | Infraestructura: Supabase + Render + Vercel | Aceptada |
| **ADR-001.7** | Autenticación: Spring Security (no Supabase Auth) | Aceptada |
| **ADR-001.8** | Archivos: Cloudflare R2 | Aceptada |

---

## 9. Conceptos del Producto y del Negocio

| Término | Definición |
|---|---|
| **Acuerdo informal** | Contrato rápido y simple para necesidades puntuales (C2C). Estado: pendiente → en curso → entregado → finalizado/cancelado. |
| **Amigable composición** | Figura legal donde las partes aceptan que la decisión del mediador de NAP es vinculante para la liberación de fondos. |
| **Anillo 1 (Core Team)** | Equipo operativo fijo: Fredinson (CEO), Steven (CTO), Eduardo (Frontend Lead), Alcides, Andrés. |
| **Anillo 2 (Outsourcing)** | Consultores externos bajo demanda: abogada, contador, marketing. |
| **Autoconfirmación** | Si el cliente no confirma ni reclama en 3 días tras la entrega, el acuerdo se confirma automáticamente (RN-007). |
| **Beta Agreement** | Contrato de gratuidad temporal firmado por beta testers. |
| **Burn Rate** | Tasa de consumo de efectivo (se mitiga con Sweat Equity y Free Tiers). |
| **Captación masiva y habitual** | Delito en Colombia si NAP recibiera fondos en cuentas propias para escrow. Se evita con Split de Pagos. |
| **Comisión dinámica** | 10% base, se reduce automáticamente a 5-7% para montos > $3M COP. |
| **Contrato formal** | Acuerdo estructurado con ciclo de vida (laboral, prestación de servicios, confidencialidad, etc.). |
| **Custodia de fondos (Escrow)** | Retención del pago por la pasarela hasta que se cumplan las condiciones acordadas. |
| **Disputa de mala fe** | Usuario que pierde una disputa calificada de mala fe: 5% extra + suspensión temporal (RN-016). |
| **Elevator Pitch** | Discurso de venta de 60 segundos (Doc 16). |
| **Emparejamiento (matching)** | Conexión automática entre necesidades y profesionales por categoría y habilidades. |
| **Facturación electrónica DIAN** | Factura obligatoria por las comisiones que cobra NAP (API con Proveedor Tecnológico autorizado). |
| **Fiducia** | Modelo alternativo de custodia para el futuro (más burocrático, para contratos grandes). |
| **Firma electrónica certificada** | Con proveedor externo (Autentic/Certicámara), para contratos formales. Incluye sello de tiempo y hash. |
| **Firma electrónica simple** | Por OTP, clickwrap o logs. Para acuerdos informales. Sin proveedor externo. |
| **Gross Volume** | Volumen total de dinero transado en la plataforma (métrica de vanidad vs. Net Spread). |
| **Hito (milestone)** | Punto de avance verificable asociado a la liberación parcial de un pago. |
| **Idempotencia** | Propiedad por la que repetir un pago no lo duplica (RNF-025). |
| **Monto mínimo transaccional** | $30.000 COP (por debajo no es rentable por el spread). |
| **Net Spread** | Margen neto de NAP después de pagar comisiones de la pasarela. |
| **Regla de Cascadas** | Orden de distribución de ingresos: 1. Servidores, 2. Legal/Contable, 3. S.A.S., 4. Salarios. |
| **Sello de tiempo** | Marca confiable que certifica cuándo se firmó un documento (RF-034). |
| **Split de Pagos** | Modelo donde la pasarela retiene y dispersa los fondos directamente (NAP nunca toca el dinero). |
| **Sweat Equity** | Esfuerzo sin remuneración inicial a cambio de participación accionaria futura. |
| **Vesting** | Adquisición progresiva de derechos sobre acciones/opciones. |
| **Wireframes (Mockups)** | Diseños visuales de las 14 pantallas (pendiente — responsabilidad de Eduardo en Figma). |

---

## 10. Stack Tecnológico

| Capa | Tecnología | Versión/Detalle |
|---|---|---|
| **Arquitectura** | Monolito modular | Package-by-feature |
| **Backend** | Spring Boot | Java 17+, Gradle/Maven |
| **ORM** | Spring Data JPA / Hibernate | Consultas parametrizadas (seguridad) |
| **Auth** | Spring Security + JWT + TOTP | MFA, RBAC |
| **API Docs** | SpringDoc (OpenAPI) | Swagger |
| **Testing** | JUnit 5 + Mockito + Testcontainers | Unitarias + integración |
| **Base de datos** | PostgreSQL 15+ | Con índices cuidadosos |
| **Hosting DB** | Supabase | PostgreSQL gestionado (free tier) |
| **Frontend** | Angular | Última LTS, TypeScript |
| **Estilos** | Tailwind CSS | Con primitivos accesibles (Angular CDK) |
| **Hosting Frontend** | Vercel | CDN, builds automáticos |
| **Hosting Backend** | Render | Contenedor, git push |
| **Almacenamiento** | Cloudflare R2 | Compatible S3, 10 GB gratis, egress gratis |
| **Pasarela de pago** | ePayco (primario) / MercadoPago (respaldo) | Split de Pagos, Nequi para retiros |
| **Firma electrónica formal** | Autentic / Certicámara | Proveedor local certificado |
| **Firma electrónica respaldo** | DocuSign | Alternativa internacional |
| **Facturación DIAN** | Alegra / Siigo / Facturadora.com | Proveedor Tecnológico autorizado |
| **Control de versiones** | Git + GitHub | Repositorio nap-backend |

---

## 11. Entidades del Modelo de Datos

| Entidad | Descripción |
|---|---|
| **ACUERDO_INFORMAL** | Acuerdo rápido derivado de una propuesta aceptada. Estados: pendiente, en curso, entregado, finalizado, cancelado, en disputa. |
| **AUDITORIA** | Registro de acciones relevantes (autor, acción, entidad, marca de tiempo). |
| **CALIFICACION** | Valoración mutua entre partes al finalizar un contrato o acuerdo. |
| **CATEGORIA** | Clasificación de necesidades y servicios. |
| **CLAUSULA** | Cláusula individual dentro de una versión de contrato. |
| **CONTRATO_FORMAL** | Contrato estructurado con ciclo de vida. Estados: borrador, revisión, aprobación, pendiente firma, vigente, renovación, terminado, cancelado. |
| **CUSTODIA** | Retención de fondos en escrow. Estados: iniciado, retenido, liberado, reembolsado, rechazado, en disputa. |
| **DISPUTA** | Conflicto entre partes sobre un acuerdo o contrato. Estados: abierta, en mediación, resuelta, cerrada por acuerdo. |
| **EVIDENCIA** | Archivo o mensaje adjunto a una disputa. |
| **FIRMA** | Firma electrónica de una parte (con hash, sello de tiempo, IP). |
| **HITO** | Punto de avance verificable de un contrato, con fecha y monto asociado. |
| **MENSAJE** | Comunicación interna entre partes en la plataforma. |
| **NECESIDAD** | Requerimiento publicado por un cliente. |
| **NOTIFICACION** | Aviso a un usuario (tipo, canal, leído/no leído). |
| **OFERTA_SERVICIO** | Servicio ofrecido por un profesional. |
| **PAGO** | Transacción económica asociada a un acuerdo o contrato. |
| **PERFIL_EMPRESA** | Datos corporativos de una empresa (NIT, representantes). |
| **PERFIL_PROFESIONAL** | Habilidades, experiencia, portafolio de un profesional. |
| **PLANTILLA** | Base para generar contratos (simplificada o formal). |
| **PROPUESTA** | Oferta de un profesional a una necesidad (alcance, precio, plazo). |
| **ROL / ROL_USUARIO** | Roles del sistema y su asignación. |
| **TRANSACCION** | Movimiento financiero individual dentro de un pago. |
| **USUARIO** | Persona o empresa registrada en la plataforma. |
| **VERSION_CONTRATO** | Versión específica de un contrato durante la negociación. |

---

## 12. Estados del Sistema

### Contrato Formal
`Borrador → EnRevision → EnAprobacion → PendienteFirma → Vigente → EnRenovacion → Terminado`
`→ Cancelado` (desde PendienteFirma, desde Vigente)

### Acuerdo Informal
`Pendiente → EnCurso → Entregado → Finalizado`
`→ Cancelado` (desde Pendiente, desde EnCurso)
`→ EnDisputa` (desde Entregado)

### Pago en Custodia (Escrow)
`Iniciado → Retenido → Liberado`
`→ Rechazado` (desde Iniciado)
`→ EnDisputa → Liberado/Reembolsado` (desde Retenido)

### Disputa
`Abierta → EnMediacion → Resuelta`
`→ CerradaAcuerdo` (desde EnMediacion)

---

## 13. Historias del Backlog (NAP-XXX)

| ID | Historia | Épica | SP |
|---|---|---|---|
| **NAP-01** | Registro individual | Identidad y Acceso | 5 |
| **NAP-02** | Registro corporativo | Identidad y Acceso | 5 |
| **NAP-03** | Inicio de sesión | Identidad y Acceso | 3 |
| **NAP-04** | Roles y permisos | Identidad y Acceso | 5 |
| **NAP-05** | KYC (verificación de identidad) | KYC | 8 |
| **NAP-06** | Perfil profesional | Perfiles | 5 |
| **NAP-07** | Perfil de empresa | Perfiles | 3 |
| **NAP-08** | Biblioteca de plantillas | Contratos Formales | 3 |
| **NAP-09** | Editor de cláusulas | Contratos Formales | 8 |
| **NAP-10** | Negociación y versiones | Contratos Formales | 8 |
| **NAP-11** | Ciclo de vida del contrato | Contratos Formales | 5 |
| **NAP-12** | Repositorio documental | Contratos Formales | 5 |
| **NAP-13** | Firma electrónica | Firma Electrónica | 8 |
| **NAP-14** | Sello de tiempo y hash | Firma Electrónica | 5 |
| **NAP-15** | Auditoría de firma | Firma Electrónica | 3 |
| **NAP-16** | Publicar necesidad | Marketplace | 5 |
| **NAP-17** | Búsqueda con filtros | Marketplace | 5 |
| **NAP-18** | Postularse a necesidad | Marketplace | 5 |
| **NAP-19** | Generar acuerdo informal | Acuerdos Informales | 3 |
| **NAP-20** | Definir alcance/precio/plazo | Acuerdos Informales | 3 |
| **NAP-21** | Aceptar acuerdo | Acuerdos Informales | 2 |
| **NAP-22** | Confirmar cumplimiento | Acuerdos Informales | 3 |
| **NAP-23** | Método de pago | Pagos y Custodia | 5 |
| **NAP-24** | Procesar pago (escrow) | Pagos y Custodia | 8 |
| **NAP-25** | Gestión de usuarios (admin) | Administración | 5 |
| **NAP-26** | Auditoría de acciones | Administración | 3 |

---

## 14. Documentos del Repositorio

### Documentación Empresarial (21 docs)

| Doc | Archivo | Descripción |
|---|---|---|
| 01 | `01_Manual_Roles_y_Funciones.md` | Roles del equipo y funciones |
| 02 | `02_Ruta_Legalizacion_Empresarial.md` | Hoja de ruta de constitución formal |
| 03 | `03_Proyeccion_Estrategica_Anual.md` | Proyección a 12 meses |
| 04 | `04_Modelo_de_Negocio.md` | Arquitectura de ingresos |
| 05 | `05_Manual_Buenas_Practicas_y_Formatos_Dev.md` | Estándares de código y formatos dev |
| 06 | `06_Manual_Operaciones_CEO.md` | Rituales semanales y control del CEO |
| 07 | `07_Matriz_Gestion_de_Riesgos.md` | Riesgos técnicos, legales y financieros |
| 08 | `08_Plantilla_Presupuesto_MVP.md` | Presupuesto del MVP |
| 09 | `09_Backlog_y_WBS.md` | WBS del proyecto |
| 10 | `10_Plan_Gestion_Stakeholders.md` | Mapa de interesados |
| 11 | `11_Manual_Operaciones_Consultores.md` | Marco para consultores externos |
| 12 | `12_Plan_Gestion_Comunicaciones_y_Cambios.md` | Matriz de comunicaciones y DoD |
| 13 | `13_Diagnostico_Ejecutivo_y_Faltantes.md` | Auditoría del estado del proyecto |
| 14 | `14_Matriz_Analisis_Competitivo.md` | Análisis de competencia |
| 15 | `15_Estructura_Matematica_Pricing.md` | Pricing y spread |
| 16 | `16_Elevator_Pitch_y_Guion_Ventas.md` | Discurso de ventas |
| 17 | `17_Plan_Gestion_Configuracion.md` | Gestión de configuración |
| 18 | `18_Formato_Unico_Aprobacion_KYC.md` | Formato de aprobación KYC |
| 19 | `19_Propuesta_de_Valor.md` | Propuesta de valor |
| 20 | `20_Proyeccion_Financiera_y_Salarial.md` | Proyección financiera |
| 21 | `21_Plan_Reclutamiento_Beta_Testers.md` | Plan UAT |

### Seguimiento

| Archivo | Descripción |
|---|---|
| `INDICE_SEGUIMIENTO.md` | Índice cronológico de sprints |
| `templates/plantilla-acta-reunion.md` | Plantilla para actas de ceremonias |
| `templates/plantilla-reporte-diario.md` | Plantilla para daily de cada dev |
| `templates/instructivo-reporte-diario.md` | Guía para llenar el reporte diario |
| `templates/plantilla-weekly-sync.md` | Plantilla para sync semanal Leads → CEO |
| `sprint-01/backlog-sprint-01.md` | Backlog del Sprint 1 (26 US) |
| `sprint-01/reportes/daily-dev-steven.md` | Reporte diario — Steven (CTO) |
| `sprint-01/reportes/daily-dev-eduardo.md` | Reporte diario — Eduardo (Frontend Lead) |
| `sprint-01/reportes/daily-dev-alcides.md` | Reporte diario — Alcides (Backend Dev) |
| `sprint-01/reportes/daily-dev-andres.md` | Reporte diario — Andrés (Frontend Dev) |
| `sprint-01/reportes/daily-ceo-fredinson.md` | Reporte ejecutivo — Fredinson (CEO) |

### Raíz

| Archivo | Descripción |
|---|---|
| `ERS_NAP_IEEE830.md` | Especificación de Requisitos (IEEE 830) |
| `ERS_NAP_IEEE830_v1.1.md` | Versión 1.1 (actualizada) |
| `ADR_Stack_Tecnologico_NAP.md` | Decisiones de arquitectura (8 ADR) |
| `INDICE_MAESTRO.md` | Mapa completo del repositorio |

---

## 15. Términos Legales

| Término | Definición |
|---|---|
| **Ley 527 de 1999** | Comercio electrónico y firmas digitales en Colombia. |
| **Ley 1581 de 2012** | Protección de datos personales en Colombia. |
| **Captación masiva y habitual** | Delito financiero que NAP evita mediante Split de Pagos. |
| **Cedula de ciudadanía** | Documento de identidad colombiano para KYC. |
| **RUT** | Registro Único Tributario (para KYC de profesionales). |
| **Responsabilidad solidaria** | Riesgo legal si un contratista no paga seguridad social (PILA). |
| **Superintendencia Financiera** | Ente que regula las pasarelas de pago en Colombia. |
| **Bad Leaver** | Socio que incumple y pierde derechos accionarios. |
| **Propiedad Intelectual (IP)** | Todo el código pertenece a Nothing Sense, no a los desarrolladores. |
| **Términos de uso (T&C)** | Reglas de la plataforma que el usuario acepta al registrarse. |
| **Política de Tratamiento de Datos** | Documento de privacidad (Ley 1581). |

---

## 16. Nombres de Proveedores Externos

| Proveedor | Uso | Tipo |
|---|---|---|
| **ePayco** | Pasarela de pago primaria (Split de Pagos) | Nacional |
| **Nequi** | Retiro de fondos para profesionales (alta adopción) | Nacional |
| **MercadoPago** | Pasarela de respaldo | Regional |
| **Autentic** | Firma electrónica certificada (prioritario) | Nacional |
| **Certicámara** | Firma electrónica certificada (alternativa) | Nacional |
| **DocuSign** | Firma electrónica (plan B internacional) | Global |
| **Alegra** | Facturación electrónica DIAN | Nacional |
| **Siigo** | Facturación electrónica DIAN (alternativa) | Nacional |
| **Facturadora.com** | Facturación electrónica DIAN (alternativa) | Nacional |
| **Supabase** | Hosting de PostgreSQL | Global |
| **Render** | Hosting del backend Spring Boot | Global |
| **Vercel** | Hosting del frontend Angular | Global |
| **Cloudflare R2** | Almacenamiento de documentos (archivos) | Global |
| **Figma** | Diseño de wireframes y mockups (herramienta) | Global |
| **Jira** | Gestión de proyectos Scrum (herramienta) | Global |

---

## 17. Abreviaciones de Carpetas

| Ruta | Contenido |
|---|---|
| `Raíz (/nap-backend)` | ERS + ADR + Índice Maestro |
| `Documentacion_Empresarial/` | 21 documentos de negocio (01-21) |
| `Documentacion Nothing Sense/` | Plan gerencial + acuerdo confidencialidad |
| `Documentos_Legales/` | 12 contratos legales (fundadores, consultores, términos) |
| `Seguimiento/` | Reportes, actas, backlog y plantillas del equipo |
| `Seguimiento/sprint-01/` | Backlog + actas + reportes del Sprint 1 |

---

> **Última actualización:** 2026-06-22
> **Mantenido por:** Fredinson Solano (CEO) / Steven Quiñones (CTO)
> **Instrucción:** Este diccionario debe actualizarse cada vez que se agregue un término nuevo a la documentación del proyecto.
