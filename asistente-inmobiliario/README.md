# Asistente Inmobiliario (Premium)

Gestión completa de propiedades: fichas, análisis de inversión, contratos, comparativas y marketing inmobiliario para LATAM.

## Skills (3)
- **gestion-inmobiliaria** — Fichas profesionales, terminología por país, contratos de arrendamiento con cláusulas por legislación, cartas de intención
- **analisis-inversion** — Cap Rate, Cash-on-Cash, GRM, precio/m², costos de cierre por país (MX/CO/AR/CL), escenarios a 5 años, benchmarks LATAM
- **marketing-inmobiliario** — Portales por país, descripciones que venden, contenido para Instagram/Facebook/WhatsApp, guía de fotografía inmobiliaria

## Commands (5)
- `crear-ficha` — Ficha profesional con descripción que vende + versión corta para WhatsApp
- `analizar-inversion` — Análisis financiero completo con 7 métricas y escenarios
- `contrato-arrendamiento` — Borrador adaptado a la legislación del país
- `comparar-propiedades` — Tabla comparativa con ranking ponderado y recomendación
- `publicar-propiedad` — Textos optimizados para 5 canales (portal, Instagram, Facebook, WhatsApp, Reel)

## MCPs recomendados
- **Brave Search** (`@anthropic/brave-search-mcp`) — Buscar precios de referencia y comparables
- **Filesystem** (`@anthropic/filesystem-mcp`) — Guardar fichas, contratos y análisis

## Cómo probar
1. Copia skills y commands a tu `.opencode/`
2. Prueba: "Crea una ficha para un departamento de 2 recámaras en la Condesa, CDMX, renta $18,000/mes"
3. Prueba: "Analiza si vale la pena comprar un depto de $2.5M MXN que se renta en $15,000/mes"
4. Prueba: "Compara estas 3 propiedades: [datos]"
5. Prueba: "Genera los textos para publicar esta propiedad en Inmuebles24, Instagram y WhatsApp"
