# Regulación de edificación en el Gran Santiago, 1997 a 2024

Sitio: https://chile-zoning.github.io/

Autores: Hugo E. Silva, Kenzo Asahi y Diego Gil, Pontificia Universidad Católica de Chile.
Contacto: husilva@uc.cl.

Mapa interactivo con dos medidas por comuna y año para 34 comunas del Gran Santiago:

1. **Índice de restrictividad** (3 a 12, más alto es más flexible). Cada polígono recibe un
   puntaje de 1 a 3 en altura máxima efectiva, coeficiente de constructibilidad y densidad
   máxima según terciles comunes de 1997 a 2024, y 4 si la norma no tiene tope. El índice es
   la suma; el promedio comunal pondera por área residencial.
2. **Suelo residencial que admite edificios altos**: fracción del área residencial donde la
   altura máxima efectiva (régimen más favorable entre aislado, continuo y pareado) permite al
   menos 4, 6 o 10 pisos (3,5 m por piso), o no tiene tope.

Fuente: panel de normas urbanísticas de los Planes Reguladores Comunales a nivel de
polígono-año. Polígonos con normas caso a caso quedan fuera de ambas medidas.

## Archivos

- `index.html`: la página (necesita conexión para d3 y tipografías).
- `data/simple.csv`: la serie comuna-año: `comuna`, `comuna_label`, `year`, `indice`,
  `h4`, `h6`, `h10`, `hlibre`, `hcasas` (shares 0 a 1; `hcasas` es la parte donde la altura
  máxima tiene tope de 9 m o menos, es decir, solo casas), `h_prom_m` (altura máxima promedio en metros,
  solo polígonos con tope). `GRAN SANTIAGO` es el promedio ponderado por área.

## Cómo citar

Silva, H. E., K. Asahi y D. Gil (2026). *Regulación de edificación en el Gran Santiago, 1997 a
2024* [datos y sitio web]. https://chile-zoning.github.io/

Los datos se usan en: Gil, D., H. E. Silva y K. Asahi. "Wealth, Homeownership, and Land Use
Regulatory Changes". *Urban Studies*, en prensa.
SSRN: https://papers.ssrn.com/abstract=7586760

## Agradecimientos

Los autores agradecen a Diego Benavides, Damián Maffioletti y José Portales por su excelente
asistencia de investigación, y a Andrea Herrera, Javier Peñafiel y Camila Carrasco por sus
contribuciones en las etapas iniciales del proyecto. También agradecen el financiamiento de
ANID a través de los proyectos FONDECYT Regular 1230839 y 1262470.
