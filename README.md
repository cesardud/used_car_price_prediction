# 🚗 Predicción de Precios de Autos Usados — Rusty Bargain

Este proyecto utiliza modelos de machine learning para predecir el valor de mercado de coches de segunda mano, como parte de la app desarrollada por la compañía ficticia **Rusty Bargain**.

El objetivo es comparar distintos algoritmos de regresión en cuanto a su **precisión**, **velocidad de predicción** y **tiempo de entrenamiento**.

---

## 🎯 Objetivo

Construir un modelo que prediga con precisión el precio de un coche usado, utilizando datos como:

- Tipo de vehículo
- Año de matriculación
- Potencia del motor
- Tipo de combustible
- Marca, modelo, kilometraje
- Reparaciones, fecha de creación del perfil, entre otros

---

## 🛠️ Herramientas y tecnologías

- Python 3
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- LightGBM
- CatBoost
- Regresión lineal, árbol de decisión, bosque aleatorio, boosting

---

## 📊 Dataset

El dataset está disponible en el archivo `car_data.csv`.

**Características destacadas:**

- `VehicleType`: tipo de carrocería
- `RegistrationYear` y `RegistrationMonth`: año y mes de matriculación
- `Power`: potencia del motor (CV)
- `FuelType`: tipo de combustible
- `Brand`, `Model`: marca y modelo del vehículo
- `NotRepaired`: si el coche ha sido reparado o no
- `Mileage`: kilometraje
- `Price`: (objetivo) precio de venta en euros

---

## 🧠 Modelos utilizados

Se compararon distintos enfoques:

### 🔹 Regresión lineal
- Modelo base para comparación.
- Muy rápido, pero con baja capacidad predictiva.

### 🌳 Árbol de decisión y bosque aleatorio
- Modelos interpretables y eficientes.
- Buen desempeño con variables categóricas codificadas.

### ⚡ Boosting (LightGBM y CatBoost)
- Mejores resultados en precisión.
- Mayor tiempo de entrenamiento, pero excelente para producción.

---

## 📈 Métricas evaluadas

- **R² Score**: qué tan bien el modelo explica la varianza del precio.
- **RMSE**: error cuadrático medio.
- **Tiempo de entrenamiento**.
- **Velocidad de predicción**.

---

## 🚀 Cómo ejecutarlo

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/used-car-price-prediction.git
   cd used-car-price-prediction

2. Crea y activa un entorno virtual:
   ```bash
   python3 -m venv venv
   source venv/bin/activate

3. Instala dependencias:
   ```bash
   pip install -r requirements.txt

4. Ejecuta en notebook:
   ```bash
   code notebook.ipynb

