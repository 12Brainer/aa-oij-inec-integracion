# 🤖 Aprendizaje Automático — Trabajo Práctico 03

Este repositorio contiene el **Trabajo Práctico 03** del curso **Aprendizaje Automático**.  
El objetivo principal es trabajar con **datasets reales del OIJ e INEC**, aplicando técnicas de **limpieza, integración y normalización** de datos para preparar la información antes del modelado.

---

## 📂 Contenido del notebook

- **Conjuntos de Datos**  
  - **OIJ:** estadísticas de criminalidad por distrito.  
  - **INEC:** información demográfica y socioeconómica (incluyendo desempleo).  
  - Procesos de carga desde archivos Excel/CSV.  

- **Preprocesamiento y Limpieza**  
  - Revisión y estandarización de columnas.  
  - Eliminación de registros inválidos y nulos.  
  - Normalización de nombres de distritos con **unidecode**.  
  - Aplicación de **fuzzy matching (rapidfuzz)** para resolver inconsistencias en nombres de distritos.  

- **Integración de Datos**  
  - Unión de las bases de OIJ e INEC a nivel de distrito.  
  - Generación de un dataset consolidado que muestra, para cada distrito:  
    - La **cantidad de delitos reportados**.  
    - La **tasa de desempleo**.  
  - Validación de correspondencia entre distritos.  
  - Revisión de la calidad de los datos resultantes.  

---

## ⚙️ Requisitos

Para ejecutar este notebook necesitas:

- Python 3.8+
- [Jupyter Notebook](https://jupyter.org/) o [JupyterLab](https://jupyter.org/install)
- Librerías:
  - `numpy`
  - `pandas`
  - `unidecode`
  - `rapidfuzz`
  - `openpyxl`  

Instala las dependencias con:

```bash
pip install numpy pandas unidecode rapidfuzz openpyxl
