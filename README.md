# Modulo 3 - TyHM II

# Contenido de la Actividad : Monitoreo y Comparativa de Cobertura Nival con QGIS
## Descripción del Proyecto
Evaluación espacio-temporal y cuantificación de la variación de superficie cubierta por nieve en el sector centro-sur de la cordillera de los Andes (con foco en el Valle de las Lágrimas), comparando el ciclo hidrológico de noviembre 2024 frente a noviembre 2026.

## Metodología Aplicada
1. Adquisición y Procesamiento Espectral: Descarga de imágenes satelitales multiespectrales Sentinel-2 (L2A) correspondientes a ambos períodos temporales. Empleo del Índice de Nieve de Diferencia Normalizada (NDSI) mediante la Calculadora Ráster para la discriminación precisa entre cobertura nival, roca desnuda y nubosidad.
2. Ajuste Cartográfico Métrico: Reproyección y fijación del Sistema de Referencia de Coordenadas métrico proyectado UTM Zona 19S (EPSG:32719) para garantizar la exactitud métrica en el cálculo de áreas y evitar distorsiones angulares.
3. Binarización y Vectorización: Segmentación espectral y conversión ráster a vectorial (poligonización) para aislar las masas de nieve efectivas, aplicando depuración de artefactos marginales de barrido orbital (NoData).
4. Cuantificación de Superficies: Cálculo matemático en la tabla de atributos mediante sintaxis espacial ($area / 10000) para obtener la superficie consolidada en hectáreas (ha).
## Resultados y Balance Interanual
Superficie nival (Noviembre 2024): 641.940 ha
Superficie nival (Noviembre 2026): 1.190.260 ha
Variación neta absoluta: +548.320 ha
Variación relativa interanual: +85,42%

Interpretación técnica: Los resultados evidencian una marcada recuperación nival interanual (+85,42%), pasando de un régimen con fuerte déficit en 2024 a un período de acumulación sustancial en 2026, lo que impacta de forma directa en el pronóstico de derrame hídrico y turnos de riego para las cuencas de los ríos Diamante y Atuel.

🌐 Mapa Web Interactivo: Puedes explorar el visor geográfico interactivo con conmutación de capas y mapa satelital en el siguiente enlace: 👉 Ver Mapa Interactivo de Cobertura Nival en GitHub Pages
