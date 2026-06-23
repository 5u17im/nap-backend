# Landing Page — Nothing Sense

**Versión:** 1.0
**Fecha:** Junio 2026
**Destinatario:** Eduardo (Frontend Lead)
**Propósito:** Brief completo con copy, estructura y especificaciones para el desarrollo de la landing page.

---

## 1. Información General

| Aspecto | Detalle |
|---|---|
| **URL sugerida** | nothingsense.co |
| **Stack frontend** | Angular + Tailwind CSS |
| **Hosting** | Vercel |
| **Idioma** | Español (Colombia) |
| **Analytics** | Google Analytics 4 (configurar desde el inicio) |
| **Formulario de contacto** | Enviar a correo de Fredinson y Steven |

### Objetivos de la Landing Page

1. Presentar Nothing Sense como estudio de desarrollo de software con identidad.
2. Presentar NAP como producto insignia y generar leads B2B (empresas beta).
3. Atraer talento técnico interesado en sumarse al equipo.
4. Ser la carta de presentación profesional para aliados, inversores y clientes de desarrollo de software.

---

## 2. Estructura de la Página

### 2.1. Navegación (Header)

Logo "Nothing Sense" (izquierda) + menú enlace de ancla:

| Enlace | Sección destino | Prioridad |
|---|---|---|
| Inicio | Hero | Siempre visible |
| Nosotros | Quiénes somos | Alta |
| NAP | Producto | Alta |
| Equipo | Equipo | Alta |
| Contacto | Formulario | Alta |

Comportamiento: menú responsivo. En móvil, hamburguesa. Navbar sticky con fondo al hacer scroll.

---

### 2.2. Sección 1 — Hero

**Objetivo:** Que el visitante entienda en 3 segundos qué es Nothing Sense.

**Diseño sugerido:**
- Fondo oscuro (casi negro) con un elemento visual llamativo (geometría simple, el signo de interrogación del logo, o un patrón sutil).
- Texto blanco, grande, sans-serif.

**Copy:**

> **Nothing Sense**
>
> *Software con identidad.*
>
> Creamos soluciones de software hechas en Colombia, con autoría propia y estándares de calidad que nos exigen ser mejores en cada proyecto.
>
> [Conoce NAP →] [Trabaja con nosotros →]

*(Dos botones CTA: el principal lleva a sección NAP, el secundario a contacto)*

---

### 2.3. Sección 2 — Quiénes Somos

**Diseño sugerido:**
- Fondo claro o blanco.
- Dos columnas en desktop: texto + imagen del equipo o ilustración.

**Copy:**

> **Somos Nothing Sense. Construimos software por convicción.**
>
> Nothing Sense nació en la Costa Caribe colombiana, entre Montería, Valledupar y La Guajira, como respuesta a una pregunta simple: ¿por qué tenemos que conformarnos con trabajos que no nos llenan o con soluciones que no entienden nuestro contexto?
>
> Somos un estudio de desarrollo de software, no una agencia de outsourcing. Cada proyecto lleva nuestra firma porque creemos en lo que hacemos. NAP es nuestro primer producto, pero no el último.

**Elementos visuales:** Foto del equipo (o ilustración representativa de la Costa Caribe + código).

---

### 2.4. Sección 3 — NAP (El Producto)

**Diseño sugerido:**
- Fondo oscuro o con acento de color.
- Tarjetas o íconos para cada funcionalidad.

**Copy:**

> **NAP: Acuerdos sin vueltas.**
>
> Una plataforma que conecta a quien necesita un servicio con quien lo resuelve, y formaliza todo el ciclo: desde la búsqueda hasta el pago.

**Las 4 funciones clave (en tarjetas):**

| Ícono | Título | Descripción breve |
|---|---|---|
| 🔍 | Encuentra | Publica tu necesidad o servicio y conéctate con la persona indicada. |
| 📝 | Formaliza | Contratos desde plantillas, desde acuerdos rápidos hasta contratos corporativos. |
| 🔒 | Paga con protección | Los fondos van a una custodia y se liberan solo cuando ambas partes cumplen. |
| ✍️ | Firma con validez | Firma electrónica con respaldo legal y registro de auditoría. |

> [Quiero ser empresa beta →] (botón que lleva a formulario de contacto)

