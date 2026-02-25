---
name: analisis-inversion
description: |
  Análisis financiero de inversiones inmobiliarias con métricas profesionales.

  Triggers when user mentions:
  - "inversión"
  - "rentabilidad"
  - "cap rate"
  - "ROI"
  - "rendimiento"
  - "comprar para rentar"
  - "plusvalía"
---

# Análisis de Inversión Inmobiliaria

Evalúa oportunidades de inversión inmobiliaria con métricas financieras profesionales y contexto de mercado LATAM.

## Métricas clave

### 1. Cap Rate (Tasa de Capitalización)
```
Cap Rate = (Ingreso Operativo Neto Anual / Precio de Compra) × 100

Ingreso Operativo Neto = Ingreso Bruto - Vacancia - Gastos Operativos
```

**Rangos de referencia LATAM:**
| País | Residencial | Comercial | Oficinas |
|------|------------|-----------|----------|
| México | 4-7% | 6-9% | 7-10% |
| Colombia | 4-6% | 6-8% | 7-9% |
| Argentina | 2-4% (en USD) | 4-7% | 5-8% |
| Chile | 3-5% | 5-8% | 6-9% |

### 2. Cash-on-Cash Return (si compra con crédito)
```
Cash-on-Cash = Flujo de Caja Anual / Inversión Inicial de Bolsillo × 100

Inversión de Bolsillo = Enganche + Costos de cierre + Remodelación
```

### 3. Precio por m²
```
Precio/m² = Precio total / Superficie construida
```
Comparar con promedio de la zona para detectar oportunidades o sobreprecios.

### 4. GRM (Gross Rent Multiplier)
```
GRM = Precio de Compra / Renta Bruta Anual
```
Menor GRM = recuperas más rápido. Benchmark: 10-15 años es aceptable en LATAM.

### 5. Plusvalía estimada
Basada en:
- Desarrollo de infraestructura en la zona (metro, hospitales, centros comerciales)
- Tendencia de precios de los últimos 3-5 años
- Planes de desarrollo urbano del municipio

## Costos de cierre por país

### México
| Concepto | Costo estimado |
|----------|---------------|
| Escrituración (notario) | 4-7% del valor |
| ISR (si es venta) | Varía según ganancia |
| ISAI (Impuesto de Adquisición) | 2-5% según estado |
| Avalúo | $3,000-8,000 MXN |
| Certificado de libertad de gravamen | $500-2,000 MXN |

### Colombia
| Concepto | Costo estimado |
|----------|---------------|
| Escrituración (notaría) | 0.54% |
| Registro | 1.67% |
| Retención en la fuente (venta) | 1% del valor |
| Impuesto de registro | 1% |

### Argentina
| Concepto | Costo estimado |
|----------|---------------|
| Escrituración | 2-3% |
| Comisión inmobiliaria | 3-4% + IVA |
| Impuesto de sellos | 1.5-3.6% según provincia |
| ITI (Impuesto a la Transferencia) | 1.5% |

## Formato de análisis de inversión

```markdown
# Análisis de Inversión — [Dirección/Nombre]

## Datos de la propiedad
| Dato | Valor |
|------|-------|
| Tipo | [Casa/Depto/Comercial] |
| Ubicación | [Colonia, Ciudad] |
| Superficie | [m²] construidos / [m²] terreno |
| Precio de lista | $[monto] [moneda] |
| Precio/m² | $[monto] |
| Precio/m² promedio zona | $[monto] (fuente: [fuente]) |
| Diferencia vs zona | [+/-]% |

## Proyección de ingresos (anual)
| Concepto | Monto |
|----------|-------|
| Renta mensual estimada | $[monto] |
| Ingreso bruto anual | $[monto] |
| Vacancia estimada ([%]) | -$[monto] |
| **Ingreso efectivo** | **$[monto]** |

## Gastos operativos (anual)
| Concepto | Monto |
|----------|-------|
| Mantenimiento | $[monto] |
| Predial/impuestos | $[monto] |
| Seguros | $[monto] |
| Administración ([%]) | $[monto] |
| Reserva para reparaciones | $[monto] |
| **Total gastos** | **$[monto]** |

## Métricas de inversión
| Métrica | Valor | Benchmark |
|---------|-------|-----------|
| Ingreso Operativo Neto | $[monto] | — |
| Cap Rate | [%] | [rango del país] |
| GRM | [años] | 10-15 años |
| Cash-on-Cash (si crédito) | [%] | >8% bueno |
| Punto de equilibrio | [meses] | — |

## Costos de adquisición
| Concepto | Monto |
|----------|-------|
| Precio | $[monto] |
| Escrituración | $[monto] |
| Impuestos de adquisición | $[monto] |
| Avalúo | $[monto] |
| Remodelación estimada | $[monto] |
| **Inversión total** | **$[monto]** |

## Escenarios a 5 años
| Escenario | Plusvalía anual | Valor en 5 años | ROI total |
|-----------|----------------|-----------------|-----------|
| Pesimista | [%] | $[monto] | [%] |
| Base | [%] | $[monto] | [%] |
| Optimista | [%] | $[monto] | [%] |

## Recomendación
**[Comprar / No comprar / Negociar precio]**
[Justificación en 3-5 oraciones]

## Supuestos
- [Supuesto 1]
- [Supuesto 2]

⚠️ Este análisis es orientativo. Los datos de mercado deben verificarse con fuentes locales actualizadas.
```

## Reglas
- Siempre muestra los supuestos de cada cálculo.
- Usa moneda local del país.
- Incluye costos de cierre en el análisis (muchos inversionistas novatos los olvidan).
- Advierte que son estimaciones y que el mercado puede variar.
- Si el usuario compra con crédito, incluye el análisis de cash-on-cash además del cap rate.
- Compara siempre el precio/m² con el promedio de la zona.
