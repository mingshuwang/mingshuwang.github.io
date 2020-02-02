+++
# Date this page was created.
date = 2017-01-01T00:00:00

# Project title.
title = "How Polycentric is Urban China?"

# Project summary to display on homepage.
summary = "We quantified the degree of polycentric urban development at both **intra-urban** and **inter-urban** levels in China with the U.S. Oak Ridge National Laboratory (ORNL)'s [LandScan](https://landscan.ornl.gov/) dataset."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "PUR_CN.png"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`

tags = ["polycentric_urban_development","China"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

+++
**Polycentric urban development** refers to different forces causing multiple previously close-by but independent urban sub-divisions to become a larger and more integrated **urban system**. **Polycentricity** is oftentimes deemed a desirable urban form, generating greater agglomeration externalities as well as facilitating the achievement of social, economic, and environmental goals. Polycentric urban development has been observed and analyzed at various geographical scales, including the **intra-urban** (e.g., Central Business Districts (CBDs), edge cities, and satellite towns within a city), and **inter-urban** (e.g., the ‘Pearl River Delta’ mega-city region) scales.

Despite much insightful work on polycentric urban development in China, there is a lack of systematic comparison at either scale. Therefore, in this project, we identified polycentric urban structure and quantified the degree of polycentricity in China at both **intra-urban** scale (i.e., [318 Chinese cities]({{< ref "publication/land2016.md" >}})) and **inter-urban** scale (i.e., [22 City-Regions]({{< ref "publication/epb2017.md" >}})) using detailed gridded population data, [U.S. Oak Ridge National Laboratory (ORNL)'s LandScan](https://landscan.ornl.gov/) dataset.

***

##### Intra-urban Polycentricity
![Chinese cities at prefecture level and above.](/img/LAND2016.jpg)
Chinese cities at prefecture level and above.

- Over 90% of cities have four or fewer intra-urban (sub)centers.
![hist_N](/img/land2016_N.png)

- Higher degree of polycentricity is found in **mountainous** cities.

- Polycentricity is positively associated with GDP per capita in **Eastern** China.

- Identified patterns of centers in a number of cities are largely consistent with corresponding master plans, for example, Shanghai and Beijing.
![shanghai](/img/land2016_sh.png)
![beijing](/img/land2016_bj.png)

***

##### Inter-urban Polycentricity: Polycentric Urban Regions (PURs)
![Polycentric Urban Regions (PURs) in China](/img/PUR_CN.png)

PUR|Full Name|Major Cities|Area*
---|---------|------------|----
BTH|Beijing-Tianjin-Hebei|Beijing, Tianjin|18.27
CSX|Central Shanxi|Taiyuan|2.79
CIM|Central Inner Mongolia|Hohhot|13.19
LDP|Liaodong Peninsula|Shenyang, Dalian|12.76
HAC|Harbin-Changchun|Harbin, Changchun|18.53
YRD|Yangtze River Delta|Shanghai, Nanjing, Hangzhou|10.05
CAH|Central Anhui|Hefei|8.63
EFJ|Eastern Fujian|Fuzhou, Xiamen (Amoy)|5.5
NJX|Northern Jiangxi|Nanchang|5.78
SDP|Shandong Peninsula|Jinan, Qingdao (Tsingtao)|7.39
CPL|Central Plain|Zhengzhou|5.68
EHB|Eastern Hubei|Wuhan|5.09
EHN|Eastern Hunan|Changsha|2.81
PRD|Pearl River Delta|Guangzhou, Shenzhen|5.47
SGX|Southern Guangxi|Nanning|4.26
CHC|Chengdu-Chongqing|Chengdu, Chongqing|26.65
CGZ|Central Guizhou|Guiyang|10.46
CYN|Central Yunnan|Kunming|9.45
GZP|Guanzhong Plain|Xi’an|5.54
LAX|Lanzhou-Xining|Lanzhou, Xining|6.85
NNX|Northern Ningxia|Yinchuan|4.07
TSM|Tianshan Mountains|Urumqi|9.56
*Area is in 10,000 sq. km*

***

- A typology of Chinese PURs is presented based on the average **intra-urban** polycentricity and **inter-urban** polycentricity, where there is only **limited** levels of association between inter-urban and inter-urban polycentricity.
![scatter](/img/epb2017_scatter.png)


- The **Yangtze River Delta** (see below) and **Pearl River Delta** have high levels of both **intra-urban** and **inter-urban** polycentricity.
![YRD](/img/epb2017_yrd.png)


- Most PURs in **Central** and **Western** China are characterized by a
primate urban system and low levels of inter-urban polycentricity, for example, the Central Guizhou (CGZ) PUR:
![CGZ](/img/epb2017_cgz.png)

***

##### References
- Xingjian Liu, **Mingshu Wang**. (2016).[How polycentric is urban China and why? A case study of 318 cities.]({{< ref "publication/land2016.md" >}}) *Landscape and Urban Planning*, *151*, 10-20 (equal contribution).
- Xingjian Liu, Ben Derudder, **Mingshu Wang**. (2018). [Polycentric urban development in China: A multi-scale analysis.]({{< ref "publication/epb2017.md" >}}) *Environment and Planning B: Urban Analytics and City Science*, *45*(5), 953-972. [DOI](https://doi.org/10.1177/2399808317690155).