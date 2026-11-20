# Nilgiris District Soil Fertility Analysis

An agricultural data analysis project evaluating soil health and nutrient distribution across samples from the **Nilgiris district, Tamil Nadu, India**. Raw laboratory test results are classified into fertility tiers (**Low, Moderate, High**) based on standard **Tamil Nadu Agricultural University (TNAU)** soil testing critical limits.

## Workbook Structure
The Excel workbook (`Nilgiris_Soil_Fertility_Analysis.xlsx`) is organized into four sheets:
1. **`Raw Data`**: Unmodified soil laboratory measurements across all sampled locations.
2. **`Fertility Status`**: Automated formula-based status classifications (`Low`, `Moderate`, `High`) for primary parameters and conditional color-coding (Red/Yellow/Green) for secondary and micronutrients.
3. **`Summary`**: Descriptive statistics (**Average, Minimum, Maximum, Sample Count**) across all 12 soil parameters, including data-quality flags for outlier values pending verification.
4. **`Charts`**: Comparative clustered column charts visualizing Macronutrient (`N, P, K`) and Secondary/Micronutrient (`S, Fe, Mg, Zn, Cu, B`) distributions.

## Soil Classification Standards (TNAU Reference)

### Primary Parameters & Macronutrients

| Parameter | Unit | Low / Deficient | Moderate / Good | High |
| :--- | :--- | :--- | :--- | :--- |
| **pH** | - | `< 6.5` (Acidic) | `6.5 – 7.5` (Neutral) | `> 7.5` (Alkaline) |
| **Electrical Conductivity (EC)** | dS/m | `<= 0.0` or `> 1.0` | `> 0.0 – 1.0` (Good) | - |
| **Organic Carbon (OC)** | % | `< 0.50` | `0.50 – 0.75` | `> 0.75` |
| **Nitrogen (N)** | kg/acre | `< 113` | `113 – 180` | `> 180` |
| **Phosphorus (P)** | kg/acre | `< 4.5` | `4.5 – 9.0` | `> 9.0` |
| **Potassium (K)** | kg/acre | `< 48` | `48 – 113` | `> 113` |

### Secondary & Micronutrients

| Parameter | Unit | Low (Red) | Moderate (Yellow) | High (Green) |
| :--- | :--- | :--- | :--- | :--- |
| **Sulfur (S)** | ppm | `< 10` | `10 – 15` | `> 15` |
| **Iron (Fe)** | ppm | `< 3.7` | `3.7 – 6.3` | `> 6.3` |
| **Magnesium (Mg)** | meq/100g | `< 1.0` | `1.0 – 1.5` | `> 1.5` |
| **Zinc (Zn)** | ppm | `< 1.2` | `1.2 – 2.0` | `> 2.0` |
| **Copper (Cu)** | ppm | `< 1.2` | `1.2 – 2.0` | `> 2.0` |
| **Boron (B)** | ppm | `< 0.5` | `0.5 – 1.0` | `> 1.0` |

## Data Quality & Methodology Notes
* **Automated Excel Logic**: Used nested `=IF()` and `=IF(AND())` functions to standardize classification across rows and eliminate manual entry errors.
* **Outlier Flagging**: Two anomalous readings (flagged with thick borders and cell notes in the `Fertility Status` and `Summary` tabs) were preserved for transparency and marked for laboratory re-verification.

## Tools Used
* **Microsoft Excel**: Data cleaning, conditional logic formulas, conditional formatting, descriptive statistics, and data visualization.
*
