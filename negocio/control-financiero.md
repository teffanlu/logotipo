# IDUNA — Control Financiero y Costeo

> Estructura para controlar capital, pagos, costeo de aterrizaje y datos de proveedores.
> Objetivo: saber el costo real por unidad y NO perder dinero al vender. Llenar con cifras reales.
> Herramienta sugerida: **Google Sheets** (una hoja por tabla) o Notion. Última actualización: junio 2026.

## 0. Regla de oro
- **Caja personal ≠ caja del negocio.** Nunca mezclar. Todo gasto/ingreso del negocio se registra aquí.
- **Costear SIEMPRE sobre el producto puesto en Maracaibo** (costo de aterrizaje), nunca sobre el precio Alibaba.
- Margen objetivo del **aparato (héroe) >55%**. Skincare = gancho (margen 20-35%).

---

## 1. Resumen de capital (actualizar siempre)

| Concepto | Monto |
|---|---|
| Capital disponible para el negocio | ~$2,625 |
| Comprometido (pedidos confirmados) | $0 |
| Gastado (pagado) | $0 |
| **Caja restante** | ~$2,625 |

### Reparto objetivo del lote 1
| Frente | Tope sugerido |
|---|---|
| Mercancía China (gua sha + aparato + accesorios) | ~$500-600 |
| Flete marítimo + aduana + casillero | *(según agencia)* |
| Skincare + gel (ruta USA) | ~$300-500 |
| Empaque/stickers local | ~$100-150 |
| **Colchón de caja / marketing / imprevistos** | **el resto (no tocar)** |

---

## 2. Fórmula de costo de aterrizaje (landed cost)

```
COSTO ATERRIZADO POR UNIDAD =
  precio unitario (FOB)
  + flete interno China por unidad
  + flete marítimo ASIGNADO por unidad
  + aduana por unidad
  + casillero/agencia por unidad
  + empaque por unidad
```

**Prorrateo del flete marítimo por CBM** (el flete se reparte según el volumen que ocupa cada producto):
```
Flete asignado a un producto = Flete marítimo total × (CBM del producto ÷ CBM total del envío)
Flete por unidad = Flete asignado al producto ÷ unidades de ese producto
```

**Precio de venta a partir del margen objetivo:**
```
Precio de venta = Costo aterrizado ÷ (1 − margen)     ej: $23.5 ÷ (1 − 0.60) = $58.75
Margen %        = (Precio de venta − Costo aterrizado) ÷ Precio de venta
```

**Ejemplo aparato galvánico (Xiazhifeng):** $15.50 FOB + ~$8 (flete+aduana+casillero+empaque) ≈ **$23.50 aterrizado** → vender $69-89 = margen **66-73%**. ✅

---

## 3. Tabla de PROVEEDORES

| Proveedor | Producto | Link/tienda | Años | Verified/TA | MOQ | Precio U | Lead time a casillero | Contacto | Rating | Notas |
|---|---|---|---|---|---|---|---|---|---|---|
| Shenzhen Easter Technology | Gua sha acero 304 | (Alibaba) | 13 | Sí / Sí | — | $2.5 (corazón, 30-50u) | ~15 días | — | 4.9 (600) | White bag gratis; cloth bag opc. $0.40 |
| Shenzhen Xiazhifeng (PAKISS) | Aparato galvánico | esongsun.m.en.alibaba.com | 9 | Sí / Sí | 10 | $15.50 | *(preguntar)* | — | 4.6 (774) | Mismo que Nove, más barato; OEM MOQ 1 |
| Shenzhen Nove | Aparato galvánico (NV-IH01) | (Alibaba) | 9 | Sí / Sí | 1 | ~$22 | 3-5 días | — | 4.9 (2736) | Galvánico (no EMS); paga-retiene 10% |
| *(empaque/accesorios)* | Faux suede pouch + pañuelo | — | — | — | 100 | $0.37 / $0.28 | *(preguntar)* | — | — | Preguntar si hacen cintillo + espátula |
| | | | | | | | | | | |

---

## 4. REGISTRO DE COMPRAS (costeo por producto)

| Fecha | Producto | Proveedor | Cant | Precio U (FOB) | Subtotal | CBM ítem | % envío (CBM) | Flete asignado | Aduana | Casillero | Empaque | **Costo aterrizado/U** | Precio venta | **Margen %** |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| | Gua sha | Easter | 50 | 2.50 | | | | | | | | | | |
| | Aparato galvánico | Xiazhifeng | 12-15 | 15.50 | | | | | | | | | | |
| | Cintillo | (empaque) | 100 | ~0.50 | | | | | | | | | | |
| | Espátula silicona | (empaque) | 100 | ~0.20 | | | | | | | | | | |
| | Faux suede pouch | (empaque) | 100 | 0.37 | | | | | | | | | | |
| | Pañuelo microfibra | (empaque) | 100 | 0.28 | | | | | | | | | | |
| | **TOTAL** | | | | | | 100% | | | | | | | |

> Skincare (ruta USA) se registra aparte con su propio flete Miami→Maracaibo (ver `sourcing-skincare-usa.md`).

---

## 5. CONTROL DE PAGOS

| Fecha | Concepto | Proveedor/Destino | Monto | Método | Estado | Notas |
|---|---|---|---|---|---|---|
| | Depósito pedido aparato | Xiazhifeng | | Trade Assurance | Pendiente | |
| | Pedido gua sha | Easter | | Trade Assurance | Pendiente | |
| | Flete marítimo | Agencia/casillero | | | Pendiente | |
| | Skincare | YesStyle/Ulta | | PayPal | Pendiente | |
| | | | | | | |

---

## 6. Punto de equilibrio (break-even)
```
Inversión total del lote 1 = suma de "Subtotal" + flete + aduana + casillero + empaque + skincare
Ganancia por kit = Precio del kit − Costo aterrizado del kit
Kits para recuperar = Inversión total ÷ Ganancia por kit
```
> Meta del lanzamiento ("Operación Retorno"): vender los kits suficientes para recuperar la inversión + 20-50 clientes con testimonio.

---

## 7. Métricas a vigilar (mensual)
- **Margen %** por producto y por kit (aparato >55%).
- **Rotación:** unidades vendidas / unidades compradas (¿reordenar?).
- **AOV** (ticket promedio): subirlo con accesorios y kits.
- **ROI del lote:** ganancia neta ÷ inversión del lote.
- **Caja restante** y colchón intacto.
