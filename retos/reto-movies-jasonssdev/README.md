# 🎬 Reto PyData Panamá – “Películas y Datos”

📌 **Descripción:**
> Analiza el dataset **IMDb MovieMetadata** (≈ 5 k films, 28 columnas) y descubre qué factores influyen en el éxito de una película usando Python y tus habilidades de análisis de datos.


📊 **Objetivo:**  
- Limpiar y explorar la información de películas.  
- Responder **10 preguntas** de negocio (listadas más abajo).  
- Ilustrar hallazgos con visualizaciones claras.  
- (Opcional) construir un pequeño modelo que prediga la recaudación (`gross`) a partir de 3 variables.

👤 **Autor del reto:**  
`jasonssdev`

---

## 📂 **Estructura del reto**
Este reto sigue la estructura estándar:
```plaintext
📂 reto-movies-jasonssdev/
 ├── README.md        # Explicación del reto
 ├── 📂 data/         # Datos del reto (dataset CSV)
 ├── 📂 src/          # Código base del reto (opcional)
 ├── 📂 tests/        # Pruebas unitarias (opcional)
 ├── 📂 submissions/  # Soluciones de los participantes
```

📢 * *Importante:**
- Si tu reto usa datasets, agrégalo en la carpeta `data/`.
- Si requiere código base, colócalo en `src/`.
- Las soluciones deben subirse en `submissions/` en formato `.ipynb`.

---

## 📌 **Datos del reto** (Si aplica)
📂 **Dataset:** `movies.csv`
🔹 **Descripción:** Información pública de ~5 000 películas: título, año, director, presupuesto, recaudación, puntuación IMDb, géneros, likes en Facebook de actores/director, etc.
🔹 **Fuente:** Adaptado del dataset IMDB 5000 Movie Dataset de Kaggle (licencia CC0).
🔹 **Diccionario de datos:**

| Columna                    | Descripción                                                  |
|----------------------------|--------------------------------------------------------------|
| `movie_title`              | Título de la película                                        |
| `title_year`               | Año de estreno                                               |
| `director_name`            | Nombre del director                                          |
| `genres`                   | Géneros separados por “\|”                                   |
| `country`                  | País principal de producción                                 |
| `budget`                   | Presupuesto (USD)                                            |
| `gross`                    | Recaudación mundial (USD)                                    |
| `imdb_score`               | Puntuación IMDb (0-10)                                       |
| `duration`                 | Duración en minutos                                          |
| `content_rating`           | Clasificación (PG-13, R, etc.)                               |
| `actor_1_name`             | Actor/actriz principal                                       |
| `director_facebook_likes`  | Likes del director en Facebook (proxy de popularidad)        |

---

## 🚀 **Cómo participar**

1️⃣ **Haz un fork del repositorio original**  
   Dirígete a <https://github.com/PyData-Panama/pydatapanama-retos> y presiona **Fork** para crear tu propia copia del proyecto en tu cuenta de GitHub.

2️⃣ **Clona *tu fork* en local**  
```bash
git clone git@github.com:<tu_usuario>/pydatapanama-retos.git
cd pydatapanama-retos
```

3️⃣ Crea una nueva rama con tu nombre de usuario
```bash
git checkout -b reto-movies-<tu_usuario>
```

4️⃣ Dirígete a la carpeta del reto y añade tu solución
```bash
cd retos/reto-movies-jasonssdev/submissions
```
```bash
touch solucion-{tu_usuario}.ipynb
```

5️⃣ Desarrolla tu solución y súbela a tu fork
```bash
git add .
git commit -m "🚀 Solución al reto Películas y Datos"
git push origin reto-movies-<tu_usuario>
```
6️⃣ Abre un Pull Request
Ve a tu fork en GitHub y pulsa “Compare & Pull Request” para enviar tu aporte al repositorio original. Asegúrate de completar el template de PR.
```
# pull request
```
---

## 🔹 **Criterios de evaluación**
Para evaluar las soluciones, se considerarán los siguientes aspectos:
✅ **Claridad y organización del código**
✅ **Uso adecuado de librerías de Python**
✅ **Calidad de la visualización (si aplica)**
✅ **Correctitud de los cálculos y análisis**

---

## 📚 **Recursos recomendados**
📌 [Documentación de Pandas](https://pandas.pydata.org/docs/)  
📌 [Documentación de Matplotlib](https://matplotlib.org/stable/contents.html)  
📌 [Documentación de Seaborn](https://seaborn.pydata.org/)  

---

🚀 **¡Esperamos tu participación!** Si tienes dudas, pregunta en nuestra comunidad o abre un Issue en GitHub. 😃

### ❓ Preguntas-desafío

1. **Duración promedio por década**  
   > ¿Cuál es la duración media de las películas y cómo ha evolucionado en cada década?

2. **Directores taquilleros**  
   > ¿Qué 5 directores acumulan la mayor recaudación total (`gross`) en el dataset?

3. **Presupuesto vs. Éxito crítico**  
   > ¿Existe correlación entre el presupuesto (`budget`) y la puntuación IMDb (`imdb_score`)?

4. **Género y clasificación**  
   > ¿Cuál es el género con el mayor porcentaje de películas clasificadas como **PG-13**?

5. **Críticas vs. Puntuación**  
   > ¿Cómo se relaciona el número de críticas de usuarios con la puntuación IMDb?

6. **Mercados más lucrativos**  
   > ¿Qué país presenta la **mediana** de recaudación (`gross`) más alta?

7. **Color vs. Blanco-y-negro**  
   > ¿Cómo difieren las puntuaciones IMDb entre películas a color y en blanco-y-negro?

8. **Rostro del éxito**  
   > ¿Qué actor o actriz aparece con mayor frecuencia entre las 100 películas con mejor puntuación IMDb?

9. **Recaudación por clasificación**  
   > ¿Cómo varía la recaudación (`gross`) según la clasificación por edad (`content_rating`)?  
   > (Comparar con un boxplot).

10. **Géneros más rentables**  
   > ¿Qué **tres géneros** presentan la recaudación promedio (`gross`) más alta?