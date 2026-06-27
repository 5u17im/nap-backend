# Especificaciones de Diseño — Pendientes Eduardo

**Documento:** Para ser diligenciado por Eduardo (Frontend Lead)
**Propósito:** Registrar las decisiones de diseño visual que Eduardo tome para Nothing Sense y NAP.

---

## 1. Logotipo

| Aspecto | Decisión |
|---|---|
| Concepto / Idea principal | |
| Tipo (isologo / imagotipo / logotipo) | |
| Archivo fuente (FIG / AI / SVG) | |
| Variante horizontal (ancho) | |
| Variante vertical / isotipo (icono solo) | |
| Versión en blanco y negro / negativo | |

## 2. Paleta de Colores — "Forest Whispers"

| Rol | Hex | RGB | Uso |
|---|---|---|---|
| **Primario / Texto principal** | `#0D0D0D` | `rgb(13, 13, 13)` | Texto, fondos oscuros, header, footer. 17.2:1 ✅ AAA |
| **Secundario / Texto secundario** | `#424750` | `rgb(66, 71, 80)` | Subtítulos, metadata. 8.3:1 ✅ AAA |
| **Fondo claro** | `#F3F0F5` | `rgb(243, 240, 245)` | Fondo principal, tarjetas, secciones |
| **Acento brillante** | `#70B924` | `rgb(112, 185, 36)` | Botones CTA sobre **fondo oscuro** (texto negro). ⚠️ Falla AA con blanco (2.43:1) |
| **Acento oscuro** | `#3B7A24` | `rgb(59, 122, 36)` | Botones CTA sobre **fondo claro** / texto blanco ✅ AA. Enlaces inline |

### Reglas de uso por contexto

| Contexto | Fondo | Acento a usar | Texto |
|---|---|---|---|
| Header / Hero | `#0D0D0D` | `#70B924` (brillante) | `#F3F0F5` |
| Secciones claras | `#F3F0F5` | `#3B7A24` (oscuro) | `#0D0D0D` |
| CTA primario (donde sea) | `#3B7A24` | — | Blanco `#FFFFFF` ✅ 5.26:1 |
| CTA secundario (outline) | transparente | borde `#3B7A24` | `#3B7A24` ✅ 4.65:1 |
| Enlaces inline | — | `#3B7A24` | — ✅ 4.65:1 |
| Hover de botones | `#2E5E1A` | — | Blanco `#FFFFFF` ✅ 6.5:1+ |

## 3. Tipografía

| Uso | Fuente | Peso | Tamaño (Desktop) | Tamaño (Móvil) |
|---|---|---|---|---|
| Títulos (h1) | | Bold / 700 | __px | __px |
| Subtítulos (h2) | | SemiBold / 600 | __px | __px |
| Encabezados (h3) | | Medium / 500 | __px | __px |
| Cuerpo de texto | | Regular / 400 | __px | __px |
| Texto pequeño / caption | | Regular / 400 | __px | __px |
| Monospace (código) | | Regular / 400 | __px | __px |

**Google Fonts link:** https://fonts.googleapis.com/...

## 4. Iconografía

| Aspecto | Decisión |
|---|---|
| Librería de iconos (Heroicons / Lucide / Phosphor / otra) | |
| Estilo (lineal / sólido / duotono) | |
| Tamaño por defecto | |
| Color por defecto | |

## 5. Componentes de la Landing Page

### 5.1. Botones

| Tipo | Fondo | Texto | Borde | Radio borde | Padding |
|---|---|---|---|---|---|
| Primario (CTA) | | | — | | |
| Secundario (outline) | transparente | | | | |
| Enlace / text | — | | — | — | — |

### 5.2. Tarjetas

| Aspecto | Decisión |
|---|---|
| Fondo de tarjetas | |
| Sombra / elevación | |
| Radio de borde | |
| Padding interno | |

### 5.3. Formulario de Contacto

| Aspecto | Decisión |
|---|---|
| Fondo de inputs | |
| Borde de inputs | |
| Radio de borde de inputs | |
| Foco (focus ring) | |
| Placeholder text | |

## 6. Accesibilidad

| Aspecto | Valor |
|---|---|
| Ratio de contraste mínimo (texto normal) | WCAG AA 4.5:1 |
| Ratio de contraste mínimo (texto grande) | WCAG AA 3:1 |
| Tamaño mínimo de fuente | __px |
| Estados de foco (focus visible) | ¿Cómo se ve? |
| Textos alternativos en imágenes | ¿Plan? |

## 7. Implementación Técnica

| Aspecto | Decisión |
|---|---|
| Framework CSS | Tailwind CSS |
| Config colors en `tailwind.config.js` | Incluir hex definidos arriba |
| Modo oscuro | ¿Sí / No / Solo claro? |
| Animaciones | ¿AOS / Intersection Observer / ninguna? |
| Formulario de contacto | ¿Formspree / EmailJS / endpoint propio? |

---

## 8. Fecha de Entrega

| Aspecto | Fecha |
|---|---|
| Propuesta de logo (3 opciones) | |
| Paleta de colores definitiva | |
| Prototipo landing page en Figma | |
| Desarrollo frontend completado | |

---

*Completar y devolver a Fredinson y Steven para validación antes de iniciar el desarrollo.*
