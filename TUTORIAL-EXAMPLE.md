# Tutorial Práctico: Introducción a GitHub

Este documento proporciona un ejemplo práctico de cómo completar cada paso del tutorial "Introduction to GitHub".

---

## 📋 Pasos del Tutorial

### ✅ Paso 0: Bienvenida
**Estado:** Completado  
**Descripción:** Configuración inicial del repositorio desde la plantilla.

---

### ✅ Paso 1: Crear una rama (Create a branch)

**Objetivo:** Aprender a crear ramas para trabajar sin afectar la rama principal.

**Comandos ejecutados:**
```bash
# Crear y cambiar a una nueva rama
git checkout -b my-first-branch

# Verificar que estamos en la nueva rama
git branch
```

**Resultado:**
- ✓ Rama `my-first-branch` creada exitosamente
- ✓ La rama se separa del código principal (`main`)
- ✓ Ahora podemos hacer cambios sin afectar `main`

**Archivo modificado:** Ninguno (solo se creó la rama)

---

### ✅ Paso 2: Hacer un commit (Commit a file)

**Objetivo:** Aprender a crear archivos y hacer commits para guardar cambios.

**Comandos ejecutados:**
```bash
# Crear el archivo PROFILE.md
echo "Welcome to my GitHub profile!" > PROFILE.md

# Agregar el archivo al staging area
git add PROFILE.md

# Hacer commit con un mensaje descriptivo
git commit -m "Add PROFILE.md"
```

**Resultado:**
- ✓ Archivo `PROFILE.md` creado
- ✓ Commit realizado con mensaje descriptivo
- ✓ Cambios guardados en la rama `my-first-branch`

**Archivos creados:**
- `PROFILE.md` (contenido: "Welcome to my GitHub profile!")

---

### 🔄 Paso 3: Abrir un Pull Request (Open a pull request)

**Objetivo:** Proponer cambios y solicitar revisión antes de integrarlos.

**Proceso:**
1. Empujar la rama al repositorio remoto:
   ```bash
   git push -u origin my-first-branch
   ```

2. En GitHub:
   - Ir a la pestaña "Pull requests"
   - Hacer clic en "New pull request"
   - Seleccionar `main` como rama base
   - Seleccionar `my-first-branch` como rama a comparar
   - Agregar título: "Add my first file"
   - Agregar descripción explicando los cambios
   - Hacer clic en "Create pull request"

**Beneficios:**
- ✓ Permite revisar cambios antes de integrarlos
- ✓ Facilita la colaboración en equipo
- ✓ Mantiene un registro de discusiones sobre el código

---

### 🎯 Paso 4: Fusionar el Pull Request (Merge your pull request)

**Objetivo:** Integrar los cambios aprobados a la rama principal.

**Proceso:**
1. Revisar los cambios en el PR
2. Esperar a que pasen las verificaciones (si existen)
3. Hacer clic en "Merge pull request"
4. Confirmar con "Confirm merge"
5. Opcionalmente, eliminar la rama fusionada

**Comandos equivalentes (línea de comandos):**
```bash
# Cambiar a la rama principal
git checkout main

# Fusionar my-first-branch
git merge my-first-branch

# Eliminar la rama local (opcional)
git branch -d my-first-branch
```

**Resultado:**
- ✓ Cambios integrados a la rama principal
- ✓ `PROFILE.md` ahora está en `main`
- ✓ Historial de cambios preservado

---

## 🚀 Ejemplo Adicional: Flujo de Trabajo Completo

Este repositorio demuestra un flujo de trabajo real con múltiples características:

### Característica 1: PROFILE.md básico
- **Rama:** `my-first-branch`
- **Commit:** "Add PROFILE.md"
- **Integración:** Fusionado a `copilot/update-all-features`

### Característica 2: Sección de habilidades
- **Rama:** `feature/add-skills-section`
- **Commit:** "Add skills and projects section to demonstrate Git workflow"
- **Contenido agregado:**
  - Sección "About Me"
  - Lista de habilidades con checkboxes
  - Proyectos actuales
  - Habilidades de GitHub completadas

### Característica 3: Tutorial práctico
- **Rama:** `feature/add-tutorial-example`
- **Commit:** "Add practical tutorial example showing all steps"
- **Archivo:** `TUTORIAL-EXAMPLE.md` (este archivo)

---

## 📊 Resumen de Comandos Git Básicos

| Comando | Descripción |
|---------|-------------|
| `git branch` | Listar ramas locales |
| `git checkout -b <nombre>` | Crear y cambiar a nueva rama |
| `git status` | Ver estado de archivos |
| `git add <archivo>` | Agregar archivo al staging |
| `git commit -m "mensaje"` | Crear commit con mensaje |
| `git push origin <rama>` | Empujar rama al remoto |
| `git merge <rama>` | Fusionar rama en la actual |
| `git log --oneline` | Ver historial de commits |

---

## 🎓 Conceptos Clave Aprendidos

1. **Branching (Ramificación):** Crear líneas paralelas de desarrollo
2. **Commits:** Guardar snapshots de cambios
3. **Pull Requests:** Proponer y revisar cambios
4. **Merging:** Integrar cambios de diferentes ramas
5. **Workflow:** Flujo completo desde desarrollo hasta producción

---

## ✨ ¡Felicitaciones!

Has completado exitosamente la introducción a GitHub. Ahora puedes:
- ✅ Crear y gestionar ramas
- ✅ Hacer commits significativos
- ✅ Colaborar usando Pull Requests
- ✅ Integrar cambios de manera segura

### Próximos pasos:
1. Crear tu propio repositorio de perfil
2. Explorar proyectos open source
3. Contribuir a proyectos existentes
4. Tomar más cursos de GitHub Skills

---

**Fecha de creación:** 2025-11-14  
**Estado del tutorial:** ✅ Completado  
**Ramas creadas:** `my-first-branch`, `feature/add-skills-section`, `feature/add-tutorial-example`
