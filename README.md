# Confusión vs Interacción en Epidemiología

## Descripción

Este proyecto ilustra mediante ejemplos simulados y visualizaciones la diferencia entre dos conceptos fundamentales en epidemiología y análisis estadístico:

- **Variable de Confusión**: Una tercera variable que afecta tanto a la exposición como al resultado, creando una asociación espuria entre ellas.
- **Variable de Interacción (Modificador de Efecto)**: Una variable que modifica la magnitud del efecto de la exposición sobre el resultado.

## 📊 Ejemplos Incluidos

### 1. Variable de Confusión
**Escenario**: Relación entre consumo de café y riesgo cardiovascular
- **Exposición**: Consumo de café
- **Resultado**: Riesgo cardiovascular
- **Confusor**: Tabaquismo

El ejemplo muestra cómo el tabaquismo puede crear una relación aparente positiva entre café y riesgo cardiovascular cuando, en realidad, la relación es negativa una vez ajustada por el confusor.

### 2. Variable de Interacción
**Escenario**: Efecto de un fármaco antihipertensivo según sexo
- **Exposición**: Dosis del fármaco
- **Resultado**: Reducción de presión arterial
- **Modificador**: Sexo biológico

El ejemplo ilustra cómo el efecto del fármaco (pendiente) varía según el sexo del paciente, demostrando una interacción estadística.

## 🔧 Requisitos

```r
library(ggplot2)
library(dplyr)
library(gridExtra)
```

## 📦 Instalación de Dependencias

```r
install.packages(c("ggplot2", "dplyr", "gridExtra"))
```

## 🚀 Uso

1. Abre el archivo `confusion_e_interaccion.Rmd` en RStudio
2. Ejecuta todos los chunks de código (Ctrl/Cmd + Alt + R)
3. O genera el documento HTML/PDF usando el botón "Knit"

## 📈 Resultados

El código genera dos gráficos comparativos:

- **Gráfico de Confusión**: Muestra la línea punteada (relación espuria sin ajustar) vs. líneas sólidas estratificadas por fumador/no fumador
- **Gráfico de Interacción**: Muestra diferentes pendientes para hombres y mujeres, indicando modificación del efecto

## 👨‍💻 Autor

Jesús F García Gavilán

## 📄 Licencia

Este proyecto es de código abierto y está disponible para fines educativos.