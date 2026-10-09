# Dashboard PCA Bancario

Web estática basada en el diseño exportado de Stitch, conectada al archivo real `dataset_pca.csv`.

## Publicar en GitHub Pages

1. Descomprime el ZIP.
2. En GitHub, crea un repositorio llamado `dashboard-pca-bancario`. Para GitHub Free, utiliza un repositorio público.
3. Sube los archivos contenidos en esta carpeta a la raíz del repositorio. `index.html` debe verse directamente al abrir el repositorio: no subas solo el ZIP ni una carpeta contenedora adicional.
4. Guarda la subida con **Commit changes**.
5. En **Settings → Pages → Build and deployment**, selecciona **Deploy from a branch**.
6. Elige **main** y **/(root)**, y pulsa **Save**.
7. Cuando termine la publicación, GitHub Pages mostrará el enlace de la web.

Documentación oficial: https://docs.github.com/es/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Archivos

- `index.html`: secciones del dashboard.
- `styles.css`: estilo azul y verde basado en Stitch, adaptado a móvil.
- `app.js`: lectura, validación, filtros, gráfico y descarga.
- `dataset_pca.csv`: 41 188 filas reales, seis componentes y la columna y.
- `DESIGN.md`: referencia de diseño original exportada de Stitch; no es una especificación de los resultados estadísticos.

No necesita instalar librerías, compilar ni ejecutar Python para funcionar en GitHub Pages. No usa servicios externos para procesar el CSV.

## Probar en tu computadora

Abre `index.html` con tu navegador. Si el navegador bloquea la carga automática de archivos locales, pulsa **Cargar CSV** y selecciona el CSV incluido.

## Funcionalidad

- Carga automática del CSV en GitHub Pages y carga manual de otro archivo con las mismas siete columnas.
- Conteos y porcentajes reales calculados con todos los registros.
- Dispersión con ejes seleccionables y muestra reproducible de hasta 5 000 puntos.
- Filtro por clase para gráfico y tabla; búsqueda adicional para tabla y descarga.
- Paginación y exportación de todas las filas filtradas, sin redondear los datos de la descarga.
- Validación de encabezados, números, clases y filas incompletas. Un error conserva el último dataset válido.

## Alcance de los resultados

El análisis previo usó StandardScaler y PCA sobre las 10 variables predictoras numéricas originales. Se conservaron seis componentes, equivalentes al 91,54 % de la varianza original estandarizada. La varianza acumulada por número de componentes fue 38,95; 52,54; 63,32; 73,82; 83,12; 91,54 %.

El CSV reducido no incluye el modelo PCA, sus cargas ni los porcentajes de varianza. Estos porcentajes son metadatos del análisis original. Si se carga otro CSV, no se recalculan ni se atribuyen a ese archivo.

PCA no utiliza y para construir los componentes. No se evaluó un clasificador: la varianza explicada no es exactitud predictiva. Los componentes no reciben etiquetas interpretativas inventadas.

La clase yes tiene 4 640 registros y no tiene 36 548. Las cifras se calculan al cargar el archivo, no mediante filas simuladas.

## Cambios respecto a Stitch

Las cuatro pantallas se integraron en una sola página con navegación por secciones, manteniendo la paleta y las tarjetas del diseño. Se sustituyeron los datos simulados, los gráficos de ejemplo y las etiquetas de componentes no justificadas por datos reales y funciones conectadas al CSV. Se eliminaron dependencias de CSS externas.

## Verificación

Se verificaron la sintaxis JavaScript, lectura de las 41 188 filas, conteos por clase, exportación filtrada, muestreo reproducible y rechazo de archivos inválidos. La revisión visual en navegador queda pendiente.
