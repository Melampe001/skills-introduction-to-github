# Instrucciones para GitHub Copilot (README_COPILOT)

Este archivo describe cómo interactuar con GitHub Copilot / asistentes automatizados en este repositorio, qué expectativas hay sobre propuestas y cambios, y las convenciones mínimas que deben seguirse antes de crear commits o *pull requests*.

## Objetivo
Proveer un conjunto claro de instrucciones y ejemplos para que Copilot (y colaboradores que usen asistentes) propongan cambios coherentes con las normas del proyecto, agilicen tareas repetitivas y generen PRs útiles y revisables.

## Contenido
- Propósito y alcance
- Estándares obligatorios antes de commits
- Formato y estructura de propuestas (archivos, PRs)
- Ejemplos de prompts útiles para Copilot
- Checklist mínimo para PRs generados por asistentes
- Contacto y responsabilidad humana

---

## Reglas obligatorias (resumen)
1. Ejecutar `make fmt` antes de crear cualquier commit. Esto aplica a todos los cambios en Go y asegura formato consistente.
2. Para cambios en `proto/` ejecutar `make proto` y añadir los archivos generados.
3. Construir y testear localmente: `make build` y `make test`.
4. CI completo: `make ci` (incluye build, fmt, lint y tests) antes de mergear.
5. Mantener la organización de carpetas: cmd/, internal/, lib/, admin/, config/, docs/, proto/, ruby/, testing/.

---

## Guía para proponer archivos o cambios (para Copilot / asistentes)
Cuando propongas un archivo (por ejemplo `README_COPILOT.md`) o cambios:
- Presenta el contenido completo del/los archivos propuestos usando el bloque de archivo con nombre.
- Incluye una descripción corta (1–3 líneas) del porqué del cambio.
- Indica los comandos que deben ejecutarse localmente para verificar (build, fmt, test).
- Si introduces código Go, crea o actualiza pruebas unitarias correspondientes (usar tests table-driven cuando sea posible).
- Si el cambio afecta `ruby/`, incrementa la versión en `ruby/lib/billing-platform/version.rb` siguiendo semver.

Ejemplo de metadatos que acompañen la propuesta:
- Rama propuesta: `copilot/README-copilot`
- Commit message sugerido: `docs: add README_COPILOT with copilot instructions`
- Comandos de verificación: `make fmt && make build && make test`

---

## Checklist mínimo para PRs generados por asistentes
Antes de abrir o pedir merge de un PR automatizado, verifica:
- [ ] `make fmt` pasó y no hay cambios pendientes de formateo.
- [ ] `make test` pasa localmente.
- [ ] `make build` pasa.
- [ ] Nuevas funciones tienen tests unitarios con cobertura razonable.
- [ ] Documentación (docs/ o README) actualizada si aplica.
- [ ] Si se modifican APIs públicas, se documentó el cambio y, si aplica, se agregó una nota de migración.
- [ ] PR description clara: propósito, cambios principales, cómo probar manualmente, riesgos conocidos.

---

## Buenas prácticas para prompts (ejemplos)
- Bueno: "Genera un nuevo archivo markdown README_COPILOT.md que explique cómo usar Copilot para proponer cambios en este repo. Incluir checklist de CI y comandos: make fmt, make build, make test."
- Mejor: "Crea README_COPILOT.md en español. Incluye: reglas obligatorias antes de commit (make fmt), pasos para proponer archivos (bloque de archivo con nombre), checklist de PRs y ejemplo de commit message y branch."
- Evita: prompts vagos como "arregla este repo" sin contexto ni instrucciones de verificación.

---

## Formato y plantilla sugerida para PR description
Título: tipo: breve descripción (ej. docs: add README_COPILOT)

Descripción:
- Resumen corto (1–2 líneas)
- Cambios principales (lista)
- Cómo probar
- Comandos a correr localmente
- Checklist (usar la lista de arriba)

---

## Responsabilidad humana
Los asistentes pueden proponer cambios, pero la revisión final y el merge deben ser realizados por un mantenedor humano. No mergear PRs automatizados sin revisión.

---

## Contacto y mantenimiento
Si la propuesta afecta flujos críticos, etiqueta a los mantenedores relevantes en la PR. Mantén este archivo actualizado cuando cambien los procesos de CI o la estructura del repo.