# PAC2 – Visualització de Dades a Catalunya

<div align="center">
  <img src="resources/logo.png" alt="Project Logo" width="200"/>
</div>

## Descripció del projecte

Aquest projecte forma part de la **PAC2 de l’assignatura de Visualització de Dades**.  
---

## Contingut

### 1. Visualitzacions principals

| Visualització | Descripció | Fitxer |
|----------------|-------------|---------|
| **Dot Density Map** | Representa les estacions de recàrrega per a vehicles elèctrics a Catalunya. Cada punt equival a una estació, mostrant la seva distribució geogràfica. | [`resources/dot_density_map.png`](docs/dot_density_map.png) |
| **Circular Dendrogram** | Representació jeràrquica circular per mostrar relacions i proximitat entre especies de eukaryotes. | [`resources/circular_dendrogram.png`](docs/circular_dendrogram.png) |
| **UpSet Plot** | Alternativa moderna als diagrames de Venn per visualitzar intersections entre conjunts en el nostre exemple tipus de vehicles implicats en accidents. | [`resources/Upset_Plot.png`](docs/Upset.png) |

---

### 2. Fitxers principals

| Directori | Contingut |
|------------|------------|
| `/data/` | Datasets utilitzats en el projecte:<br>• `Estacions_de_recàrrega_per_a_vehicle_elèctric_a_Catalunya_20251105.csv`<br>• `Accidents_de_trànsit_amb_morts_o_ferits_greus_a_Catalunya_20251106.csv`<br>• `seqs.fasta` |
| `/resources/` | Imatges de exmples de les visualitzacions i altres imatges utilitzades al md. |
| `/docs/` | Fitxers generats per l'execució i la compilació HTML i dependències. |
| `/PAC2_visualitzacions.Rmd` | Arxiu principal R Markdown amb tot el codi i anàlisi. |
| `/PAC2_visualitzacions.html` | Output HTML final per a la presentació del projecte. |

---

## Llibreries utilitzades

El projecte utilitza R i els següents paquets:

```r
library(sf)
library(ggplot2)
library(dplyr)
library(mapSpain)
library(UpSetR)       # o ComplexUpset
library(tidyverse)
library(readr)
library(stringr)
