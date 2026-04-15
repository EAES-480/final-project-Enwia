# data

Place data file(s) in this folder.

Then, include codebooks (variables, and their descriptions) for your data file(s)
using the following format.

Section 1: Introduction: 
This project investiagtes whether Titanite U-Pb ages are related to thermal and geochmeical conditions recorded in titanite from intrusive rock samples associated with porphyry copper deposit systems from the state of Sonora, Mexico. Titanite is a useful accessory mineral because it can preserve both trace element compositions and geochronological information, making it an effective tool for understanding magmatic processes. The dataset used in this study consists of titanite analyses from several rock samples. Each observation represents a single titanite analysis, with associated measurements of U–Pb age (Ma), Zr-in-titanite temperature (°C), Eu anomaly (Eu/Eu*), and Ce anomaly. Zr-in-titanite temperature provides an estimate of the thermal conditions during titanite crystallization. The Eu anomaly reflects plagioclase fractionation and magma evolution, while the Ce anomaly is commonly used as a proxy for oxidation state. By comparing these variables to titanite U–Pb ages, this project aims to determine whether magmatic conditions and geochemical signatures vary through time.

## name of data file --> Ttn.csv
Section 2: 
Observations: 279 titanite analyses
Variables: 5
- `Sample_ID`: Identifier for each titanite sample analysis point.
- `Temperature_C`: Temperature from Zr in titanite thermometer (°C)
- `Age_Ma`: The age of titanite crystallization measured in millions of years (Ma) using U–Pb geochronology.
- `Eu_Anomaly`: Europium anomaly is a ratio that measures the Eu anomaly relative to neighboring rare earth elements. Used as an indicator of: plagioclase fractionation, magma evolution, and redox conditions. Values >1 or <1 indicate enrichment or depletion of Eu.
- `Ce_Anomaly`: Cerium anomaly a ratio that measures the Ce anomaly relative to other rare earth elements. Commonly used as a proxy for: oxidation state (redox conditions) and magma fertility in porphyry systems.

Section 3: 
Response Variables (Y): Temperature_C, Eu_Anomaly, Ce_Anomaly
Predictor (X): Age_Ma

Question 1: Is titanite U–Pb age related to Zr-in-titanite temperature? Tests whether thermal conditions change through time.

Question 2: Is titanite U–Pb age related to the Eu Anomaly & Ce Anomaly? Tests whether fractionation processes and oxidation state vary with age.

Methods: I will use the figures above plus linear regression models. I made some scatter plots above of titanite U–Pb age versus each variable (Zr-in-titanite temperature, Eu anomaly, and Ce anomaly) to visually assess trends and relationships in the data. Next, I'm going to use linear regression models to quantify the relationships between age and each predictor variable. I'm planning to evaulate R^2 and p-value.


