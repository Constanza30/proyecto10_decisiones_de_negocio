# 📊 Proyecto 10. Priorización de Hipótesis y Test A/B

En el presente repositorio una tienda online busca incrementar sus ingresos.  Se realizó un análisis para presentarle al equipo de marketing, se definieron varias hipótesis y se ejecutó una **prueba A/B** para evaluar su impacto en métricas clave como conversión e ingresos.

---

## 🎯 Objetivo
- Priorizar hipótesis de negocio usando ICE y RICE.
- Analizar los resultados de una prueba A/B.
- Determinar si los cambios implementados generan mejoras estadísticamente significativas.

---

## 🔹 Parte 1 – Priorización de hipótesis
Se evaluaron 9 hipótesis utilizando los frameworks **ICE** y **RICE**.

**Hallazgos clave:**
- ICE prioriza impacto y confianza
- RICE incorpora el alcance, cambiando el orden de prioridad
- Las hipótesis mejor posicionadas se relacionan con:
  - Formularios de suscripción
  - Nuevos canales de adquisición
  - Recomendaciones de productos

📌 Estas hipótesis fueron la base para la prueba A/B.

---

## 🔹 Parte 2 – Análisis del Test A/B

### 📈 Ingresos acumulados
- El Grupo B superó consistentemente al Grupo A
- A partir de la mitad del experimento, la diferencia se vuelve clara y sostenida

### 🛒 Tamaño promedio del pedido
- Inicialmente parecía mayor en el Grupo B
- Tras eliminar valores atípicos, no se detectó una diferencia significativa

### 🔄 Tasa de conversión
- El Grupo B mostró una mejora consistente
- Conversión +17.07% tras filtrar usuarios anómalos
- Diferencia estadísticamente significativa (p < 0.05)

---

## 🚨 Manejo de valores atípicos
Se identificaron usuarios anómalos mediante:
- Percentiles 95 y 99
- Usuarios con: más de 2 pedidos, pedidos superiores a 435 USD

El filtrado permitió obtener conclusiones más confiables.

---

## 📊 Pruebas estadísticas
- Conversión: diferencia significativa a favor del Grupo B  
- Tamaño de pedido: no significativa, antes ni después del filtrado

---

## ✅ Conclusión final
📌 Decisión: Parar la prueba y declarar al Grupo B como líder

**Justificación:**
- Mejora clara y estadísticamente significativa en la conversión
- El tamaño promedio del pedido no se ve afectado negativamente
- Implementar los cambios del Grupo B es beneficioso para el negocio

---

## 🛠️ Herramientas y tecnologías
- Python. (Pandas, NumPy, SciPy)
- Visualización. Matplotlib, Seaborn
- Estadística. Mann-Whitney U Test
- Metodología. ICE, RICE, A/B Testing
