# IDUNA — Kit de variantes del isotipo

Variantes maestras generadas a partir de `../image_f7afa246.svg`.

## Paleta oficial
| Rol | Color | HEX |
|---|---|---|
| Base / fondo | Crema Arena | `#F5F1E9` |
| Texto / contraste | Charcoal Lab | `#2D2D2D` |
| Impacto / marca | Terracota Profundo | `#A45A41` |
| Acento | Nude Suave | `#E8C5B0` |
| Premium (digital) | Oro Mate | `#B08D57` |

## Archivos

### `variantes/`
- **isotipo-charcoal.svg** — Isotipo aislado (símbolo solo), fondo transparente. Archivo maestro.
- **isotipo-charcoal-crema.svg** — Versión principal: charcoal sobre crema.
- **isotipo-blanco-terracota.svg** — Blanco sobre terracota (empaque a color).
- **isotipo-oro-charcoal.svg** — Oro mate sobre charcoal (Línea Premium / referencia digital del foil).
- **isotipo-compacto-charcoal.svg** — Versión compacta con trazo engrosado para tamaños pequeños (≤32px).
- **isotipo-compacto-crema.svg** — Versión compacta sobre crema.
- **favicon-32.svg** — Favicon listo (compacto, 32px, fondo crema).

### Hoja de prueba
- **favicon-test.svg** — Compara el isotipo ORIGINAL vs COMPACTO a 16/24/32/48/64/128px.

## Diagnóstico de legibilidad (datos del trazo)
- Parte más delgada del trazo: **3.4%** del ancho del símbolo.
- A **16px** el trazo fino mide ~0.5px → se desvanece. No usar el original en favicon.
- A **48px en adelante** el original funciona perfecto.
- Para usos ≤32px usar la **versión compacta** (trazo engrosado ~+150 unidades).

## Pendiente / siguientes pasos
- Versiones con wordmark (horizontal y vertical) en tinta única.
- Validar contraste del terracota para texto pequeño (accesibilidad).
- Probar foil real en muestra física de empaque.
