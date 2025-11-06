# 🏙️ Análisis de Datos de Airbnb en Nueva York

Este proyecto analiza un conjunto de datos de **Airbnb en la ciudad de Nueva York (2019)** con el objetivo de comprender mejor las características, tendencias y patrones del mercado de alquiler vacacional.  
El análisis se centra en la **exploración, limpieza y preparación de los datos** para su uso en estudios posteriores o modelos predictivos.

---

## 🎯 Objetivos del proyecto

1. **Exploración y comprensión de los datos:**  
   Analizar la estructura del dataset, revisar la calidad de los datos y comprender las variables más relevantes.

2. **Limpieza y preprocesamiento:**  
   Eliminar duplicados, valores atípicos y columnas irrelevantes para garantizar un conjunto de datos limpio y confiable.

3. **División del dataset:**  
   Separar los datos en conjuntos de entrenamiento y prueba para futuros modelos de machine learning.

4. **Almacenamiento de datos procesados:**  
   Guardar los datos finales en `./data/processed` (no incluido en el repositorio por privacidad y tamaño).

---

## 🧩 Dataset

**Fuente:**  
[AB_NYC_2019.csv](https://raw.githubusercontent.com/4GeeksAcademy/data-preprocessing-project-tutorial/main/AB_NYC_2019.csv)

El *dataset* inicial contiene **48,895 entradas** y **16 columnas**.

### Resumen de Características

| Columna | Tipo de Dato | Recuento No Nulo | Descripción |
| :--- | :--- | :--- | :--- |
| `id` | `int64` | 48895 | Identificador de la vivienda. |
| `name` | `object` | 48879 | Nombre del anuncio (categórico). |
| `host_id` | `int64` | 48895 | Identificador del arrendador. |
| `host_name` | `object` | 48874 | Nombre del arrendador (categórico). |
| `neighbourhood_group` | `object` | 48895 | Grupo de vecindario (categórico). |
| `neighbourhood` | `object` | 48895 | Vecindario específico (categórico). |
| `latitude` | `float64` | 48895 | Latitud de la ubicación. |
| `longitude` | `float64` | 48895 | Longitud de la ubicación. |
| `room_type` | `object` | 48895 | Tipo de habitación. |
| `price` | `int64` | 48895 | Precio por noche. |
| `minimum_nights` | `int64` | 48895 | Estancia mínima requerida. |
| `number_of_reviews` | `int64` | 48895 | Número total de reseñas. |
| `last_review` | `object` | 38843 | Fecha de la última reseña (**contiene nulos**). |
| `reviews_per_month` | `float64` | 38843 | Reseñas por mes (**contiene nulos**). |
| `calculated_host_listings_count`| `int64` | 48895 | Listados calculados por anfitrión. |
| `availability_365` | `int64` | 48895 | Días de disponibilidad en el año. |

**Nota sobre los datos:** El *dataset* contiene 10 columnas de datos numéricos y 6 columnas de datos categóricos u *object*. Las columnas `name`, `host_name`, `last_review` y `reviews_per_month` contienen valores nulos que requieren tratamiento.

---

## 🧼 Limpieza de datos

Se eliminaron o modificaron:
- Columnas irrelevantes: `id`, `host_id`, `name`, `host_name`, `neighbourhood`
- Registros duplicados
- Valores nulos o inconsistentes

El objetivo fue dejar un dataset estructurado y útil para análisis posteriores.

---

## 🛠️ Tecnologías utilizadas

- **Python 3**
- **Pandas**
- **NumPy**
- **Jupyter Notebook**

---

## 🚀 Cómo ejecutar el proyecto

1. Clona este repositorio:  
   ```bash
   git clone https://github.com/<tu-usuario>/<tu-repo>.git
   cd <tu-repo>
   ```

2. Instala las dependencias necesarias:  
   ```bash
   pip install pandas numpy jupyter
   ```

3. Abre el notebook en Jupyter:  
   ```bash
   jupyter notebook explorar.ipynb
   ```

---

## 📊 Resultados esperados

- Dataset limpio y preparado para futuros análisis.
- Identificación de patrones en los precios, ubicaciones y disponibilidad.
- Base sólida para el desarrollo de modelos predictivos o dashboards interactivos.

---

## 📁 Estructura del proyecto

```
├── data/
│   ├── raw/             # Datos originales
│   └── processed/       # Datos limpios (no incluidos en el repo)
├── explore.ipynb        # Notebook principal
├── README.md            # Este archivo
└── requirements.txt     # Dependencias (opcional)
```

---

## 🧠 Autor

**Bryan Jumbo Torres**  
Proyecto desarrollado como parte de un ejercicio de análisis de datos.  