# Plan de Gestión Directiva y Operacional (Project Management Plan)

**Entidad Promotora:** Nothing Sense (S.A.S. en Formación)
**Iniciativa Estratégica:** Según proyecto (actual: Plataforma NAP)
**Autor / Aprobador:** Fredinson Solano Rois (CEO / Ing. Civil, Especialista y Magíster en Gerencia de Proyectos)
**Co-Fundador Técnico:** Steven Ricardo Quiñones (Ing. de Sistemas)

---

## 0. Identidad Corporativa

### Propósito
Crear software con identidad propia —donde cada línea de código refleje quiénes somos— mientras crecemos como profesionales y generamos ingresos sostenibles.

### Misión
Desarrollar soluciones de software que resuelvan problemas reales del contexto colombiano, con altos estándares de calidad técnica y diseño, dando a conocer nuestra autoría y construyendo una fuente de ingresos estable para el equipo.

### Visión
Ser un estudio de desarrollo de software reconocido en Colombia por la calidad de sus productos, la autoría propia de sus soluciones y el crecimiento continuo de sus miembros. Nothing Sense no es solo NAP; es el primero de muchos proyectos con nuestra firma.

### Valores
- **Autoría y orgullo:** No somos solo ejecutores, somos creadores. Cada proyecto lleva nuestra firma.
- **Sentido donde otros no ven nada:** El mercado laboral tradicional "no tiene sentido" (Nothing Sense). Construimos nuestro propio camino, con reglas claras y propósito.
- **Hecho en Colombia:** Entendemos nuestro contexto y construimos para él. Sin copiar modelos foráneos.
- **Simple, directo, sin burocracia:** Soluciones limpias, sin vueltas.
- **Trabajo digno:** Esto es también un negocio. Generar ganancias nos permite seguir creando.

---

## 1. Resumen Ejecutivo y Origen de la Entidad

**Nothing Sense** nace como un emprendimiento tecnológico (*Startup*) originado a partir de la sinergia estratégica entre la ingeniería de sistemas (liderada por Steven Ricardo) y la gerencia integral de proyectos (liderada por Fredinson Solano). El núcleo fundacional opera bajo un esquema de cercanía ("grupo de amigos y familiares"), pero se estructura bajo rigurosos estándares corporativos para asegurar su viabilidad comercial. El objetivo es desplegar la plataforma NAP minimizando el riesgo financiero inicial (*Bootstrapping*) y maximizando el retorno de inversión a través de una ejecución ágil.

## 2. Mapa de Recursos Humanos (Matriz de Adquisición de Personal)

Para la puesta en marcha (*Go-To-Market*) y escalamiento de NAP, la gerencia proyecta una estrategia de recursos humanos dividida en dos anillos de responsabilidad:

### Anillo 1: Núcleo Operativo Fijo (Core Team)
El equipo actual asume el riesgo inicial (*Sweat Equity*) y es el motor del desarrollo.
- **CEO & Project Manager:** Fredinson Solano (Dirección corporativa, validación de negocio, estrategia).
- **Backend Tech Lead:** Steven Ricardo Quiñones (Arquitectura de software, DevOps, liderazgo técnico del lado del servidor).
- **Frontend Tech Lead:** Eduardo Morales (UI/UX, familiar directo con responsabilidades limitadas exclusivamente a la ejecución técnica de su célula frontend).
- **Desarrollador Backend:** (Soporte operativo para la Célula Backend, reportando a Steven).

### Anillo 2: Consultores Externos y Servicios Bajo Demanda (Outsourcing)
Para evitar la carga prestacional prematura y mantener el modelo *Lean*, se han perfilado recursos de confianza profesional (círculo cercano del CEO) que prestarán servicios por honorarios u horas, activados estratégicamente ante hitos regulatorios o de despliegue comercial:
- **Asesoría Legal y *Compliance* (Abogada externa - Ex pareja):** Revisión de Contratos Comerciales, Política de Datos (Ley 1581), elaboración de Términos y Condiciones, y formalización societaria ante Cámara de Comercio.
- **Asesoría Contable y Financiera (Contador externo - Amigo):** Estructuración tributaria ante la DIAN, vinculación técnica de facturación electrónica y liquidación de impuestos corporativos.
- **Dirección de Marketing y Estrategia B2B (Administradora de Empresas):** Planificación de campañas para el lanzamiento C2C, relacionamiento corporativo y estrategias de conversión comercial.

## 3. Estructura de Desglose de Trabajo (EDT / WBS) — Marco Genérico

La siguiente EDT es un marco genérico aplicable a cualquier proyecto de software que desarrolle Nothing Sense. Los paquetes de trabajo (Work Packages) se ajustan según la naturaleza y alcance de cada proyecto. A continuación se presenta la EDT base con el proyecto actual (NAP) como ejemplo.

| Código | Paquete de Trabajo (Work Package) | Responsable | Duración (Semanas) |
| :--- | :--- | :--- | :--- |
| **WP-1.0** | **Planeación, Arquitectura y Setup Inicial** | Líder Técnico / Gerente | 2 |
| **WP-2.0** | **Diseño de Experiencia de Usuario (UX/UI)** | Frontend Lead | 3 |
| **WP-3.0** | **Core de Negocio (IAM, Roles, Auth)** | Backend Lead | 4 |
| **WP-4.0** | **Motor Transaccional (Lógica de negocio principal)** | Backend + Frontend | 5 |
| **WP-5.0** | **Integraciones Externas (Pagos, APIs, servicios)** | Líder Técnico | 3 |
| **WP-6.0** | **Cumplimiento Legal y Documentación** | Consultores / Gerente | 2 |
| **WP-7.0** | **Pruebas de Integración (QA) y UAT** | Todo el equipo | 3 |
| **WP-8.0** | **Go-Live, Marketing y Despliegue Producción** | Equipo + Consultores | 2 |

> *Los WPs técnicos (2, 3 y 4) se ejecutan en metodologías iterativas (Sprints) permitiendo el paralelismo entre Frontend y Backend mediante diseño de interfaces por contratos (API Contracts). Las duraciones y responsables se ajustan por proyecto.*

## 4. Repositorio Documental Exigido (Activos de los Procesos de la Organización - OPA)

Para garantizar la retención del conocimiento y facilitar el abordaje corporativo, la gerencia exige la consolidación y actualización de los siguientes artefactos vivos:

1. **Documentación Técnica:** Especificación de Requisitos de Software (ERS), Diagrama Entidad-Relación (DER) consolidado, Documentación de API (Swagger/OpenAPI) y Componentes UI (Figma).
2. **Documentación Legal y Operativa:** Acuerdos Fundacionales (MoU), Términos y Condiciones, Acuerdos de Nivel de Servicio (SLA) y Manual Interno de Resolución de Disputas Comerciales.
3. **Documentación Comercial:** *Pitch Deck* Ejecutivo (10 diapositivas para B2B), Modelo Financiero Base (Flujo de caja proyectado) y Plan de Medios/Lanzamiento.

---
*Aprobado por Gerencia - Framework fundamentado en el Project Management Institute (PMI) aplicable a marcos de trabajo ágiles.*
