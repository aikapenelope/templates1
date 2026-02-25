# AikaOS Templates Premium

5 expertos listos para usar con AikaOS. Sin terminal, sin configuración.

## Cómo instalar un template (3 pasos)

### Paso 1: Descarga la carpeta del experto

Descarga la carpeta del experto que quieras usar (ej: `investigador-web/`).

> Desde GitHub: Code > Download ZIP, descomprime, y quédate con la carpeta del experto que quieras.

### Paso 2: Crea un Worker

En AikaOS, haz clic en **Create Worker**.

### Paso 3: Selecciona la carpeta

Haz clic en **Select Folder** y apunta a la carpeta del experto que descargaste.

**Listo.** El worker ya tiene los skills y commands configurados. Empieza a chatear.

---

## Expertos disponibles

| Experto | Qué hace | Skills | Commands |
|---------|----------|--------|----------|
| **investigador-web** | Investiga temas, verifica datos, compara opciones | 3 | 5 |
| **creador-contenido** | Crea posts, calendarios editoriales, copywriting | 3 | 5 |
| **asistente-obsidian** | Gestiona tu vault, weekly reviews, Zettelkasten | 3 | 5 |
| **ventas-b2b** | Prospección, propuestas, manejo de objeciones | 3 | 5 |
| **asistente-inmobiliario** | Fichas, análisis de inversión, contratos, marketing | 3 | 5 |

Cada carpeta de experto tiene un `README.md` con ejemplos de qué preguntarle.

## Estructura de cada carpeta

```
investigador-web/          ← esta carpeta es la que seleccionas
├── .opencode/
│   ├── skills/            ← instrucciones del experto (se activan solas)
│   │   ├── investigacion-web/SKILL.md
│   │   ├── sintesis-reportes/SKILL.md
│   │   └── verificacion-fuentes/SKILL.md
│   └── commands/          ← prompts listos para usar
│       ├── investigar-tema.md
│       ├── comparar-opciones.md
│       ├── resumen-articulo.md
│       ├── verificar-dato.md
│       └── monitorear-tema.md
└── README.md
```

No necesitas tocar nada dentro de `.opencode/`. Solo apunta a la carpeta y AikaOS lee todo automáticamente.

## MCPs recomendados

Para sacar el máximo provecho, conecta estos MCPs en la configuración de tu worker:

| MCP | Para qué sirve | Lo usan |
|-----|----------------|---------|
| Firecrawl (`firecrawl-mcp`) | Scraping web | investigador-web |
| Brave Search (`@anthropic/brave-search-mcp`) | Búsquedas web | investigador-web, ventas-b2b, inmobiliario |
| Obsidian (`obsidian-mcp-server`) | Acceso al vault | asistente-obsidian |
| Gmail (`@anthropic/google-gmail-mcp`) | Envío de emails | ventas-b2b |
| Google Calendar (`@anthropic/google-calendar-mcp`) | Gestión de citas | ventas-b2b |
| Twitter/X (`@enescinar/twitter-mcp`) | Publicar en X | creador-contenido |
| Filesystem (`@anthropic/filesystem-mcp`) | Leer/escribir archivos | todos (ya incluido) |

Los MCPs son opcionales. Los expertos funcionan sin ellos, pero con MCPs pueden ejecutar acciones (buscar, enviar emails, publicar).
