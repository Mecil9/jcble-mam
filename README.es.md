# Jcble_mam

[简体中文](README.zh-CN.md) | [English](README.en.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

`jcble-mam` es una skill general de Codex para crear y operar flujos de contenido empresarial, redacción, promoción de marketing en línea y equipos colaborativos multi-Agent.

Idiomas Markdown compatibles:

- Chino simplificado `zh-CN`
- Inglés `en`
- Español `es`
- Japonés `ja`
- Coreano `ko`

## Casos de uso

- Gestión de documentos de empresa
- Planificación de soluciones y redacción de propuestas
- Planificación de temas para redes sociales
- Planificación de PPT corporativos y de soluciones
- Redacción de textos de producto
- Briefs visuales para productos, soluciones y material promocional
- Inteligencia de mercado global
- Seguimiento de noticias del sector
- Búsqueda de clientes internacionales
- Borradores de correos de prospección
- Retrospectivas semanales y mensuales de contenido, plataformas y leads
- Configuración de sesiones persistentes multi-Agent en Codex
- Creación, traducción y localización de Markdown multilingüe

## Nombre de la skill

El nombre instalable de la skill es:

```text
jcble-mam
```

`Jcble_mam` se mantiene como nombre visible y alias para usuarios. El flujo de trabajo es genérico y puede adaptarse a cualquier empresa.

## Instalación

Clona este repositorio en un directorio de skills de Codex:

```bash
git clone https://github.com/Mecil9/jcble-mam.git ~/.agents/skills/jcble-mam
```

Después inicia una nueva sesión de Codex para refrescar el registro de skills.

## Configuración

Antes de usar la skill, adapta estos marcadores de posición a tu propio espacio de trabajo:

```text
COMPANY_WORKSPACE=/path/to/company/workspace
COMPANY_KNOWLEDGE_BASE=/path/to/company/knowledge-base
COMPANY_MARKETING_WORKSPACE=/path/to/company/content-marketing-workspace
```

Si tu empresa usa otros nombres de carpetas, actualiza los archivos de referencia o crea archivos de índice equivalentes.

## Archivos principales

- `SKILL.md` - condiciones de activación y flujo principal
- `references/agent-team-roles.md` - biblioteca de roles multi-Agent
- `references/session-orchestration.md` - creación, nombres, sincronización y enrutamiento de mensajes en sesiones Codex
- `references/company-material-boundaries.md` - límites de materiales de empresa y reglas de datos sensibles
- `references/multilingual-workflow.md` - reglas de Markdown multilingüe, límites de localización y lista de revisión
- `assets/task-card-template.md` - plantilla de ficha de tarea
- `assets/message-template.md` - plantilla de bus de mensajes
- `assets/retrospective-template.md` - plantilla de retrospectiva semanal/mensual

## Notas de seguridad

Antes de publicar externamente:

- elimina datos confidenciales de clientes, contratos, finanzas, nómina, credenciales y datos personales
- verifica todas las afirmaciones públicas con archivos fuente aprobados
- mantén los correos de prospección como borradores hasta la aprobación humana
- no presentes imágenes generadas como productos reales, sitios reales o escenas reales de clientes

## Licencia

MIT
