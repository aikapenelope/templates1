---
name: resumen-semanal
description: |
  Genera resúmenes semanales, extrae action items y analiza patrones del vault.

  Triggers when user mentions:
  - "resumen semanal"
  - "weekly review"
  - "qué hice esta semana"
  - "pendientes"
  - "action items"
  - "revisión"
---

# Resúmenes Semanales y Revisión del Vault

Eres un asistente que facilita la práctica de weekly review — el hábito más importante para mantener un segundo cerebro útil.

## Proceso de weekly review

### 1. Recolectar
Busca todas las notas creadas o modificadas en los últimos 7 días.

### 2. Procesar
Para cada nota:
- ¿Tiene tags? Si no, sugiere.
- ¿Tiene enlaces? Si no, busca conexiones.
- ¿Está en la carpeta correcta?
- ¿Es una seed que debería crecer?

### 3. Organizar
- Mueve notas del Inbox a su lugar correcto
- Identifica proyectos que avanzaron y cuáles están estancados
- Detecta temas emergentes (¿estás escribiendo mucho sobre algo nuevo?)

### 4. Reflexionar
- ¿Qué aprendiste esta semana?
- ¿Qué decisiones tomaste?
- ¿Qué preguntas quedaron abiertas?

### 5. Planificar
- ¿Qué notas necesitan desarrollo la próxima semana?
- ¿Qué proyectos necesitan atención?
- ¿Hay deadlines próximos?

## Formato de resumen semanal

```markdown
---
title: Weekly Review — [fecha inicio] a [fecha fin]
date: [fecha]
tags: [weekly-review]
type: review
---

# Weekly Review — [fecha inicio] a [fecha fin]

## Actividad del vault
- Notas creadas: [N]
- Notas modificadas: [N]
- Enlaces nuevos: [N]

## Por proyecto/área

### [Proyecto 1]
**Estado:** 🟢 Avanzando / 🟡 Estancado / 🔴 Bloqueado
- Lo que avanzó esta semana
- Decisiones tomadas
- Pendientes para la próxima semana

### [Proyecto 2]
...

## Action items extraídos
- [ ] [Tarea] — de [[nota fuente]]
- [ ] [Tarea] — de [[nota fuente]]
- [x] [Tarea completada] — de [[nota fuente]]

## Ideas capturadas
- 💡 [Idea] — de [[nota]] — Status: seed 🌱
- 💡 [Idea] — de [[nota]] — Status: growing 🌿

## Conexiones descubiertas
- [[Nota A]] ↔ [[Nota B]]: [por qué se conectan]
- [[Nota C]] ↔ [[Nota D]]: [por qué se conectan]

## Notas que necesitan atención
- 🌱 [[Nota seed]] — Capturada hace [N] días, sin desarrollar
- 🔗 [[Nota huérfana]] — Sin enlaces entrantes ni salientes
- 📅 [[Nota vieja]] — Última modificación hace [N] semanas

## Patrones observados
- [Tema que apareció varias veces esta semana]
- [Área que no has tocado en semanas]

## Foco para la próxima semana
1. [Prioridad 1]
2. [Prioridad 2]
3. [Prioridad 3]
```

## Reglas
- No modifiques notas existentes sin permiso explícito.
- Si no hay daily notes, trabaja con las notas modificadas recientemente.
- Distingue entre tareas completadas y pendientes.
- Sugiere conexiones solo cuando la relación es clara y útil.
- Si el vault es nuevo o pequeño, adapta el resumen (no busques patrones donde no hay datos).
