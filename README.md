
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



## Five Measured HT29 Cells

The actin fluorescence image was opened in Fiji, where five cells were selected and traced using the Freehand Selection tool. Each cell outline was added to the ROI Manager, and the **Show All** and **Labels** options were enabled to display the selected cells with their corresponding labels.



*Description: F-actin fluorescence image of HT29 human colon cancer cells from the BBBC018 dataset (Image ID: 13571), showing the five selected cells used for morphological analysis in Fiji. Each selected cell is labeled for identification.*

[View Figure 1: Five Measured HT29 Cells](https://github.com/EllaCadungog/cytoskleleton-BBBC018-13571/blob/main/figures/measured__cells.png)

**Figure 1.** The image shows five HT29 cells selected for morphological analysis. The cells display differences in their size and shape, with some showing more angular or irregular boundaries. These visible differences are consistent with the Angular cell edges phenotype. The selected cells were used to measure cell area, circularity, and actin fluorescence intensity to quantify their morphological characteristics.

---

## Cell Area versus Circularity

The measurements obtained from Fiji were analyzed in RStudio. A scatter plot was generated to examine the relationship between cell area and circularity among the five selected cells.

*Description: Scatter plot illustrating the relationship between cell area and circularity among five measured HT29 cells displaying the Angular cell edges phenotype from image ID 13571.*

[View Figure 2: Cell Area versus Circularity](https://github.com/EllaCadungog/cytoskleleton-BBBC018-13571/blob/main/figures/area_vs_circularity.png)

**Figure 2.** The measured cell areas ranged from 1,586 to 4,404 pixels². Cell 2 had the largest area, while Cell 1 had the smallest area. Circularity values ranged from 0.426 to 0.832, with a mean circularity of approximately 0.580.

The differences in cell area indicate that the selected HT29 cells varied in size. The circularity values also showed variation in cell shape. Cells with lower circularity values had outlines that were less similar to a perfect circle, while higher values indicated more rounded shapes. These findings suggest that the selected cells exhibited differences in their morphology, which is consistent with the Angular cell edges phenotype.

---

## Actin Fluorescence Intensity

The mean actin fluorescence intensity of the five measured cells was compared to examine differences in F-actin signal.



*Description: Graph comparing the mean F-actin fluorescence intensity of five measured HT29 cells from image ID 13571, representing the Angular cell edges phenotype.*

[View Figure 3: Actin Fluorescence Intensity](https://github.com/EllaCadungog/cytoskleleton-BBBC018-13571/blob/main/figures/actin_intensity.png)

**Figure 3.** The mean actin fluorescence intensity across the five cells was approximately 370.947. Cell 1 had the highest mean intensity at 425.834, while Cell 2 had the lowest at 301.647.

The differences in mean actin fluorescence intensity indicate variation in the detected F-actin signal among the five HT29 cells. Cell 1 showed the highest fluorescence intensity, while Cell 2 showed the lowest. Since actin is an important component of the cytoskeleton, these differences may reflect variations in the distribution or abundance of F-actin within the selected cells. However, fluorescence intensity alone cannot determine the exact organization of the actin cytoskeleton or explain the cause of the angular cell edges.

---

## Overall Interpretation

The morphological analysis of five HT29 cells revealed variations in cell area, circularity, and actin fluorescence intensity. The differences in cell size and shape indicate that the selected cells did not have identical morphological characteristics. The circularity measurements and fluorescence intensity values further demonstrate variation among the cells. Overall, the findings are consistent with the Angular cell edges phenotype and show how Fiji and RStudio can be used to quantify cell morphology and F-actin fluorescence in HT29 human colon cancer cells.

## Cell Morphology Summary ##

**Table 1.** The measurements obtained from Fiji were summarized to compare the morphological characteristics of the five selected HT29 cells.
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
