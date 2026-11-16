# GeoSeguridad AMB - Matemáticas Discretas (MAT 4021)
**Universidad del Norte** | **Profesor:** MSc. Iván Gómez

## Integrantes
* Santiago Coley
* Ivan Rocha
* Isaac Curiel
* Stephf Castro
* Juan Ramirez

## Descripción del Proyecto
GeoSeguridad AMB es un sistema de optimización de rutas basado en Teoría de Grafos y Álgebra Booleana. Calcula la ruta más segura entre dos puntos del Área Metropolitana de Barranquilla evaluando variables como la tasa de hurtos sectorizada y el déficit de iluminación fotométrica (¬L), utilizando el algoritmo de Dijkstra con ponderación convexa.

## Cómo ejecutar el proyecto (Reproducibilidad)
El proyecto fue diseñado bajo una arquitectura *Offline-First* y no requiere instalación de dependencias, servidores locales ni bases de datos externas.

1. Descargue el archivo principal `GeoSeguridad_AMB_MAT4021_v6.html` de este repositorio.
2. Haga doble clic sobre el archivo para abrirlo en cualquier navegador web moderno (Google Chrome, Firefox, Edge, Safari).
3. **No requiere API Keys:** La cartografía de OpenStreetMap y el motor de enrutamiento topológico están embebidos y se renderizan nativamente en el navegador.

## Casos de Prueba (Validación)
Para validar la optimalidad del algoritmo según los requisitos del curso, el sistema incluye casos preconfigurados. 
* Abra el panel derecho "Rutas (A → B)".
* Seleccione en el modal de pruebas el **Caso 1: Portal Prado → Uninorte**.
* Podrá comparar métricas exactas (distancia, tiempo, exposición a hurtos y tramos oscuros) entre la ruta rápida (Google Maps, α=1) y la ruta segura (Dijkstra, α=0.25).
