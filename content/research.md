---
title: "Research"
date: 2026-07-24T12:00:00Z
menu: main
weight: 20
draft: false
header:
  navbar:
    enable: true
math: true
---

<meta name="color-scheme" content="light dark" />

## Current Research

#### Evaluating Aerosols in GEOS-CAM

Accurate forecasts of aerosols are essential for predicting air quality and its impacts on human health. Weather prediction models that couple aerosols to the meteorology, such as the Goddard Earth Observing System (GEOS) Forward Processing (GEOS-FP), provide a wealth of information that can be used to further our understanding of air quality prediction. Recent advancements in the use of a stretched grid to allow for high spatial resolution over the United States have allowed for the GEOS Convection Allowing Model (GEOS-CAM) to generate forecasts of meteorological and aerosol diagnostics at a resolution as fine as ~2.5 km. 

While aerosols in GEOS-FP have been thoroughly evaluated in a research framework, validation of aerosols within GEOS-CAM has been limited up until this point. By performing a more in-depth assessment of aerosols within GEOS-CAM, recommendations can be made for applications of these forecasts and areas of improvement within GEOS-CAM. To evaluate GEOS-CAM, aerosol optical depth (AOD) forecasts were compared with the GEOS-FP prediction system and ground-based observations of AOD values from the Aerosol Robotic Network (AERONET). 

When compared against AERONET observations, both GEOS-CAM and GEOS-FP showed similar bias and RMSE throughout much of the United States regardless of forecast hour or initialization time as seen in Figure 1. This was not true however along the east coast of the United States where strong negative biases and high RMSE values were found in GEOS-CAM only. This discrepancy was a result of the mid-July 2026 extreme smoke event that the eastern United States faced. When analysis was performed without the extreme smoke event days, this discrepancy between the models no longer exists, as seen [here](/uploads/no_smoke_aod_6panel_ALL_20260529_20260721_00z.gif).


{{< figure src="/uploads/aod_6panel_ALL_20260529_20260727_00z.gif" title="Figure 1" caption="Biases (top), RMSE (middle), and Correlation (bottom) present throughout the United States in GEOS-CAM (left) and GEOS-FP (right)." alt="Biases (top), RMSE (middle), and Correlation (bottom) present throughout the United States in GEOS-CAM (left) and GEOS-FP (right)." >}}

GEOS-CAM is shown to be performing well throughout the United States with correlations around 0.75 as seen in Figure 1. GEOS-FP also performed well with correlations much closer to 1.0. While each model is likely subject to underlying biases related to smoke emission, transport, and optical properties, this discrepancy is believed to be a result of the lack of AOD data assimilation within GEOS-CAM. This was difficult to identify in regular day-to-day variability of AOD as seen [here](/uploads/GSFC_no_smoke_speciation.png), but was easily identifiable during the extreme smoke event.

{{< figure src="/uploads/GSFC_speciation_smoke.png" title="Figure 2" caption="Speciation of AOD at Goddard Space Flight Center during an extreme smoke event in mid-July 2026." alt="Speciation of AOD at Goddard Space Flight Center during an extreme smoke event in mid-July 2026." >}}

In Figure 2, each day at 18Z a drastic change in AOD is seen in the GEOS-FP portion that is not present in the GEOS-CAM portion. When this AOD data assimilation occurs, the modeled GEOS-FP AOD value adjusts to more closely match observations for the initial conditions. This can also be observed when looking at the evolution of the forecasts in Figure 3. The evolution of the GEOS-CAM AOD forecasts shows an increase in AOD that aligns with the timing of the observed AOD increase but does not match the magnitude of the increase. The increase of AOD in the GEOS-FP forecasts aligns in both the timing and magnitude of the observed AOD increase. 

{{< figure src="/uploads/chiclet_aod_GSFC.png" title="Figure 3" caption="Evolution of the AOD forecasts from July 15th to July 20th at Goddard Space Flight Center." alt="Evolution of the AOD forecasts from July 15th to July 20th at Goddard Space Flight Center." >}}

<!-- {{< qr text="www.linkedin.com/in/carturner" />}} -->
Check out my [poster](/uploads/AnEvaluationOfAerosolsInGEOS-CAM.pdf)

Check out this GEOS-CAM [animation](https://svs.gsfc.nasa.gov/5665)

## Previous Work

#### Quantifying Methane Fluxes Over the Great Dismal Swamp

Methane accounts for 12% of all greenhouse gases and is approximately 80 times more effective at trapping heat in the atmosphere than carbon dioxide. It is estimated that 20-40% of natural methane emissions come from wetlands causing high levels of uncertainty in climate models. Quantifying methane emissions from wetlands allows for more accurate climate model predictions. Two bottom-up studies, measuring the source to estimate the plume, have been conducted in the Great Dismal Swamp in 1980-1981 and 2018 to identify methane fluxes. This study uses a top-down technique, measuring the plume to estimate the source, to identify methane fluxes and compare measurement techniques. 

To quantify methane emissions with a top-down approach, the mass balance technique was used. This technique uses wind speed and direction with gas concentrations to identify trace gas concetrations moving through a plane with the equation below. This technique was used with methane measurements taken over the Great Dismal Swamp during the SARP 2025 field campaign flights.

$$
flux=vcos(\alpha)\int_{z_o}^{z_1}\int_{-y}^{y}(X-X_{bg})dydz
$$

![Visual Respresentation of the Mass Balance Technique used to identify trace gas concentrations moving through a plane.](/uploads/mbt_diagram.png)

When compared, the top-down and bottom-up analyzes of methane fluxes from the Great Dismal Swamp showed similar results. Bottom-up methods showed slightly lower levels of methane flux but this could be due to variability in the day to day timescale. This study provides a basis for comapring top-down and bottom-up methane fluxes but does not provide a complete picture. Accurate comparisons are limited by the lack of concurrent top-down and bottom-up measurements. 


Check out my AGU 2025/ AMS 2026 [Poster](/uploads/SARP_Site_Poster.pdf)
