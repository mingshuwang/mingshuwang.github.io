+++
# Date this page was created.
date = 2017-12-15T00:00:00

# Project title.
title = "Polycentricity & Carbon Emissions"

# Project summary to display on homepage.
summary = "We explored the relationship between urban forms (e.g., **polycentricity** and **compactness**) and carbon dioxcide emissions in over 100 Chinese cities."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "FFDAS.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`

tags = ["polycentric_urban_development","China"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

+++
Since 2007, China has become the nation with the highest amount of CO<sub>2</sub> emissions. Aiming at contributing to the global emission reduction goals while sustaining the country’s economic development, the Chinese government has
adopted advancing the development of low-carbon cities. More recently, at the 4th Central Government Urban Conference (2015), China’s leadership reiterated the importance of the pursuit of **compact, efficient, and environmentally friendly urban development**.

Although existing GHG emission reduction strategies rely on technological solutions (e.g., renewable energy and zero-carbon buildings) and market-based approaches (e.g., carbon trading), they are oftentimes unable to reach carbon reduction goals by themselves. Similarly, smart city initiatives call for an integrated approach to sustainability, emphasizing the idea that **technology is not enough"**. Indeed, a growing body of literature has identified that **urban forms** can be used as a supplementary emission reduction strategy.

Since the late 1990s, research has highlighted the role of urban forms, including **polycentric** urban form and **compact** urban form, in fostering sustainable development. Therefore, in this project, we explored the relationship between urban forms (e.g., **polycentricity**, **compactness**, size, wealth, density) and CO<sub>2</sub> emissions in over 100 Chinese cities based on multi-sourced data. Before empiricallytesting any relatioship, we had to find data for/in China.


***

##### Carbon Emission Data for China

There are three gridded CO<sub>2</sub> datasets available for China, namely the Emission Database for Global Atmospheric Research ([EDGAR](http://edgar.jrc.ec.europa.eu/)), the Fossil Fuel Data Assimilation System ([FFDAS](http://www.gurneylab.org/portfolio-item/ffdas/)), and the China High Resolution Emission Gridded Data ([CHRED](http://www.cityghg.com/)). Additionally, National Bureau of Statistics of China (NBSC) provides energy statistics at province level.

Data|Temporal Span|Spatial Resolution|Spatial Coverage
----|-------------|------------------|----------------
EDGAR|1970--2012|0.1° × 0.1°|Global|
FFDAS|1997--2011|0.1° × 0.1°|Global|
CHRED|2007, 2012|10 km × 10 km, 1 km× 1 km|China

![Province R](/img/jcp2017.png)
*Three gridded CO<sub>2</sub> datasets of China, in 2007*

***

- Correlation coefficient (Pearson's *r*) at province level (N=30):
![Province R](/img/jcp2017_prov_R.png)

- Correlation coefficient (Pearson's *r*) at prefecture city level (N=340):
![Prefecture R](/img/jcp2017_pre_R.png)


***

##### Urban Forms VS CO<sub>2</sub> emissions

- Conceptualization of **compactness**
    + *A* = the area of the gray square (rectangle); *A'* = the area of the dotted circle
    + More compact (a) and Less compact (b) urban form
![compactness](/img/jupd2017_compactness.jpg)

- Conceptualization of **polycentricity**
    + Each solid circle refers to a subdivision of a city; the relative area of the circle denotes the relative population size of that subdivision
    + A less polycentric urban systems (a) and a more polycentric urban systems (b)
![polycentricity](/img/jupd2017_poly.jpg)

- Results
    + **Polycentric** urban form is associated with **more** CO<sub>2</sub> emissions.
    + **Compact** urban form is associated with **less** CO<sub>2</sub> emissions.
    + **Larger** cities are more energy efficient (economies of scale).
    + There is a substantial **Wealth effects** on carbon emissions.

***

##### References
- **Mingshu Wang**, Marguerite Madden, Xingjian Liu. (2017).[Exploring the Relationship between Urban Forms and CO2 Emissions in 104 Chinese Cities.]({{< ref "publication/jupd2017.md">}}) *Journal of Urban Planning and Development*, *4*, 04017014.
- **Mingshu Wang**, Bofeng Cai. (2017). [A two-level comparison of CO2 emission data in China: Evidence from three gridded data sources]({{< ref "publication/jcp2017.md">}}) *Journal of Cleaner Production*, *148*, 194-201.