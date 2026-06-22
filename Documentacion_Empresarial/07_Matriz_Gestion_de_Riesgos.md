# Matriz de Gestión de Riesgos Corporativos y Técnicos (Ampliada)

Este documento es un artefacto vivo que debe ser revisado mensualmente por el CEO y los Tech Leads para anticipar amenazas a la plataforma NAP y activar los planes de mitigación o contingencia correspondientes.

## 1. Riesgos de Ejecución Técnica y Operacional
| ID | Descripción del Riesgo | Probabilidad | Impacto | Plan de Mitigación (Contingencia) | Responsable |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **RT-01** | Caída prolongada de la pasarela de pagos (Nequi/ePayco). | Media | Alto | Mostrar banner de "Mantenimiento Bancario", pausar autoconfirmaciones de 3 días y extender plazos temporalmente. | Backend Lead |
| **RT-02** | Fuga de talento clave (Salida de un desarrollador). | Baja | Alto | Documentación estricta (Swagger) y cesión de IP para rápida integración de reemplazo. | CEO / Tech Leads |
| **RT-03** | Vulnerabilidad de ciberseguridad (Fuga de datos). | Baja | Crítico | Encriptación (JWT, Bcrypt), prevención de inyecciones SQL (JPA/Hibernate parametrizado) y backups diarios. | Backend Lead |
| **RT-04** | Subestimación de tiempos de desarrollo (Retraso). | Alta | Medio | Aplicar metodología Ágil, priorización MoSCoW (Must/Should/Could/Won't) y *Sprints* de 2 semanas. | CEO / Tech Leads |
| **RT-05** | Fallas de integración y cuellos de botella entre Front y Back. | Media | Alto | Definir "API Contracts" (Swagger) estrictos antes de escribir código visual. Usar Mock APIs. | Tech Leads |
| **RT-06** | Sobrecarga de Servidores (Picos de Tráfico). | Baja | Medio | Configurar Auto-escalamiento en el proveedor de hosting (Render + Vercel). Optimización e indexación de queries SQL. | Backend Lead |

## 2. Riesgos Legales, Financieros y Comerciales
| ID | Descripción del Riesgo | Probabilidad | Impacto | Plan de Mitigación (Contingencia) | Responsable |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **RL-01** | Demanda por pérdida de fondos o disputa en acuerdo C2C. | Alta | Medio | Escudarse en T&C (NAP como mero intermediario). Activar Consultora Legal ante PQRs formales. | CEO / Legal |
| **RL-02** | Agotamiento de caja (*Burn Rate*) previo al lanzamiento. | Media | Alto | Mantener *Sweat Equity* y servidores en *Free Tiers* hasta validación de mercado. | CEO |
| **RL-03** | Congelamiento de fondos por la pasarela (Alerta Lavado Activos). | Baja | Crítico | Aplicar verificación KYC estricta desde el Backend; trazabilidad financiera transparente. | Contable / CEO |
| **RL-04** | Riesgo de demandas laborales por contratistas (Reclamación de vínculo). | Media | Crítico | Contratos blindados como prestación de servicios independientes, sin horario fijo ni subordinación. | CEO / Legal |
| **RL-05** | Fraudes por suplantación de identidad en la plataforma (Cuentas falsas). | Alta | Alto | Integrar biometría facial / validación de cédula contra base de datos registral (API de terceros) en el Onboarding. | Backend Lead |
| **RL-06** | Baja adopción de usuarios en el lanzamiento (Fracaso Beta). | Media | Alto | Campaña de marketing hiper-segmentada (B2B). Iteración rápida basada en *Feedback* de usuarios. | Mkt / CEO |
