# 🌐 Los 5 Pilares del Ciclo de Vida del Dato

Práctica de colaboración en GitHub: cada alumno/a escribe **una tarjeta** de la web siguiendo el ciclo completo
**issue → rama → commit → pull request → review → merge**, organizado en el **Project** del repo.

Duración aproximada: 45–60 min.

---

## 🃏 Tarjetas

Cada equipo tiene una página con 4 tarjetas ya preparadas. Cada persona elige **una** (si sois más de 4, trabajad en pareja) y copia el texto en su bloque `TARJETA N`. Despliega tu equipo para ver el contenido:

<details>
<summary><b>Equipo 1 · Origen y Captura</b> · <code>data-origin/data-origin.html</code></summary>

1. **Fuentes estructuradas y no estructuradas**
   - `<h3>`: Datos ordenados y datos caóticos
   - `<p>`: Las fuentes estructuradas (bases de datos, APIs, ERP) tienen un formato fijo de filas y columnas. Las no estructuradas (logs, sensores, redes sociales) llegan como texto, imágenes o eventos y hay que procesarlas antes de usarlas.

2. **Recolección e ingestión**
   - `<h3>`: Cómo entran los datos al sistema
   - `<p>`: La ingestión es el proceso de traer datos desde su origen a un almacén central. Puede hacerse por lotes (batch), por ejemplo cada noche, o en tiempo real (streaming), a medida que los datos se generan.

3. **Data Governance**
   - `<h3>`: Reglas del juego para los datos
   - `<p>`: El gobierno del dato define quién es responsable de cada dato, quién puede acceder y con qué calidad mínima debe estar. Sin estas reglas, cada equipo acaba con su propia versión de la verdad.

4. **Metadatos y procedencia**
   - `<h3>`: Datos sobre los datos
   - `<p>`: Los metadatos describen un dato: su origen, su formato, cuándo se creó y quién lo modificó. La procedencia (data lineage) permite rastrear de dónde viene cada cifra de un informe.

</details>

<details>
<summary><b>Equipo 2 · Limpieza y Transformación</b> · <code>data-cleaning/data-cleaning.html</code></summary>

1. **Data Wrangling y calidad**
   - `<h3>`: Ordenar antes de analizar
   - `<p>`: El data wrangling consiste en limpiar, unificar y dar forma a los datos en bruto. Se calcula que ocupa gran parte del tiempo de un proyecto de datos, porque un análisis solo es tan bueno como los datos que usa.

2. **Valores nulos y outliers**
   - `<h3>`: Huecos y valores extremos
   - `<p>`: Los valores nulos son datos que faltan y se pueden eliminar o rellenar (por ejemplo, con la media). Los outliers son valores muy alejados del resto: pueden ser errores o casos reales importantes, así que hay que revisarlos antes de borrarlos.

3. **ETL/ELT y pipelines**
   - `<h3>`: Extraer, transformar y cargar
   - `<p>`: ETL extrae los datos, los transforma y después los carga en el almacén. ELT los carga primero y los transforma dentro del almacén. Un pipeline automatiza estos pasos para que se ejecuten solos y siempre igual.

4. **Feature Engineering**
   - `<h3>`: Crear variables útiles
   - `<p>`: El feature engineering transforma los datos en variables que un modelo entiende mejor. Por ejemplo, a partir de una fecha se puede crear el día de la semana o si era festivo.

</details>

<details>
<summary><b>Equipo 3 · Análisis y Modelado</b> · <code>data-analysis/data-analysis.html</code></summary>

1. **Estadística descriptiva y visualización**
   - `<h3>`: Resumir y ver los datos
   - `<p>`: La estadística descriptiva resume los datos con medidas como la media, la mediana o la desviación típica. Los gráficos (histogramas, diagramas de dispersión) ayudan a detectar patrones que una tabla esconde.

2. **Machine Learning**
   - `<h3>`: Aprender a partir de ejemplos
   - `<p>`: En el aprendizaje supervisado el modelo aprende con ejemplos etiquetados, como emails marcados como spam o no spam. En el no supervisado busca estructura por sí mismo, sin etiquetas.

3. **Experimentación y validación**
   - `<h3>`: Comprobar que el modelo funciona
   - `<p>`: Para saber si un modelo generaliza, se entrena con una parte de los datos y se evalúa con otra que no ha visto. Técnicas como la validación cruzada y los tests A/B evitan conclusiones engañosas.

