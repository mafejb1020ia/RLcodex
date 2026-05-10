# Análisis de Supervivencia del Titanic

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)


Proyecto de analítica de datos en Python usando el archivo `tested.csv`. El cuaderno principal, `RL_Housing.ipynb`, desarrolla un flujo completo en español: comprensión del dataset, exploración, limpieza, ingeniería de variables, entrenamiento de una regresión logística, evaluación e interpretación de resultados.

## Archivos del proyecto

| Archivo | Descripción |
|---|---|
| `RL_Housing.ipynb` | Cuaderno Jupyter con el análisis completo y el modelo predictivo. |
| `tested.csv` | Dataset base con información de pasajeros del Titanic. |
| `README.md` | Documentación del proyecto. |
| `index.html` | Página de presentación lista para GitHub Pages. |

## Datos

El dataset contiene 418 registros y 12 columnas originales:

- `PassengerId`, `Survived`, `Pclass`, `Name`, `Sex`, `Age`, `SibSp`, `Parch`, `Ticket`, `Fare`, `Cabin`, `Embarked`.

La variable objetivo es `Survived`, donde `0` indica que el pasajero no sobrevivió y `1` indica que sobrevivió.

## Flujo del análisis

1. Carga y validación del archivo CSV.
2. Revisión de estructura, tipos de datos y valores faltantes.
3. Análisis exploratorio con tablas y visualizaciones.
4. Creación de variables derivadas como `Title`, `FamilySize`, `IsAlone`, `FarePerPerson` y `Deck`.
5. Preparación de variables numéricas y categóricas con un pipeline de `scikit-learn`.
6. Entrenamiento de un modelo de regresión logística.
7. Evaluación con accuracy, AUC ROC, matriz de confusión y validación cruzada.
8. Generación de predicciones en `titanic_predictions.csv`.

## Requisitos

Instala las librerías necesarias con:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Ejecución

Abre el cuaderno con Jupyter:

```bash
jupyter notebook RL_Housing.ipynb
```

También puedes abrirlo en JupyterLab:

```bash
jupyter lab RL_Housing.ipynb
```

Ejecuta las celdas de arriba hacia abajo. El cuaderno está preparado para trabajar con `tested.csv` en la misma carpeta.

## Nota analítica

En este archivo, la variable `Survived` está muy asociada con `Sex`. Por esa razón, el modelo puede alcanzar métricas altas. El cuaderno incluye una revisión crítica de esta relación para evitar interpretar el resultado como una prueba definitiva de causalidad o como una validación histórica independiente.

## Publicación en GitHub Pages

El archivo `index.html` sirve como página principal del repositorio. Para publicarlo:

1. Sube todos los archivos a GitHub.
2. Entra a `Settings > Pages`.
3. Selecciona la rama principal y la carpeta raíz.
4. Guarda la configuración.

GitHub Pages mostrará automáticamente la página `index.html`.

## Reconocimientos

Este proyecto y los conocimientos aplicados fueron adquiridos y desarrollados durante el curso de formación de **Talento Tech**.