---

### 2.5. Sección 4 — Equipo

**Diseño sugerido:**
- Fondo claro.
- Grid de 3 tarjetas (una por fundador), cada una con foto, nombre, rol y ciudad.

**Copy (título de sección):**

> **Tres fundadores, tres ciudades, una visión.**

**Tarjetas:**

| Nombre | Rol | Ciudad |
|---|---|---|
| Fredinson Solano Rois | CEO — Gerencia de Proyectos | Valledupar |
| Steven Ricardo Quiñones | CTO — Arquitectura y Backend | Montería |
| Eduardo [Apellido] | Frontend Lead — Experiencia de Usuario | La Guajira |

*Sin fotos aún — usar placeholder o ilustración mientras se toman fotos profesionales.*

---

### 2.6. Sección 5 — Contacto

**Diseño sugerido:**
- Fondo oscuro.
- Formulario simple (3 campos: nombre, correo, mensaje).
- Botón de envío.

**Copy:**

> **Trabajemos juntos.**
>
> ¿Eres una empresa interesada en NAP? ¿Tienes un proyecto de software? ¿Quieres sumarte al equipo?
>
> [Nombre]
> [Correo electrónico]
> [Mensaje]
>
> [Enviar →]

*El formulario envía un correo a la dirección que definan los fundadores.*

---

### 2.7. Footer

**Copy mínimo:**

> **Nothing Sense**
> *Software con identidad.*
>
> Montería, Córdoba — Colombia
>
> [LinkedIn] [GitHub] [Correo]
>
> © 2026 Nothing Sense. Todos los derechos reservados.

---

## 3. Especificaciones Técnicas para Eduardo

### Diseño Responsive

| Breakpoint | Dispositivo | Comportamiento |
|---|---|---|
| < 768px | Móvil | Layout de una columna, menú hamburguesa, texto ajustado |
| 768px - 1024px | Tablet | Dos columnas donde sea posible |
| > 1024px | Desktop | Layout completo |

### Paleta de Colores

*Pendiente de definir valores exactos en Manual de Marca. Mientras tanto, usar:*

| Uso | Color sugerido |
|---|---|
| Fondo hero y footer | #0D0D0D (casi negro) |
| Fondo secciones claras | #FFFFFF |
| Texto sobre fondo oscuro | #FFFFFF |
| Texto sobre fondo claro | #1A1A1A |
| Color acento (botones, detalles) | #00BFA6 (verde menta) o #FF6B35 (naranja) — por decidir |
| Fondo tarjetas equipo | #F5F5F5 |

### Tipografía

- **Títulos:** Inter o Montserrat (sans-serif geométrica)
- **Cuerpo:** Inter
- Usar Google Fonts. Tamaños: h1 ~48px, h2 ~36px, body ~16px, ajustar en móvil.

### Animaciones (opcional, baja prioridad)

- Fade-in sutil al hacer scroll (usar Intersection Observer o librería como AOS).
- Transición suave del menú sticky.
- Sin animaciones complejas que afecten rendimiento.

### SEO

| Aspecto | Valor sugerido |
|---|---|
| Title | Nothing Sense — Software con Identidad |
| Description | Estudio colombiano de desarrollo de software. Creadores de NAP, la plataforma de gestión y creación de contratos con protección de pagos y firma electrónica. |
| Keywords | desarrollo de software Colombia, contratos electrónicos, plataforma contratos, firma electrónica, escrow, Nothing Sense, NAP |
| Open Graph | Imagen 1200x630px del logo o del equipo |
| Canonical | URL principal |

### Rendimiento

- Lazy loading en imágenes.
- Compresión de assets.
- Minimizar CSS y JS (Angular build optimizado ya lo hace).
- Tiempo de carga objetivo: < 2 segundos.

---

## 4. Contenido Adicional (Futuras Iteraciones)

Para posteriores versiones de la landing page:

- **Blog / Notas técnicas:** Artículos del equipo sobre desarrollo, tecnología y el mercado colombiano.
- **Casos de éxito de NAP:** Cuando haya clientes beta.
- **Página de producto NAP con más detalle:** Cuando la plataforma esté operativa.
- **Sección de precios de NAP:** Cuando el modelo de monetización esté activo.
