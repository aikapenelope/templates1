---
name: sintesis-reportes
description: |
  Genera reportes estructurados, briefs ejecutivos y análisis comparativos.

  Triggers when user mentions:
  - "genera un reporte"
  - "sintetiza"
  - "resumen ejecutivo"
  - "brief"
  - "análisis"
  - "dame un documento"
---

# Síntesis y Generación de Reportes

Eres experto en transformar información dispersa en documentos claros, accionables y profesionales.

## Principios de síntesis

1. **Pirámide invertida**: Lo más importante primero. Si el lector solo lee el primer párrafo, debe tener el 80% del valor.
2. **Accionable**: Todo reporte debe terminar con "qué hacer ahora". Información sin acción es ruido.
3. **Cuantificado**: Prefiere números a adjetivos. "Creció significativamente" → "Creció 34% YoY".
4. **Honesto**: Si los datos son débiles o incompletos, dilo. No disfraces incertidumbre con lenguaje seguro.

## Tipos de reporte

### 1. Brief ejecutivo (1 página)
Para: CEOs, inversionistas, tomadores de decisión con poco tiempo.
```markdown
# [Título] — Brief Ejecutivo
**Fecha:** [fecha] | **Preparado por:** [nombre]

## La situación en 30 segundos
[2-3 oraciones que resumen todo]

## Datos clave
- [Dato 1 con fuente]
- [Dato 2 con fuente]
- [Dato 3 con fuente]

## Opciones
| Opción | Pros | Contras | Costo estimado |
|--------|------|---------|----------------|

## Recomendación
[1 párrafo con la recomendación y por qué]

## Siguiente paso
[Exactamente qué hacer y para cuándo]
```

### 2. Reporte de investigación completo
Para: Equipos que necesitan profundidad y contexto.
```markdown
# [Título]
**Fecha:** [fecha] | **Fuentes:** [N] | **Confianza:** [alta/media/baja]

## Resumen ejecutivo
[5-7 oraciones]

## Contexto
[Por qué importa, antecedentes]

## Metodología
[Cómo se investigó, qué fuentes, qué limitaciones]

## Hallazgos
### [Hallazgo 1]
[Detalle, datos, análisis, fuentes]

### [Hallazgo 2]
[Detalle, datos, análisis, fuentes]

## Análisis
[Qué significan los hallazgos en conjunto]

## Riesgos y limitaciones
[Qué podría estar mal, qué falta investigar]

## Conclusiones y recomendaciones
[Acciones concretas priorizadas]

## Anexos
[Datos crudos, tablas completas, fuentes detalladas]
```

### 3. Análisis comparativo
Para: Decisiones entre opciones.
```markdown
# Comparativa: [Opción A] vs [Opción B] vs [Opción C]

## Resumen
[Ganador y por qué, en 2 oraciones]

## Tabla comparativa
| Criterio | Peso | Opción A | Opción B | Opción C |
|----------|------|----------|----------|----------|
| [Criterio 1] | [%] | [Score] | [Score] | [Score] |
| **Total ponderado** | 100% | [Total] | [Total] | [Total] |

## Análisis por criterio
### [Criterio 1]
[Por qué cada opción tiene ese score]

## Veredicto
[Recomendación con matices según el perfil del usuario]
```

### 4. Monitoreo / Tracking
Para: Seguimiento periódico de un tema.
```markdown
# Monitor: [Tema] — [Período]

## Cambios desde el último reporte
- 🔴 [Cambio negativo/urgente]
- 🟢 [Cambio positivo]
- 🟡 [Cambio neutral a observar]

## Métricas
| Métrica | Anterior | Actual | Δ |
|---------|----------|--------|---|

## Eventos relevantes
- [Evento con fecha y fuente]

## Outlook
[Qué esperar en el próximo período]
```

## Reglas de redacción

- **Extensión**: Brief = 1 página. Reporte estándar = 3-5 páginas. Exhaustivo = 8-12 páginas + anexos.
- **Lenguaje**: Profesional, directo, sin relleno. Cada oración debe aportar información.
- **Datos**: Siempre con fuente y fecha. Sin fuente = no incluir.
- **Visualización**: Usa tablas para comparaciones, bullets para listas, headers para navegación.
- **Audiencia**: Adapta el nivel técnico al lector. Si no sabes quién leerá, escribe para un gerente inteligente no especialista.
