# Trayectoria de la regulación de edificación en suelo residencial en el Gran Santiago, 1997 a 2024

Sitio: https://chile-zoning.github.io/

Autores: Hugo E. Silva, Kenzo Asahi y Diego Gil, Pontificia Universidad Católica de Chile.
Contacto: husilva@uc.cl.

Mapa interactivo con dos medidas del nivel de restrictividad de la regulación de edificación
urbana, por comuna y año, para 34 comunas del Gran Santiago. Las medidas sólo se aplican en
suelo que admite uso residencial.

1. **Índice de flexibilidad** (3 a 12, más alto es más flexible). Cada polígono recibe un
   puntaje de 1 a 3 en altura máxima efectiva, coeficiente de constructibilidad y densidad
   máxima según terciles comunes de 1997 a 2024, y 4 si la norma no tiene tope. El índice es
   la suma; el promedio comunal pondera por área residencial.
2. **Suelo residencial que admite edificios altos**: fracción del área residencial donde la
   altura máxima efectiva (régimen más favorable entre aislado, continuo y pareado) permite al
   menos 4, 6 o 10 pisos, o no tiene tope. Un edificio de N pisos requiere 2,5 m × N + 1,5 m
   (11,5 m para 4 pisos, 16,5 m para 6 y 26,5 m para 10). También se mide la fracción donde
   sólo se permiten casas.

Fuente: panel de normas urbanísticas de los Planes Reguladores Comunales a nivel de
polígono-año. Polígonos con normas caso a caso quedan fuera de ambas medidas.

## Archivos

- `index.html`: la página (necesita conexión para d3 y tipografías).
- `data/simple.csv`: la serie comuna-año. Columnas: `comuna`, `comuna_label`, `year`,
  `indice` (3 a 12), y las fracciones del área residencial (0 a 1) `h4`, `h6`, `h10` (admite
  4, 6 o 10 pisos), `hlibre` (altura sin tope en algún régimen) y `hcasas` (tope de 9 m o
  menos en todos los regímenes, es decir, sólo casas). `h_prom_m` es la altura máxima
  efectiva promedio en metros, ponderada por área, sólo en polígonos con tope. La fila
  `GRAN SANTIAGO` es el promedio ponderado por área.

## Cómo citar

Silva, H. E., K. Asahi y D. Gil (2026). *Trayectoria de la regulación de edificación en suelo
residencial en el Gran Santiago, 1997 a 2024*: https://chile-zoning.github.io/

Los datos se usan en: Gil, D., Silva, H. E., & Asahi, K. (2026). Wealth, homeownership, and
land use regulatory changes. *Urban Studies, 0*(0). https://doi.org/10.1177/00420980261498609.
Versión en SSRN: https://papers.ssrn.com/abstract=7586760

## Agradecimientos

Los autores agradecen a Diego Benavides, Damián Maffioletti y José Portales por su excelente
asistencia de investigación, y a Andrea Herrera, Javier Peñafiel y Camila Carrasco por sus
contribuciones en las etapas iniciales del proyecto. También agradecen el financiamiento de
ANID a través de los proyectos FONDECYT Regular 1230839 y 1262470.
