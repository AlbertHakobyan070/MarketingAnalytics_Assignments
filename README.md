# Bass Model Analysis — Samsung Micro RGB TV

**Author:** Albert Hakobyan  
**Course:** DS 223 · Marketing Analytics (AUA)  
**Date:** March 2026

---

## What this is

A Bass diffusion model analysis predicting the adoption of Samsung's Micro RGB TV (announced 2025, $29,999 for 115"). LG's OLED TV (2013–2025) is used as the look-alike product to estimate innovation (p) and imitation (q) parameters.

## Innovation chosen

**Samsung Micro RGB TV** — selected from TIME's Best Inventions of 2025. It uses individually controlled RGB LEDs under 100 micrometers, achieving 100% BT.2020 color gamut. It targets the same ultra-premium segment that OLED TVs which entered the market a decade earlier.

## Look-alike product

**LG OLED TV** (2013–2025) — the first commercially successful OLED TV, launched at ~$15,000 in 2013. Both products are premium display technologies from Korean manufacturers that created entirely new TV categories.

## Results for the Samsung's Micro RGB TV:

| Parameter | Value |
|---|---|
| p (innovation) | 0.0032 |
| q (imitation) | 0.4428 |
| m (market potential) | ~38.8M units |
| Predicted peak year | ~2036 |
| Peak annual shipments | ~4.36M units |

## Repo structure

```
├── README.md
├── bass_model_analysis.Rmd
├── data/
│   └── OLED_TV_Global_Annual_Shipments_2013_2025.csv
├── report/
│   ├── Albert Hakobyan MA Bass Model Assignment 1
│   └── other/  Component pdf/html files of the combined report
└── img/ 
    └── Empty (No images were made for this project, all figures are in the report)
```

> Download and view the report/Albert Hakobyan MA Bass Model Assignment 1.pdf for the most amount of information about the project.

## Data sources

OLED TV shipment data (2013–2025) was compiled from free, publicly accessible industry sources:

- **DisplaySearch / OLED-Info** (2013–2014): [oled-info.com](https://www.oled-info.com/displaysearch-says-77000-oled-tvs-were-sold-2014-generating-280-million-revenue)
- **LG Display IR calls** (2015): [oled-info.com](https://www.oled-info.com/lg-display-sold-400000-oled-tv-panels-2015-half-q4)
- **IHS Markit** (2016–2019): via [Broadband TV News](https://www.broadbandtvnews.com/2018/01/05/record-number-of-oled-tvs-shipped-before-the-holidays/), [OLED-Info](https://www.oled-info.com/ihs-global-oled-tv-sales-were-11-million-q4-2019)
- **TrendForce** (2020–2023): [trendforce.com](https://www.trendforce.com/presscenter/news/20221019-11431.html), [Statista](https://www.statista.com/statistics/260316/global-oled-tv-shipments/)
- **Omdia** (2024–2025): [BusinessWire](https://www.businesswire.com/news/home/20250227890254/en/), [OLED-Info](https://www.oled-info.com/omdia-samsung-electronics-sold-around-2-million-oled-tvs-2025-38-2024)

## How to run

1. Open `bass_model_analysis.Rmd` in RStudio
2. Make sure `./data/OLED_TV_Global_Annual_Shipments_2013_2025.csv` is in place
3. Knit to HTML

Required packages: `ggplot2`, `ggpubr`, `knitr`, `diffusion` (installed automatically by the script).
