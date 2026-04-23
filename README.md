# **ANALISIS DE DATOS END TO END**

## **VIOLENCIA INTRAFAMILIAR EN COLOMBIA.**

**Autor:** Ovidio Antonio Guerreo Mosquera<br>
**Fecha:** 16/04/2025<br>
**Dataset:** Reporte Delito Violencia Intrafamiliar Policía Nacional<br>
**Registros:** ~ 661K filas<br>
**Cobertura temporal:** 01/01/2010 - 31/10/2025<br>

# **1. DEFINICION DEL PROBLEMA.**

## **1.1. Tipo de Problema:**

Este dataset registra cada evento reportado de violencia intrafamiliar (VIF) captado por la Policia Nacional de Colombia entre 2010 y 2025. Es un problema de **analisis descriptivo-exploratorio** con componenente de series de tiempo,orientado a:

* Identificar patrones geoespaciales (¿Donde se concentran los delitos?).

* Analizar tendencias temporales (¿Los delitos de VIF estan creciendo o reduciendose?)

* Caracterizar perfiles de victimas (genero, grupo etario).

* Evaluar la modalidad del delito (armas medios utilizados).

La VIF es un problema de seguridad ciudadana y salud publica.


## **1.2. Objetivos del Analisis:**

* Describir la evolucion anual y mensual de los delitos VIF.

* Identificar el perfil de la victima predominante (genero y grupo etario).

* Identificar los departamentos y municipios con mayor concentracion de delitos VIF (Top 5).

* Determinar los medios / armas utilizados.


## **1.3. Preguntas del Problema (Negocio):**

* ¿Cual es la distribuccion por genero?

* ¿Concentracion de delitos por departamento?

* ¿Como evolucionan los delitos por vif en el tiempo?

* ¿Cual es el top de las armas medios utilizadas?

* ¿Que grupo etario concentra la mayor victimazacion?



# **6. COMO REPRODUCIR EL ANALISIS.**

## **6.1. Clone el repositorio:**

```bash
git clone https://github.com/Su_Usuario/vif-colombia-analysis.git
cd vif-colombia-analysis
```

## **6.2. Cree el entorno virtual e instale las dependencias:**
```bash
python -m venv .venv
source .venv/bin/activate        # Ejecute esta linea si su sistema operativo es Mac o Linux
.venv\Scripts\activate           # Ejecute esta si su sistema operativo es Windows
pip install -r requirements.txt
```

## **6.3. Descargue el dataset:**
El archivo de datos no esta incluido en el repositorio por su tamaño.

Descarguelo desde el portal oficial de datos abiertos de Colombia:
🔗 [Reporte Delito Violencia Intrafamiliar — Policia Nacional](https://www.datos.gov.co/Seguridad-y-Defensa/Reporte-Delito-Violencia-Intrafamiliar-Polic-a-Nac/vuyt-mqpw/about_data)

Una vez descargado, colócalo en:

`data/raw/Reporte_Delito_Violencia_Intrafamiliar_Policía_Nacional.csv`


## **6.4. Ejecute los notebooks en el siguiente orden:**
```
notebooks/01_exploracion.ipynb
notebooks/02_limpieza.ipynb
notebooks/03_analisis.ipynb
notebooks/04_visualizaciones.ipynb
```