# AikaOS Templates — Banco de Pruebas

5 templates premium listos para probar con tu instalación de OpenWork/AikaOS.

## Instalación manual

Cada template tiene su carpeta con la estructura exacta de `.opencode/`. Para instalar uno:

```bash
# Desde la raíz de tu proyecto donde corre OpenWork
cp -r templates1/investigador-web/skills/* .opencode/skills/
cp -r templates1/investigador-web/commands/* .opencode/commands/
```

O copia todo de golpe:
```bash
for t in investigador-web creador-contenido asistente-obsidian ventas-b2b asistente-inmobiliario; do
  cp -r "templates1/$t/skills/"* .opencode/skills/ 2>/dev/null
  cp -r "templates1/$t/commands/"* .opencode/commands/ 2>/dev/null
done
```

Después reinicia OpenWork para que detecte los nuevos skills y commands.

## Templates incluidos

| Template | Skills | Commands | MCPs sugeridos |
|----------|--------|----------|----------------|
| **investigador-web** | 3 | 5 | Firecrawl, Brave Search, Filesystem |
| **creador-contenido** | 3 | 5 | Twitter/X, Brave Search, Filesystem |
| **asistente-obsidian** | 3 | 5 | Obsidian MCP, Filesystem |
| **ventas-b2b** | 3 | 5 | Gmail, Calendar, Brave Search |
| **asistente-inmobiliario** | 3 | 5 | Brave Search, Filesystem |

## Estructura de cada template

```
template-name/
├── skills/
│   └── skill-name/
│       └── SKILL.md          ← instrucciones persistentes del agente
├── commands/
│   └── command-name.md       ← prompts predefinidos con frontmatter
└── README.md                 ← qué hace, cómo probar, MCPs necesarios
```

## MCPs recomendados

Para sacar el máximo provecho, conecta estos MCPs en OpenWork:

- **Firecrawl** (`firecrawl-mcp`): scraping web, el más rápido
- **Brave Search** (`@anthropic/brave-search-mcp`): búsquedas web
- **Filesystem** (`@anthropic/filesystem-mcp`): ya incluido en OpenCode
- **Obsidian** (`obsidian-mcp-server`): acceso al vault
- **Gmail** (`@anthropic/google-gmail-mcp`): envío de emails
- **Google Calendar** (`@anthropic/google-calendar-mcp`): gestión de citas
- **Twitter/X** (`@enescinar/twitter-mcp`): publicación en X
