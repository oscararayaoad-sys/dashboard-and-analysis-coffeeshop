# ☕ Dashboard y Análisis de cafetería

Un análisis integral de datos de ventas y comportamiento del consumidor enfocado en optimizar la estrategia comercial y la rentabilidad de una cafetería mediante el uso de Python y Power BI.

---

## 2. Insignias / Badges

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![License](https://img.shields.io/badge/Licencia-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Estado-Completado-blue?style=for-the-badge)

---

## 3. Tabla de Contenidos

1. [Características Principales / Objetivos](#4-características-principales--objetivos)
2. [Arquitectura / Estructura del Repositorio](#5-arquitectura--estructura-del-repositorio)
3. [Requisitos Previos e Instalación](#6-requisitos-previos-e-instalación)
4. [Guía de Uso / Ejemplos Rápidos](#7-guía-de-uso--ejemplos-rápidos)
5. [Tecnologías Utilizadas](#8-tecnologías-utilizadas)
6. [Resultados o Demo](#9-resultados-o-demo-capturas--gifs)
7. [Licencia y Créditos / Autor](#10-licencia-y-créditos--autor)

---

## 4. Características Principales / Objetivos

* **Análisis Exploratorio de Datos (EDA):** Limpieza, agregación e identificación de patrones de compra y horas pico de ventas.
* **Segmentación Estratégica:** Clasificación de productos a través de una **Matriz BCG** (Productos Estrella, Vaca, Incógnita y Perro) para orientar decisiones de menú y pricing.
* **Análisis de Coocurrencia:** Identificación de combinaciones frecuentes de productos (ventas cruzadas) para estrategias de *bundling*.
* **Visualización Interactiva:** Creación de un Dashboard dinámico en Power BI para el monitoreo de KPIs de negocio.

---

## 5. Arquitectura / Estructura del Repositorio

```text
dashboard-and-analysis-coffeeshop/
├── data/
│   ├── raw/                # Datos originales sin procesar
│   └── processed/          # Datos limpios y listos para Power BI
├── notebooks/
│   ├── 01_cleaning_cafeteria.ipynb   # EDA y Limpieza de datos
│   └── 02_analyzed_cafeteria.ipynb   #Matriz BCG y Análisis de Coocurrencia
├── dashboard/
│   └── 03_dashboard_cafeteria.pbix # Reporte interactivo de Power BI
├── assets/
├── src/
│   └── README.es.md
├── .gitignore
├── LICENSE
├── README.es.md
└── requirements.txt
```

---

## 6. Requisitos Previos e Instalación

### Requisitos
* **Python 3.10+**
* **Power BI Desktop** (para visualizar el archivo `.pbix`)

### Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/oscararayaoad-sys/dashboard-and-analysis-coffeeshop.git
   cd dashboard-and-analysis-coffeeshop
   ```

2. Crea un entorno virtual e instala las dependencias:
   ```bash
   python -m venv venv
   source venv/bin/activate  # En Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

---

## 7. Guía de Uso / Ejemplos Rápidos

1. **Ejecutar la canalización de datos (EDA/Procesamiento):**
   ```bash
   jupyter notebook notebooks/01_cleaning_cafeteria.ipynb
   ```
2. **Abrir el Dashboard:**
   Navega a la carpeta `dashboard/` y abre `03_dashboard_cafeteria.pbix` directamente en **Power BI Desktop**.

---

## 8. Tecnologías Utilizadas

* **Lenguaje:** Python 3.10+
* **Librerías de Análisis:** Pandas, NumPy
* **Librerías de Visualización:** Seaborn, Matplotlib
* **Business Intelligence:** Microsoft Power BI (DAX, Power Query)

---

## 9. Resultados o Demo (Capturas / GIFs)

### 📊 Dashboard Interactivo (Power BI)

> *Demostración del panel de control dinámico en Power BI para el monitoreo de ventas y KPIs.*

| Dashboard Interactividad |
| :---: |
| ![Power BI Demo](assets/powerbi_dashboard.gif) |
*(Si no tienes un GIF, puedes reemplazar la ruta por una captura `.png` o `.jpg` del dashboard)*

---

### 🔍 Hallazgos Clave del Análisis de Datos (Python / Seaborn)

El análisis exploratorio reveló patrones críticos para la toma de decisiones comerciales:

| Matriz BCG (Portafolio) | Mapa de Calor: Hora vs Día |
| :---: | :---: |
| ![Matriz BCG](assets/grafico_6.png) | ![Demanda por Hora y Día](assets/grafico_1.png) |
| **Segmentación Estratégica:** Clasificación de productos según margen e ingresos (*Estrellas*, *Caballos de batalla*, *Interrogantes* y *Perros*). | **Horas Pico:** Identificación clara de horas de alta demanda (especialmente a las 09:00 hrs todos los días) para optimizar turnos de personal. |

| Tipo de Servicio por Categoría | Métodos de Pago Preferidos |
| :---: | :---: |
| ![Tipo de Servicio](assets/grafico_3.png) | ![Metodo de Pago](assets/grafico_4.png) |
| **Preferencia de Consumo:** Predominio masivo del consumo *"Para servir"* frente a *"Para llevar"*, destacando las categorías de Cafés y Repostería. | **Comportamiento Financiero:** La tarjeta de Débito es el método de pago principal en todas las categorías, seguido por Crédito. |

---

## 10. Licencia y Créditos / Autor

* **Licencia:** Distribuido bajo la Licencia MIT. Consulta `LICENSE` para más información.
* **Autor:** Oscar Araya ([@oscararayaoad-sys](https://github.com/oscararayaoad-sys))
