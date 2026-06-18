# Formato Único Corporativo: Aprobación KYC y Antifraude (Know Your Customer)

Este procedimiento garantiza el cumplimiento de la política de prevención de lavado de activos y blindaje contra suplantación de identidad en la plataforma NAP.

---
**ID USUARIO A VERIFICAR:** [UID_Plataforma]
**CORREO ELECTRÓNICO:** [Email]
**TIPO DE PERFIL:** [C2C / B2B Empresa]

### 1. Validación Documental (Cotejo de Identidad)
Para permitir que el usuario firme contratos electrónicos y movilice dinero, debe superar las siguientes validaciones automatizadas o manuales (por Backoffice):

- [ ] **Validación de Cédula:** El número de Cédula de Ciudadanía / Extranjería cargado coincide exactamente con el nombre de registro.
- [ ] **Prueba de Vida (Liveness Check):** La "selfie" o captura facial tomada en vivo coincide biométricamente con la fotografía del documento de identidad cargado.
- [ ] **Cruce de Listas de Riesgo:** El número de documento **NO** aparece registrado en la "Lista Clinton", Interpol, o listas restrictivas de la Fiscalía General de la Nación (Prevención LA/FT).

### 2. Validación de Contacto (MFA)
- [ ] Verificación de Correo Electrónico (Link de confirmación / OTP validado).
- [ ] Verificación de Número de Teléfono (SMS OTP validado con indicativo +57).

### 3. Veredicto Antifraude
- [ ] **APROBADO:** El usuario cumple con el nivel de confianza (Trust Level 1) y se le habilitan las funcionalidades de creación de contratos formales e informales, y recepción de pagos.
- [ ] **RECHAZADO / CUENTA BLOQUEADA:** Se encontraron discrepancias graves (Documento forjado, robo de identidad o figuración en listas de riesgo). 
  - **Motivo del Rechazo:** __________________________________

### 4. Responsabilidad Legal
*En cumplimiento con la Ley 1581 de 2012, el registro facial y documental será encriptado, protegido por el Backend Tech Lead, y utilizado exclusivamente para fines probatorios en caso de demandas civiles derivadas de un contrato firmado en la plataforma.*

---
**Sello Digital del Motor Antifraude o Agente Operativo:**
[Timestamp de Aprobación]
