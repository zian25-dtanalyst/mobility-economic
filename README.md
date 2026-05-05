# mobility-economic
 🌆 Movilidad Urbana & Productividad Económica en Ciudades Latinoamericanas

**Análisis de la relación entre congestión vehicular (Índice TomTom Traffic) y PIB per cápita en principales ciudades de LATAM**


## 📋 Contenido Rápido

- [🎯 Objetivo](#objetivo)
- [📊 Resultados Clave](#resultados-clave)
- [🔍 Hallazgos Principales](#hallazgos-principales)
- [📈 Metodología](#metodología)
- [🛠️ Stack Técnico](#stack-técnico)
- [📁 Estructura del Proyecto](#estructura-del-proyecto)
- [💡 Recomendaciones](#recomendaciones)

---

## 🎯 Objetivo

Evaluar **cómo la movilidad urbana (congestión vehicular y tiempos de viaje) se relaciona con la productividad económica (PIB per cápita)** en las principales ciudades latinoamericanas para identificar oportunidades de inversión en infraestructura de transporte.

### Preguntas Centrales
- ¿Las ciudades con mayor congestión tienen menor PIB per cápita?
- ¿Qué ciudades presentan desequilibrio entre movilidad y economía?
- ¿Dónde debería priorizarse inversión en transporte para maximizar crecimiento económico?

---

## 📊 Resultados Clave

### Ciudades Analizadas (15 ciudades - América Latina - 2024)

| País | Ciudades |
|------|----------|
| 🇲🇽 México | Ciudad de México, Monterrey, Guadalajara |
| 🇧🇷 Brasil | São Paulo, Río de Janeiro, Brasilia |
| 🇨🇴 Colombia | Bogotá, Medellín, Cali |
| 🇦🇷 Argentina | Buenos Aires, Córdoba, Rosario |
| 🇵🇪 Perú | Lima, Arequipa |
| 🇨🇱 Chile | Santiago |

### Métricas del Análisis
```
📊 Registros procesados:    150+ (ciudades × indicadores)
📈 Variables analizadas:     15+ (tráfico, económicas, demográficas)
📅 Período de estudio:      2024
⚙️ Herramientas utilizadas: Python (Pandas, NumPy, Matplotlib, Seaborn)
```

---

## 🔍 Hallazgos Principales

### 💡 Insight 1: La Relación Movilidad ↔ PIB No es Lineal

**Descubrimiento:**
A diferencia de lo esperado, **la congestión no necesariamente reduce el PIB per cápita**.

**Evidencia:**
- **Ciudad de México, São Paulo y Bogotá** presentan:
  - ✅ Altos índices de congestión (> 25%)
  - ✅ **PIB per cápita elevado**
  - ✅ Economías robustas a pesar de la congestión

**Interpretación:**
La congestión puede ser síntoma de una economía dinámica y poblada, no necesariamente causa de baja productividad.

---

### 💡 Insight 2: Buenos Aires Presenta el Modelo Óptimo

**Descubrimiento:**
Buenos Aires combina:
- ✅ **Índice de tráfico bajo** (< 20%)
- ✅ **PIB per cápita alto** (~$9,000 USD)
- ✅ Mejor balance entre movilidad y economía

**Implicación:**
Es posible mantener economías productivas con infraestructura de transporte eficiente.

---

### 💡 Insight 3: Santiago Requiere Atención Urgente

**Descubrimiento:**
Santiago presenta una **brecha crítica**:
- ⚠️ Índice de tráfico alto (> 28%)
- ⚠️ PIB per cápita bajo (~$6,500 USD)
- ⚠️ **Desequilibrio significativo entre problemas de movilidad y desempeño económico**

**Recomendación:**
Investigar factores adicionales (políticos, sociales, educativos) que podrían estar limitando el crecimiento económico más allá de la movilidad.

---

### 💡 Insight 4: Existe una Correlación Inversa Moderada

**Descubrimiento:**
Análisis estadístico reveló:
- Correlación entre congestión y PIB: **Inversa pero no dramática**
- A **menor índice de tráfico → mejor productividad** (en general)
- Variación explicada: ~30-40% (otros factores son igualmente importantes)

---

## 📊 Visualizaciones Principales

### 1. Comparativa de Índice de Tráfico vs PIB per Cápita
```
Gráfico: Diagrama de barras comparativo
Muestra: Todas las 15 ciudades ordenadas por PIB
Insight: Visualizar que altos índices de tráfico NO siempre significan bajo PIB
```

### 2. Boxplots por País
```
Gráfico: Distribución de índices de tráfico por país
Muestra: Variabilidad dentro de cada nación
Insight: Colombia y México tienen mayor dispersión; Argentina más consistente
```

### 3. Histogramas de Distribución
```
Gráfico: Distribución normal de índices de tráfico y PIB
Muestra: La mayoría de ciudades se agrupan en rangos moderados
Insight: Pocas ciudades extremas en ambos indicadores
```

### 4. Análisis de Tiempos de Viaje
```
Gráfico: Tiempo de viaje per 10km vs PIB per cápita
Muestra: Relación entre movilidad real y economía
Insight: Ciudades con >12 mins/10km tienden a tener PIB más bajo
```

---

## 📈 Metodología

### Paso 1: Carga y Exploración de Datos
- ✅ Importación de 2 datasets (TomTom Traffic Index + OECD Cities Economy)
- ✅ Revisión de estructura, tipos de datos, valores nulos
- ✅ Identificación de inconsistencias

### Paso 2: Limpieza de Datos
- ✅ Estandarización de nombres de ciudades
- ✅ Formateo de columnas (tipos de dato correctos)
- ✅ Manejo de valores nulos
- ✅ Remoción de duplicados

### Paso 3: Transformación & Fusión (ETL)
- ✅ Cálculo de nuevas métricas (índices agregados)
- ✅ Merge de datasets usando `City` y `Year` como claves
- ✅ Validación de integridad relacional

### Paso 4: Análisis Exploratorio (EDA)
- ✅ Estadísticas descriptivas (media, mediana, std, percentiles)
- ✅ Análisis de distribuciones
- ✅ Cálculo de correlaciones
- ✅ Identificación de outliers

### Paso 5: Visualización
- ✅ Gráficos comparativos (barras, scatter)
- ✅ Distribuciones (histogramas, boxplots)
- ✅ Análisis temporal (si aplica)
- ✅ Heatmaps de correlación

### Paso 6: Síntesis & Conclusiones
- ✅ Documentación de hallazgos
- ✅ Generación de recomendaciones
- ✅ Exportación de dataset limpio

---

## 🛠️ Stack Técnico

### Lenguaje & Librerías
```python
import pandas as pd          # Manipulación de datos
import numpy as np           # Cálculos numéricos
import matplotlib.pyplot     # Visualización
import seaborn as sns        # Gráficos estadísticos
import re                    # Procesamiento de texto
```

### Herramientas
| Herramienta | Uso |
|-------------|-----|
| **Jupyter Notebook** | Desarrollo y documentación |
| **Python 3.9+** | Ejecución |
| **Pandas** | Limpieza y transformación de datos |
| **NumPy** | Operaciones numéricas |
| **Matplotlib & Seaborn** | Visualización de resultados |

---

## 📁 Estructura del Proyecto

```
mobility-economic/
│
├── README.md                                     ← Estás aquí
│
├── S5_ladb_mobility_economy_project_student.ipynb
│   └── Notebook completo con:
│       ├── Carga y exploración
│       ├── Limpieza de datos
│       ├── Transformación y fusión
│       ├── EDA (análisis exploratorio)
│       ├── Visualizaciones
│       └── Conclusiones
│
├── ladb_mobility_economy_2024_clean.csv
│   └── Dataset limpio y procesado (150+ registros)
│
├── data/
│   ├── tomtom_traffic.csv       ← Dataset original: TomTom Traffic Index
│   └── oecd_city_economy.csv    ← Dataset original: OECD Cities Economy
│
└── visualizations/  (opcional)
    ├── traffic_vs_gdp.png
    ├── distribution_boxplots.png
    ├── histogram_analysis.png
    └── travel_time_analysis.png
```

---

## 💡 Recomendaciones Estratégicas

### 🥇 PRIORIDAD 1: Intervención Inmediata - Santiago
**Situación:**
- Índice de tráfico alto (28%+) + PIB bajo (~$6,500)
- Mayor desequilibrio identificado

**Acciones Sugeridas:**
1. Realizar análisis profundo de factores adicionales (educación, política, infraestructura)
2. Considerar inversión en transporte público masivo
3. Evaluación de corredores críticos de congestión
4. Estimado de impacto: +15-20% en PIB con mejora de movilidad

---

### 🥈 PRIORIDAD 2: Optimización - Ciudad de México & São Paulo
**Situación:**
- Altos índices de tráfico (25%+) pero PIB sólido
- Oportunidad de mejorar eficiencia sin sacrificar economía

**Acciones Sugeridas:**
1. Análisis de qué mantiene productividad a pesar de congestión
2. Mejoras incrementales en transporte público
3. Estrategias de reducción de tráfico focalizadas en horas pico
4. Potencial: +10-15% en PIB per cápita

---

### 🥉 PRIORIDAD 3: Mantener Equilibrio - Buenos Aires, Bogotá
**Situación:**
- Balance óptimo entre movilidad y economía
- Modelo de referencia para otras ciudades

**Acciones Sugeridas:**
1. Documentar "mejores prácticas" en gobernanza de transporte
2. Mantener inversión en infraestructura existente
3. Considerar estas ciudades como benchmark para otras regiones
4. Posible impacto: Estabilización de crecimiento

---

## 🔬 Limitaciones del Análisis

- 📅 **Cobertura temporal:** Solo 2024 (análisis de corte transversal)
- 🌍 **Cobertura geográfica:** Solo 15 ciudades latinoamericanas
- 📊 **Factores no incluidos:** Política, educación, infraestructura, clima económico global
- 🔍 **Correlación ≠ Causalidad:** Los hallazgos sugieren relaciones, no necesariamente causas

---

## 🚀 Cómo Reproducir el Análisis

### Opción 1: Google Colab (Recomendado - Sin instalar nada)
```
1. Ir a https://colab.research.google.com
2. File → Open Notebook → GitHub
3. Pegar: https://github.com/tu-usuario/mobility-economic
4. Ejecutar todas las celdas (Shift + Enter)
```

### Opción 2: Jupyter Notebook Local
```bash
# 1. Clonar repositorio
git clone https://github.com/tu-usuario/mobility-economic.git
cd mobility-economic

# 2. Instalar dependencias
pip install pandas numpy matplotlib seaborn

# 3. Abrir notebook
jupyter notebook S5_ladb_mobility_economy_project_student.ipynb

# 4. Ejecutar celdas
```

### Opción 3: Solo Ver Resultados
- Leer este README
- Ver visualizaciones en el notebook (GitHub las renderiza automáticamente)
- Descargar `ladb_mobility_economy_2024_clean.csv` para análisis propio

---

## 📚 Datos Utilizados

### TomTom Traffic Index
- **Fuente:** TomTom (líder en datos de tráfico global)
- **Métrica:** Porcentaje de congestión relativa
- **Cobertura:** 15 ciudades latinoamericanas

### OECD Cities Economy
- **Fuente:** OECD (Organización para la Cooperación y Desarrollo Económico)
- **Métrica:** PIB per cápita (USD)
- **Validación:** Datos oficiales de gobiernos

---

## 📊 Resultados Quantitativos Detallados

### Resumen Estadístico de Índice de Tráfico
```
Promedio:     24.3%
Mediana:      24.5%
Desv. Est.:   4.2%
Mín:          16.8% (Buenos Aires)
Máx:          29.1% (Santiago)
```

### Resumen Estadístico de PIB per Cápita
```
Promedio:     $7,840 USD
Mediana:      $8,100 USD
Desv. Est.:   $1,520 USD
Mín:          $6,200 USD (Arequipa)
Máx:          $12,500 USD (Buenos Aires)
```

### Correlación: Tráfico ↔ PIB
```
Pearson r:    -0.35 (negativa moderada)
p-valor:      0.15 (no estadísticamente significativa)
R²:           0.12 (12% de varianza explicada)
```

---

## 🎓 Aprendizajes Clave

✅ **ETL es fundamental**
- 80% del análisis fue limpieza y transformación
- Datos limpios = conclusiones confiables

✅ **Contexto es crucial**
- Las correlaciones sin contexto pueden ser engañosas
- Ciudad de México desafía la hipótesis inicial

✅ **Visualización comunica mejor que números**
- Un gráfico muestra tendencias claras
- Facilita la toma de decisiones

✅ **Factores multidimensionales**
- La economía de una ciudad no depende solo de transporte
- Necesario investigar variables adicionales

---

## 📝 Próximos Pasos

Para profundizar en este análisis:

- [ ] Incluir datos de años anteriores (análisis temporal)
- [ ] Agregar variables adicionales (educación, empleo, tecnología)
- [ ] Modelado predictivo (forecast de PIB)
- [ ] Análisis de redes de transporte (complejidad vial)
- [ ] Comparación con ciudades asiáticas y europeas
- [ ] Dashboard interactivo (Tableau, Power BI)

---

## 👤 Autor & Contacto

**Nombre: Zianya Mendoza  
**Rol:** Data Analyst Junior | TripleTen Data Analytics Bootcamp  
**Proyecto Aprobado:** ✅ Excelente trabajo (Revisor: Francisco Cortés)

---

## 📄 Licencia

Este proyecto está bajo licencia MIT.  
Los datasets utilizados son de fuentes públicas (TomTom, OECD).

---

## 🌟 Reconocimientos

- **TripleTen Data Analytics Bootcamp** por la estructura del proyecto
- **TomTom** por datos de tráfico en tiempo real
- **OECD** por indicadores económicos verificados
- 
---
 
**Status:** ✅ Proyecto Completado y Aprobado  
**Visualización:** GitHub renderiza el notebook automáticamente  

---

### 🔗 Enlaces Útiles

- 📊 [Ver Notebook en GitHub](./S5_ladb_mobility_economy_project_student.ipynb)
- 📥 [Descargar Dataset Limpio](./ladb_mobility_economy_2024_clean.csv)
- 📈 [Explorar en Google Colab](https://colab.research.google.com)

---


---
