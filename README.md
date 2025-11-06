# PAC2 – Visualització de Dades

<div align="center">
  <img src="resources/logo.png" alt="Project Logo" width="200"/>
</div>

## Descripció del projecte

En aquesta PAC 2 es demana d'explorar **tres tècniques de visualització** diferents.
L’objectiu és entendre’n **l’origen, el funcionament, els avantatges i limitacions**, i crear una **visualització pròpia** amb dades obertes per a cadascuna.

Les tècniques assignades són:

1. Dot Density Map
2. Circular Dendrogram
3. UpSet Plot

---

## Contingut

### 1. Visualitzacions principals

| Visualització | Descripció | Fitxer |
|----------------|-------------|---------|
| **Dot Density Map** | Representa les estacions de recàrrega per a vehicles elèctrics a Catalunya. Cada punt equival a una estació, mostrant la seva distribució geogràfica. | [`docs/dot_denisty_map.png`](docs/dot_denisty_map.png) |
| **Circular Dendrogram** | Representació jeràrquica circular per mostrar relacions i proximitat entre especies de eukaryotes. | [`docs/circular_dendogram.png`](docs/circular_dendogram.png) |
| **UpSet Plot** | Alternativa moderna als diagrames de Venn per visualitzar intersections entre conjunts en el nostre exemple tipus de vehicles implicats en accidents. | [`docs/UpSet.png`](docs/UpSet.png) |

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
