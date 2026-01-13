Risk-Analysis-Dashboard

===

\## 🚀 Descripción del Proyecto

El dashboard integra dos fuentes de datos críticas:

1\. \*\*Reporte CENDEU:\*\* Datos del Banco Central sobre la situación crediticia de deudores en múltiples bancos (A, B y C).

2\. \*\*Registro de Transferencias:\*\* Datos internos de movimientos de efectivo entre deudores.



A través de \*\*R y la librería `visNetwork`\*\*, el sistema procesa estos datos para generar un grafo de red dirigido donde los nodos son los deudores y las aristas representan tanto deudas bancarias como flujos de capital.



\## 🛠️ Tecnologías Utilizadas

\* \*\*Lenguaje:\*\* R

\* \*\*Librerías principales:\*\* \* `tidyverse` (Manipulación de datos)

&nbsp;   \* `visNetwork` (Visualización de grafos interactivos)

&nbsp;   \* `janitor` (Limpieza de datos)

&nbsp;   \* `htmlwidgets` (Exportación a Dashboard web)



\## 📈 Características Principales

\- \*\*Topología Radial Inversa:\*\* Los bancos se ubican en el núcleo central como "anclas", permitiendo ver cómo gravitan los deudores a su alrededor.

\- \*\*Consolidación de Flujos:\*\* Las transferencias entre los mismos deudores se suman automáticamente, ajustando el grosor de las flechas según el volumen transaccionado.

\- \*\*Semaforización de Riesgo:\*\* Los nodos cambian de color automáticamente según la peor situación crediticia informada en el sistema (Verde: Situación 1-2, Rojo: Situación 3+).

\- \*\*Reporte Ejecutivo:\*\* El archivo HTML incluye una tabla automática con el Top 5 de deudores por exposición total.



\## 📂 Estructura del Repositorio

\* `script\_analisis.R`: Código fuente completo y comentado.

\* `index.html`: Dashboard interactivo (Portfolio demo).

\* `data/`: (Opcional) Archivos de ejemplo con datos anonimizados.



\## 💡 Insights de Negocio

Este análisis permite a un oficial de riesgo detectar:

\* \*\*Efecto Contagio:\*\* Deudores que están al día en nuestro banco pero en default en la competencia.

\* \*\*Concentración:\*\* Grupos de deudores que se transfieren fondos entre sí para cubrir obligaciones.



---

\*Desarrollado como parte de un proyecto de análisis de riesgo crediticio avanzado.\*



