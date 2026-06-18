# Presupuesto Base y Flujo de Caja del MVP (Cost Baseline)

Para mantener el control del "Burn Rate", el CEO debe registrar y vigilar los costos operativos. Durante la fase de desarrollo e iteración inicial (Mes 1 al 4), el objetivo estratégico es mantener la infraestructura técnica en **$0 COP**, aprovechando las capas gratuitas (*Free Tiers*) de proveedores globales.

## 1. Costos de Infraestructura Técnica (Proyección)
| Ítem / Servicio | Funcionalidad en el Proyecto | Costo en Fase Desarrollo | Costo Proyectado Producción |
| :--- | :--- | :--- | :--- |
| **Base de Datos (SQL)** | Almacenamiento seguro de contratos | $0 (Supabase / Render Free) | ~$20 - $50 USD / mes |
| **Alojamiento Servidor** | Ejecución de lógica Backend / APIs | $0 (Render / Railway Free) | ~$10 - $20 USD / mes |
| **Alojamiento Cliente** | Despliegue de aplicación Frontend | $0 (Vercel / Netlify Free) | $0 - $20 USD / mes |
| **Servicio de Correos** | Notificaciones OTP (Factor Doble) | $0 (Resend / SendGrid Free) | Variable (Por volumen) |
| **Dominio y SSL** | Direccionamiento (ej. `nothingsense.co`) | ~$15 - $30 USD (Gasto Anual) | Anualizado |

## 2. Costos Variables Comerciales (C2C / B2B)
| Ítem / Servicio | Uso Estratégico | Asignación del Costo |
| :--- | :--- | :--- |
| **Pasarela (ePayco/Nequi)** | Gestión de pagos y custodia (*Escrow*) | ~2.99% + 900 COP. Se traslada como costo oculto al usuario o se deduce de la comisión de NAP. |
| **Proveedor de Firmas** | Firma Electrónica Certificada local | Pago por uso (Cobrado al cliente dentro de la transacción). |

## 3. Directriz de Cero Gasto Prematuro
- **Fase Semilla:** Toda compra de suscripciones de software, licenciamiento o ampliación de capacidad de servidores está temporalmente **congelada**. Los Tech Leads (Steven y Eduardo) tienen la directriz de programar bajo optimización máxima para no agotar las capas gratuitas.
- **Autorización de Escalamiento:** El CEO autorizará migrar las bases de datos y servidores a capas de cobro (*Upgrades*) únicamente cuando el volumen transaccional de NAP empiece a generar ingresos de comisiones suficientes para absorber el costo tecnológico (*Punto de Equilibrio*).
