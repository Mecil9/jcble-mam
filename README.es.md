# Jcble_mam

[English](README.md) | [简体中文](README.zh-CN.md) | Español | [日本語](README.ja.md) | [한국어](README.ko.md)

`jcble-mam` es una skill para Codex orientada a operaciones de contenido empresarial, flujos de redacción, promoción de marketing en línea y coordinación de sesiones multi-Agent.

Ayuda a Codex a trabajar como un equipo coordinado de contenido y marketing para gestión documental, redacción de propuestas, textos de producto, temas para redes sociales, briefs visuales, investigación de mercado, búsqueda de clientes, borradores de correos y retrospectivas semanales o mensuales.

## Qué hace

- Crea un equipo reutilizable de Agents para contenido y marketing empresarial.
- Define roles para coordinación editorial, gestión documental, planificación de propuestas, redacción, textos de producto, planificación de PPT, briefs visuales, inteligencia de mercado, búsqueda de clientes, borradores de correo, revisión y retrospectivas.
- Soporta sesiones persistentes de Codex por rol y un flujo de bus de mensajes.
- Soporta salida Markdown en chino simplificado, inglés, español, japonés y coreano.
- Mantiene el contenido externo vinculado a evidencia aprobada y revisión humana.

## Instalación para Codex

Clona este repositorio en tu directorio de skills de Codex:

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

Después inicia una nueva sesión de Codex para refrescar el registro de skills.

Si tu configuración de Codex usa otro directorio de skills, clona el repositorio allí y conserva este nombre de carpeta:

```text
jcble-mam
```

## Uso básico

Después de instalarlo, pide a Codex lo que necesitas en lenguaje natural. Ejemplos:

```text
Usa jcble-mam para crear un equipo de contenido y marketing para mi empresa.
```

```text
Usa jcble-mam para convertir este documento de producto en texto para web y un borrador de email de prospección.
```

```text
Usa jcble-mam para crear sesiones independientes de Codex para editor, redactor, investigación de mercado, brief visual y revisión.
```

```text
Usa jcble-mam para escribir este resumen de propuesta en inglés, español, japonés y coreano.
```

## Configuración del espacio de trabajo

Antes de usar la skill con archivos de empresa, asigna estos marcadores de posición a tu propio espacio de trabajo:

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

Si tu empresa usa otros nombres de carpetas, actualiza los archivos de referencia o crea archivos de índice equivalentes.

## Archivos incluidos

- `SKILL.md` - condiciones de activación y flujo principal
- `references/agent-team-roles.md` - biblioteca de roles multi-Agent
- `references/session-orchestration.md` - creación, nombres, sincronización y enrutamiento de mensajes en sesiones Codex
- `references/company-material-boundaries.md` - límites de materiales de empresa y reglas de datos sensibles
- `references/multilingual-workflow.md` - reglas de Markdown multilingüe, límites de localización y lista de revisión
- `assets/task-card-template.md` - plantilla de ficha de tarea
- `assets/message-template.md` - plantilla de bus de mensajes
- `assets/retrospective-template.md` - plantilla de retrospectiva semanal/mensual

## Notas de seguridad

Antes de publicar o enviar contenido externamente:

- elimina datos confidenciales de clientes, contratos, finanzas, nómina, credenciales y datos personales
- verifica todas las afirmaciones públicas con archivos fuente aprobados
- mantén los correos de prospección como borradores hasta la aprobación humana
- no presentes imágenes generadas como productos reales, sitios reales o escenas reales de clientes

## Licencia

MIT
