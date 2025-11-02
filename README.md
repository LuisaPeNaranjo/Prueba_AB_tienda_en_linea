# Proyecto de Prueba A/B - Sistema de Recomendaciones

**Autor:** Luisa Peña

## Objetivo del estudio

El propósito de esta prueba A/B es evaluar el impacto de un nuevo sistema de recomendaciones en el embudo de conversión de una tienda en línea internacional:

- product_page → product_cart → purchase

Se comparan dos grupos:

- **Grupo A (control):** sin cambios en el embudo  
- **Grupo B (experimental):** con el nuevo sistema de recomendaciones

## Datos

Todos los datasets se encuentran en la carpeta `data/`:

- `ab_project_marketing_events_us.csv`: calendario de eventos de marketing  
- `final_ab_new_users_upd_us.csv`: usuarios que se registraron entre el 7 y 21 de diciembre de 2020  
- `final_ab_events_upd_us.csv`: eventos de los nuevos usuarios  
- `final_ab_participants_upd_us.csv`: participantes de la prueba A/B  

## Estructura del repositorio

`/Prueba_AB_tienda_en_linea/`
│-- `README.md`
│-- `prueba A/B.ipynb # Notebook con análisis completo`
│-- `imagenes/ # Visualizaciones generadas`
│ ├── `01_distribucion_eventos_por_grupo.png`
│ └── `02_funnel_stage_comparison.png`
│-- `data/ # Datasets originales`


## Análisis realizado

1. **Exploración de datos (EDA)**  
   - Limpieza: valores faltantes, duplicados y tipos de datos  
   - Distribución de usuarios por grupo, región y dispositivo  

2. **Evaluación del embudo de conversión**  
   - product_page → product_cart → purchase  
   - Comparación entre grupos A y B  

3. **Prueba estadística**  
   - Prueba Z para comparar proporciones de conversión  
   - Evaluación de significancia estadística (p < 0.05)  

4. **Conclusiones y recomendaciones**  
   - No se encontraron diferencias estadísticamente significativas entre los grupos A y B (p > 0.05)  
   - Recomendaciones para nuevas pruebas:  
     - Aumentar tamaño de muestra  
     - Evitar usuarios repetidos entre grupos (contaminación)  
     - Medir indicadores adicionales (tiempo de permanencia, tasa de retorno, valor promedio de compra)  
     - Complementar con análisis cualitativo (UX, encuestas)

## Visualizaciones

### Distribución de eventos por grupo
![Distribución de eventos por grupo](Prueba_AB_tienda_en_linea/imagenes/01_distribucion_eventos_por_grupo.png)

### Comparación del embudo de conversión
![Funnel Stage Comparison](Prueba_AB_tienda_en_linea/imagenes/02_funnel_stage_comparison.png)
