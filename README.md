# 🌐 Los 5 Pilares del Ciclo de Vida del Dato

Práctica de colaboración en GitHub: cada alumno/a escribe **una tarjeta** de la web siguiendo el ciclo completo
**issue → rama → commit → pull request → review → merge**, organizado en el **Project** del repo.

Duración aproximada: 45–60 min.

---

## 🃏 Tarjetas disponibles

Cada equipo tiene una página con 4 tarjetas ya preparadas. Cada persona elige **una tarjeta** (si sois más, trabajad en pareja).

| Equipo | Archivo | Tarjetas |
|---|---|---|
| 1 · Origen y Captura | `data-origin/data-origin.html` | 1 Fuentes estructuradas y no estructuradas · 2 Recolección e ingestión · 3 Data Governance · 4 Metadatos y procedencia |
| 2 · Limpieza y Transformación | `data-cleaning/data-cleaning.html` | 1 Data Wrangling y calidad · 2 Valores nulos y outliers · 3 ETL/ELT y pipelines · 4 Feature Engineering |
| 3 · Análisis y Modelado | `data-analysis/data-analysis.html` | 1 Estadística descriptiva · 2 Machine Learning · 3 Experimentación y validación · 4 Segmentación y patrones |
| 4 · Despliegue y Monitorización | `deployment/deployment.html` | 1 MLOps · 2 Dashboards y reporting · 3 Recomendación en tiempo real · 4 Monitorización y mantenimiento |
| 5 · Impacto y Dirección Estratégica | `strategic-direction/strategic-direction.html` | 1 Storytelling con datos · 2 ROI e impacto · 3 Retroalimentación y mejora · 4 Ética, privacidad y gobierno |

Mira `examples/examples.html` para ver cómo queda una tarjeta terminada.

---

## 🧭 Pasos

### 1. Clona el repo

```bash
git clone https://github.com/<organizacion-del-bootcamp>/hello_world_from_PR.git
cd hello_world_from_PR
```

### 2. Crea tu issue

1. Abre la pestaña **Projects** del repo y comprueba que nadie ha reservado ya tu tarjeta.
2. **Issues → New issue → 🃏 Mi tarjeta**. Título: `Tarjeta: Equipo 1 · Recolección e ingestión`.
3. Asígnatelo (**Assignees → assign yourself**).
4. El issue aparece solo en el Project, en **Todo**. Muévelo a **In Progress**.

### 3. Crea la rama desde el issue

En el issue, panel derecho: **Development → Create a branch → Checkout locally**. GitHub te da los comandos:

```bash
git fetch origin
git checkout <nombre-de-la-rama>
```

### 4. Escribe tu tarjeta

Edita **solo** tu bloque `TARJETA N` en el HTML de tu equipo: cambia el `<h3>` y el `<p>`.
Abre `index.html` en el navegador para comprobar cómo queda.

### 5. Commit y push

```bash
git add .
git commit -m "Añade tarjeta Recolección e ingestión"
git push -u origin <nombre-de-la-rama>
```

### 6. Abre el Pull Request

1. GitHub muestra el botón **Compare & pull request**. Base: `main`.
2. En la descripción escribe `Closes #<número-de-tu-issue>`, así el issue se cierra solo al hacer merge.
3. En **Reviewers** pide revisión a un compañero/a de tu equipo.

### 7. Review y merge

- **Quien revisa**: abre **Files changed**, deja al menos un comentario y pulsa **Review changes → Approve**.
- **El/la instructor/a** hace el merge. El issue se cierra y la tarjeta pasa a **Done** en el Project.

---

## 🆘 Problemas comunes

- **`git push` rechazado**: seguramente estás en `main`. Haz `git checkout <tu-rama>`.
- **El PR tiene conflictos**: has editado fuera de tu bloque `TARJETA N`. Deshaz esos cambios.
- **No aparece la plantilla**: estás en otro repo. Revisa que la URL sea la de la organización del bootcamp.

## ⭐ Extra para quien acabe antes: provocar un conflicto

Dos personas cambian el mismo `<h2>` de su página en ramas distintas y abren PR. Al hacer merge del primero,
el segundo tendrá conflicto. Resolvedlo:

```bash
git checkout <tu-rama>
git pull origin main
```

Editad el archivo, dejad la versión buena (borrad `<<<<<<<`, `=======`, `>>>>>>>`), y haced commit y push.

---

## 👩‍🏫 Preparación (solo instructor/a)

Este repo es la plantilla original: **no se trabaja aquí**. Para cada bootcamp:

1. Haz fork a la organización del bootcamp y desvincúlalo del original (**Settings → Danger Zone → Leave fork network**).
2. En el fork: **Settings → General → Features**, activa **Issues** y **Projects**. Añade a los alumnos con permiso **Write**.
3. En la organización: **Projects → New project → Board**. Nómbralo, por ejemplo, `Pilares del Dato`.
4. En el repo: pestaña **Projects → Link a project** y elige el tablero.
5. En el Project: **⋯ → Workflows**:
   - Activa **Auto-add to project** con el filtro `is:issue,pr` para este repo.
   - Comprueba que **Item closed** y **Pull request merged** mueven a **Done** (vienen activados).
6. En el Project: **⋯ → Settings → Manage access**, da permiso **Write** a los alumnos para que puedan mover tarjetas.
7. Opcional: protege `main` (**Settings → Branches**) exigiendo 1 aprobación antes del merge.
