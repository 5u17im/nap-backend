# Estructura Matemática de Pricing y Rentabilidad (Spread)

Como startup, el "Gross Volume" (dinero transado) es engañoso. Lo único que garantiza la supervivencia es el **Net Spread** (Margen de ganancia neta después de pagar a pasarelas).

## 1. Estructura de Costos de Pasarela (Estimación ePayco/Nequi)
Para recibir y dispersar dinero en Colombia, las pasarelas cobran un *Fee* (Tarifa).
- **Costo base estimado de pasarela:** `2.99% + $900 COP` por transacción (más IVA de la comisión).
- **Costo de Retiro (Dispersión):** Algunos proveedores cobran tarifas planas (ej. $1.000 COP) por enviar el dinero de la cuenta Escrow a la cuenta bancaria del trabajador.

## 2. Simulación Transaccional Matemática (Comisión Dinámica del 10%)

### Caso A: Contrato de cuantía baja ($50.000 COP)
- **Monto Total del Contrato:** $50.000 COP
- **Comisión Cobrada por NAP (10%):** $5.000 COP
- **Costo Pasarela (Entrada):** ($50.000 * 2.99%) + $900 = $2.395 COP + IVA = ~$2.850 COP
- **Costo Dispersión (Salida):** ~$1.000 COP
- **Ganancia Neta (Spread):** $5.000 - $3.850 = **$1.150 COP** (Margen del 2.3% real).

### Caso B: Contrato de cuantía media ($500.000 COP)
- **Monto Total del Contrato:** $500.000 COP
- **Comisión Cobrada por NAP (10%):** $50.000 COP
- **Costo Pasarela (Entrada):** ($500.000 * 2.99%) + $900 = $15.850 COP + IVA = ~$18.861 COP
- **Costo Dispersión (Salida):** ~$1.000 COP
- **Ganancia Neta (Spread):** $50.000 - $19.861 = **$30.139 COP** (Margen del 6.02% real).

## 3. Directriz Gerencial de Pricing
1. **Monto Mínimo Transaccional:** Por seguridad matemática, **no se pueden permitir contratos en NAP por montos inferiores a $30.000 COP**. Por debajo de este valor, la comisión de la pasarela absorbe más del 10% cobrado y NAP operaría a pérdida.
2. **Dinamicidad en Grandes Ligas:** Para contratos superiores a $3.000.000 COP, el 10% de comisión ($300.000) puede ahuyentar a clientes B2B. El algoritmo de Pricing debe reducir la comisión automáticamente al 5% o 7% para altos volúmenes, manteniendo un excelente *Spread* neto.
