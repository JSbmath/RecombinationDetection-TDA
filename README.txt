# Identification of Recombination in Viruses using Topological Data Analysis / Identificación de Recombinación en Virus Utilizando Análisis Topológico de Datos

This repository contains the code, data references, results, and documentation for the Master's thesis titled "Identification of Recombination in Viruses using Topological Data Analysis" by Jaime Salvador López Viveros, completed at the Joint Graduate Program in Mathematical Sciences UNAM-UMSNH under the supervision of Dra. Nelly Sélem Mojica.

The main objective of this work is to identify horizontal gene transfer events (recombination and reassortment) in viral genomes (specifically Influenza H7N9 and SARS-CoV-2) using Topological Data Analysis (TDA), particularly persistent homology. The project involved implementing the methodology, validating it with known cases (like the H7N9 triple reassortment), evaluating its robustness, and developing computational tools for visualizing topological features.

---

Este repositorio contiene el código, referencias de datos, resultados y documentación de la tesis de Maestría titulada "Identificación de Recombinación en Virus Utilizando Análisis Topológico de Datos" por Jaime Salvador López Viveros, realizada en el Posgrado Conjunto en Ciencias Matemáticas UNAM-UMSNH bajo la tutoría de la Dra. Nelly Sélem Mojica.

El objetivo principal de este trabajo es identificar eventos de transferencia genética horizontal (recombinación y reordenamiento) en genomas virales (específicamente Influenza H7N9 y SARS-CoV-2) mediante el Análisis Topológico de Datos (TDA), particularmente la homología persistente. El proyecto incluyó la implementación de la metodología, su validación con casos conocidos (como el reordenamiento triple en H7N9), la evaluación de su robustez y el desarrollo de herramientas computacionales para la visualización de características topológicas.

---

## Interactive 3D Visualization / Visualización Interactiva 3D

An online interactive version of the TDA process visualization is available here:
**[https://tda-reordenamiento-triple-h7n9.streamlit.app/](https://tda-reordenamiento-triple-h7n9.streamlit.app/)**

This tool implements a 3D visualization of simplicial complexes derived from genetic distance matrices of viral sequences. It replicates the validation experiment for the H7N9 triple reassortment (Section 5.1.1), where a distance matrix of six concatenated sequences reveals a 1-hole and a 2-hole, indicative of reassortment among H9N2, H7N9, and H7N3 strains. You can adjust the filtration value to explore how topological features evolve, reflecting the formation and collapse of cycles and cavities that signal evolutionary events.

---

Una versión interactiva en línea de la visualización del proceso de TDA se encuentra disponible aquí:
**[https://tda-reordenamiento-triple-h7n9.streamlit.app/](https://tda-reordenamiento-triple-h7n9.streamlit.app/)**

Esta herramienta implementa una visualización 3D de complejos simpliciales derivados de matrices de distancia genética de secuencias virales. Replica el experimento de validación para el reordenamiento triple de H7N9 (Sección 5.1.1), donde una matriz de distancia de seis secuencias concatenadas revela un hueco de dimensión 1 y un hueco de dimensión 2, indicativos de reordenamiento entre las cepas H9N2, H7N9 y H7N3. Puedes ajustar el valor de filtración para explorar cómo evolucionan las características topológicas, reflejando la formación y el colapso de ciclos y cavidades que señalan eventos evolutivos.

---

## Repository Structure / Estructura del Repositorio

The repository is organized as follows:

* `/Experimentos de validacion/`: Contains validation experiments, including negative controls, sample size variation tests, and controlled simulations.
* `/H7N9 Reordenamiento Triple/`: Contains the main case study analysis for H7N9, including specific scripts, results, genomic data references, and the main interactive visualization notebook.
* `/XBB.1 SarsCov2/`: Contains the analysis of recombination in SARS-CoV-2.
* `README.md`: This file.
* `Identificación de recombinación en virus utilizando Análisis Topológico de datos.pdf`: The full thesis document.

---

El repositorio está organizado de la siguiente manera:

* `/Experimentos de validacion/`: Contiene los experimentos de validación, incluyendo controles negativos, pruebas de variación de tamaño muestral y simulaciones controladas.
* `/H7N9 Reordenamiento Triple/`: Contiene el análisis del caso de estudio principal para H7N9, incluyendo scripts específicos, resultados, referencias de datos genómicos y el notebook principal de visualización interactiva.
* `/XBB.1 SarsCov2/`: Contiene el análisis de recombinación en SARS-CoV-2.
* `README.md`: Este archivo.
* `Identificación de recombinación en virus utilizando Análisis Topológico de datos.pdf`: El documento completo de la tesis.

---

## Usage / Uso

Navigate to the specific experiment directories (e.g., `/H7N9 Reordenamiento Triple/Visualizacion/`) to find Jupyter notebooks or scripts. The notebooks, especially the main visualization notebook for H7N9, provide examples of how the analysis pipeline is executed, from data loading and distance matrix calculation (using Hamming distance, ignoring gaps and 'N's) to persistent homology computation and visualization (persistence diagrams, barcodes, heatmaps, 3D simplicial complexes).

Data was sourced from NCBI Virus Database and GISAID. Due to data sharing policies (especially for GISAID), raw sequence data may not be included directly in this repository. Please refer to the accession numbers or identifiers provided in the thesis or code to retrieve the data from the original sources. Sequence alignment was performed using tools like Clustal Omega and Nextclade.

---

Navega a los directorios de experimentos específicos (p. ej., `/H7N9 Reordenamiento Triple/Visualizacion/`) para encontrar los notebooks Jupyter o scripts. Los notebooks, especialmente el notebook principal de visualización para H7N9, proporcionan ejemplos de cómo se ejecuta el pipeline de análisis, desde la carga de datos y el cálculo de la matriz de distancias (usando la distancia de Hamming, ignorando gaps y 'N's) hasta el cómputo de la homología persistente y la visualización (diagramas de persistencia, códigos de barras, mapas de calor, complejos simpliciales 3D).

Los datos se obtuvieron de NCBI Virus Database y GISAID. Debido a las políticas de compartición de datos (especialmente para GISAID), los datos de secuencias crudas pueden no estar incluidos directamente en este repositorio. Por favor, consulta los números de acceso o identificadores proporcionados en la tesis o el código para obtener los datos de las fuentes originales. El alineamiento de secuencias se realizó utilizando herramientas como Clustal Omega y Nextclade.

---

## Citation / Cita

If you use the code or findings from this repository in your work, please cite the original thesis:

López Viveros, Jaime Salvador. (2025). *Identificación de Recombinación en Virus Utilizando Análisis Topológico de Datos*. Master's Thesis, Posgrado Conjunto en Ciencias Matemáticas UNAM-UMSNH, Morelia, Michoacán.

---

Si utilizas el código o los hallazgos de este repositorio en tu trabajo, por favor cita la tesis original:

López Viveros, Jaime Salvador. (2025). *Identificación de Recombinación en Virus Utilizando Análisis Topológico de Datos*. Tesis de Maestría, Posgrado Conjunto en Ciencias Matemáticas UNAM-UMSNH, Morelia, Michoacán.