4. **Segmentación y patrones**
   - `<h3>`: Encontrar grupos ocultos
   - `<p>`: El clustering agrupa elementos parecidos sin saber de antemano qué grupos existen. Se usa, por ejemplo, para segmentar clientes según su comportamiento de compra.

</details>

<details>
<summary><b>Equipo 4 · Despliegue y Monitorización</b> · <code>deployment/deployment.html</code></summary>

1. **MLOps**
   - `<h3>`: Llevar modelos a producción
   - `<p>`: MLOps aplica las prácticas de DevOps a los modelos de machine learning: versionado, pruebas automáticas y despliegue continuo. Su objetivo es que un modelo pase del notebook a producción de forma fiable.

2. **Dashboards y reporting**
   - `<h3>`: Datos a la vista de todos
   - `<p>`: Un dashboard muestra los indicadores clave de forma visual y actualizada. Herramientas como Power BI, Tableau o Looker Studio permiten automatizar informes que antes se hacían a mano.

3. **Recomendación en tiempo real**
   - `<h3>`: Sugerencias al instante
   - `<p>`: Los sistemas de recomendación proponen productos o contenidos según el comportamiento del usuario. En tiempo real, el modelo responde en milisegundos mientras la persona navega, como en Netflix o Spotify.

4. **Monitorización y mantenimiento**
   - `<h3>`: Vigilar el modelo en producción
   - `<p>`: Con el tiempo los datos cambian y el modelo pierde precisión (data drift). Monitorizar sus métricas permite detectarlo a tiempo y reentrenarlo antes de que tome malas decisiones.

</details>

<details>
<summary><b>Equipo 5 · Impacto y Dirección Estratégica</b> · <code>strategic-direction/strategic-direction.html</code></summary>

1. **Storytelling con datos**
   - `<h3>`: Contar historias con datos
   - `<p>`: El storytelling combina datos, visualizaciones y narrativa para explicar un hallazgo. Una buena historia responde a qué ha pasado, por qué importa y qué decisión hay que tomar.

2. **ROI e impacto en negocio**
   - `<h3>`: ¿Merece la pena el proyecto?
   - `<p>`: El retorno de la inversión (ROI) compara el beneficio de un proyecto de datos con lo que ha costado. Medirlo ayuda a justificar nuevos proyectos y a priorizar los que más valor aportan.

3. **Retroalimentación y mejora**
   - `<h3>`: Aprender de los resultados
   - `<p>`: Los resultados de cada decisión generan nuevos datos que vuelven al inicio del ciclo. Este bucle de retroalimentación permite mejorar los modelos y los procesos de forma continua.

4. **Ética, privacidad y gobierno**
   - `<h3>`: Usar los datos con responsabilidad
   - `<p>`: Trabajar con datos implica respetar la privacidad de las personas y leyes como el RGPD. También hay que vigilar los sesgos de los modelos para que no discriminen a ningún colectivo.

</details>


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
3. En el panel derecho del issue:
   - **Assignees** → asígnatelo.
   - **Projects** → el issue ya aparece en el tablero. Pon tu **Equipo** y cambia **Status** a **In Progress**.

### 3. Crea la rama desde el issue

En el issue, panel derecho: **Development → Create a branch → Checkout locally**. GitHub te da los comandos:

```bash
git fetch origin
git checkout <nombre-de-la-rama>
```

### 4. Escribe tu tarjeta

Edita **solo** tu bloque `TARJETA N` en el HTML de tu equipo: copia el `<h3>` y el `<p>` de la sección **Tarjetas**.
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
3. Copia la plantilla del Project a la organización y enlázala al repo:

   ```bash
   gh project copy 56 --source-owner Factoria-F5-madrid --target-owner <org> --title "Pilares del Dato"
   gh project link <numero-nuevo> --owner <org> --repo <org>/hello_world_from_PR
   ```

   Ya trae el tablero, el campo **Equipo**, la vista **Mis tarjetas** y los workflows de **Todo** y **Done** automáticos.
   Si no tienes `gh`, desde la organización: **Projects → New project → Templates** (solo dentro de Factoria-F5-madrid).
4. En el Project copiado: **⋯ → Workflows → Auto-add to project**, actívalo con el filtro `is:issue` para este repo (GitHub no copia este workflow).
5. En el Project: **⋯ → Settings → Manage access**, da permiso **Write** a los alumnos para que puedan mover tarjetas.
6. Opcional: protege `main` (**Settings → Branches**) exigiendo 1 aprobación antes del merge.
