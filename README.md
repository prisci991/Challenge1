# 📊 Challenge 1 - Modelado de Datos con Python  

Este proyecto forma parte del **Challenge de Data Science de Alura Latam**, cuyo objetivo es analizar el rendimiento de 4 tiendas mediante técnicas de análisis y visualización de datos.  

Se procesan y visualizan métricas clave como facturación, ventas por categoría, calificaciones promedio, productos más vendidos y costos de envío, además de mapas de calor de ubicación geográfica de ventas.  

---

## 📂 Contenido del Proyecto  
El Jupyter Notebook contiene:  

1. **Importación de datos** desde archivos `.csv` alojados en GitHub.  
2. **Análisis exploratorio** de facturación, categorías y calificaciones.  
3. **Identificación de productos más y menos vendidos**.  
4. **Cálculo de costos de envío promedio**.  
5. **Visualizaciones con Matplotlib** (barras, tortas, horizontales).  
6. **Mapas de calor con Folium** para geolocalización de ventas.  
7. **Informe final** con conclusiones y recomendación de la mejor tienda para vender.  

---

## ⚙️ Ejecución en Google Colab  

### 1️⃣ Abrir el notebook en Colab  
- Ve a [Google Colab](https://colab.research.google.com/).  
- Cargar el archivo:
```bash
Challenge1_Modelado_de_datos_con_Pyhton.ipynb
```

### 2️⃣ Instalar dependencias necesarias  
En una celda de Colab ejecuta:  
```python
!pip install pandas matplotlib numpy folium
```
### 3️⃣ Ejecutar las celdas en orden

* Los datasets se cargan directamente desde GitHub mediante pandas.read_csv(), por lo que no necesitas subir archivos manualmente.

* Al llegar a las celdas de visualización de mapas (folium), se generarán mapas interactivos que podrás explorar directamente en Colab.

### 📦 Dependencias

* pandas → Manipulación y análisis de datos.

* numpy → Cálculos numéricos.

* matplotlib → Gráficos y visualizaciones.

* folium → Mapas interactivos y mapas de calor.

## 🛠️ Posibles Problemas y Soluciones  

| Problema | Causa | Solución |
|----------|-------|----------|
| ❌ Error al cargar archivos CSV | URLs externas cambiaron o conexión a internet inestable | Revisar que las URLs de los CSV de GitHub estén activas |
| ❌ `ModuleNotFoundError` | Librerías no instaladas en Colab | Ejecutar `!pip install pandas matplotlib numpy folium` |
| ❌ Mapas no se muestran en Colab | Limitación temporal de renderizado | Usar `m.save("mapa.html")` y descargar el archivo para abrirlo en el navegador |
| ❌ Error con acentos/encoding | Configuración de UTF-8 en algunos sistemas | Usar `pd.read_csv(url, encoding="utf-8")` |

## ✅ Conclusión

Este proyecto permite practicar modelado y análisis de datos con Python, aplicando visualizaciones gráficas y mapas interactivos para tomar decisiones basadas en datos.

La recomendación final del análisis es que la Tienda 1 es la más rentable para vender, gracias a su alto ingreso total y buen desempeño general.
