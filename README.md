
# Cytoskeleton and Cell Morphology Analysis (BBBC018)

Karp Chapter 9: The Cytoskeleton and Cell Motility

**Student ID:** 202400718  
**Dataset:** BBBC018 – Human HT29 Colon-Cancer Cells  
**Selected Phenotype:** Angular cell edges  
**Image ID:** 13571  
**Actin Filename:** 13571-actin.DIB


## Introduction ##

The cytoskeleton plays an important role in maintaining cell shape, providing structural support, and allowing cells to change their morphology. In this activity, fluorescence images of HT29 human colon-cancer cells from the BBBC018 dataset were examined to observe F-actin distribution and cell shape.

The selected phenotype was Angular cell edges. Five cells were measured using Fiji, and their measurements were analyzed in RStudio to compare cell area, circularity, aspect ratio, and mean actin fluorescence intensity.

---

## Dataset and Selected Images ##

The fluorescence images were obtained from the Broad Bioimage Benchmark Collection (BBBC018).

- Dataset: BBBC018
- Phenotype: Angular cell edges
- Image ID: 13571
- Actin filename: 13571-actin.DIB

The actin channel was used to examine F-actin staining and identify cell boundaries. F-actin is part of the cytoskeleton and contributes to cell shape, mechanical support, and cellular movement.

---

## Methods ##

### Fiji Analysis 

- The actin fluorescence image `13571-actin.DIB` was opened in Fiji using Bio-Formats.
- The cell outlines were examined, and five cells were selected for measurement.
- Area, Mean gray value, Shape descriptors, and Display label were enabled under Set Measurements.
- The Freehand Selection tool was used to trace each selected cell, and the selections were added to ROI Manager.
- All five cells were measured, and the measurements were saved as `data/fiji_results.csv`.
- The annotated fluorescence image showing the five measured cells was saved as `figures/measured_cells.png`.

### R Analysis

- The Fiji measurements were imported into RStudio using an R script.
- The measurements were analyzed to examine cell area, circularity, aspect ratio, and mean actin fluorescence intensity.
- Mean values were calculated to summarize the five selected cells.
- A scatter plot was generated to examine the relationship between cell area and circularity.
- A graph was generated to compare the mean actin fluorescence intensity of the five measured cells.
- The figures were saved in the `figures/` folder.

---

## Results ##

The following figures present the results of the cell morphology analysis using Fiji and RStudio. Five HT29 cells from image ID 13571 were examined to determine their cell area, circularity, aspect ratio, and mean F-actin fluorescence intensity.

### Five Measured HT29 Cells

The actin fluorescence image was opened in Fiji, where five cells were selected and traced using the Freehand Selection tool. Each cell outline was added to ROI Manager, and the Show All and Labels options were used to display the selected cells. The annotated image was saved for documentation.

**Figure 1. Measured HT29 Cells**

*Description: F-actin fluorescence image of HT29 human colon-cancer cells from the BBBC018 dataset, image ID 13571, showing the five selected cells used for cell morphology analysis in Fiji.*

[View Figure 1 (Measured Cells)](figures/measured_cells.png)

### Cell Area versus Circularity

Using the measurements obtained from Fiji, a scatter plot was generated in RStudio to examine the relationship between cell area and circularity among the five selected cells.

**Figure 2. Cell Area versus Circularity**

*Description: Scatter plot showing the relationship between cell area and circularity among the five measured HT29 cells displaying the Angular cell edges phenotype from image ID 13571.*

[View Figure 2 (Cell Area versus Circularity)](figures/area_vs_circularity.png)

The measured cell areas ranged from 1,586 to 4,404 pixels². Cell 2 had the largest area, while Cell 1 had the smallest area. Circularity values ranged from 0.426 to 0.832, with a mean circularity of approximately 0.580. These differences indicate variation in the shapes of the selected cells.

### Actin Fluorescence Intensity

The mean actin fluorescence intensity of the five measured cells was compared to examine differences in F-actin signal.

**Figure 3. Actin Fluorescence Intensity**

*Description: Graph comparing the mean F-actin fluorescence intensity of five measured HT29 cells from image ID 13571, representing the Angular cell edges phenotype.*

[View Figure 3 (Actin Fluorescence Intensity)](figures/actin_intensity.png)

The mean actin fluorescence intensity across the five cells was approximately 370.947. Cell 1 had the highest mean intensity at 425.834, while Cell 2 had the lowest at 301.647. These differences indicate variation in the measured actin fluorescence signal among the selected cells.

---

## Cell Morphology Summary ##

The measurements obtained from Fiji were summarized to compare the morphological characteristics of the five selected HT29 cells.

| Phenotype | Image ID | Cells Measured | Mean Area (px²) | Mean Circularity | Mean Aspect Ratio | Mean Actin Signal |
|---|---:|---:|---:|---:|---:|---:|
| Angular cell edges | 13571 | 5 | 3143.4 | 0.580 | 1.653 | 370.947 |

The mean cell area was 3,143.4 pixels², and the mean aspect ratio was approximately 1.653. The mean circularity of 0.580 indicates that the measured cells varied in how closely their shapes resembled circles. The average actin signal was approximately 370.947.

---

## Interpretation ##

The cell morphology analysis showed differences in the size, shape, and F-actin fluorescence intensity of the five selected HT29 cells. Cell area varied considerably, indicating that the selected cells differed in size. Circularity also varied, suggesting differences in cell shape. The aspect ratio provided additional information about cell elongation, while mean actin fluorescence intensity showed differences in the measured F-actin signal.

These findings are relevant to the study of the cytoskeleton because actin filaments help maintain cell shape and support changes in cell morphology. However, the measurements describe only five selected cells from one image field. Therefore, the results cannot establish that all cells displaying the Angular cell edges phenotype have the same characteristics.

---

## Conclusion ##

This activity demonstrated how Fiji and RStudio can be used to analyze cell morphology and F-actin fluorescence in HT29 human colon-cancer cells. Five cells from BBBC018 image ID 13571 were measured to compare cell area, circularity, aspect ratio, and mean actin fluorescence intensity.

The results showed variation in cell size, shape, and actin fluorescence signal among the selected cells. This activity provided practical experience in using image-analysis software to quantify cellular characteristics and understand the relationship between the cytoskeleton and cell morphology.

---


## References ##

Broad Institute. (n.d.). *Broad Bioimage Benchmark Collection (BBBC).* https://bbbc.broadinstitute.org/

Schneider, C. A., Rasband, W. S., & Eliceiri, K. W. (2012). NIH Image to ImageJ: 25 years of image analysis. *Nature Methods, 9*, 671–675. https://doi.org/10.1038/nmeth.2089

R Core Team. (n.d.). *R: A language and environment for statistical computing.* https://www.r-project.org/
```
