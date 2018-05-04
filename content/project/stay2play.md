+++
# Date this page was created.
date = 2017-01-01T00:00:00

# Project title.
title = "Plan Your City Trip based on User-generated Contents"

# Project summary to display on homepage.
summary = "This project proposes a travel planner for city trips by integrating multiple crowdcoursed user-generated contents to provide cutomized information for tourists. We harvested hotel reviews from [TripAdvisor](https://www.tripadvisor.com), photos from [Flickr](https://www.flickr.com), and travel costs from [Uber](https://www.uber.com)."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "ag2017_recommendation.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`

tags = ["urban_mobilities","United_States"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

+++
Customers rely on online user-generated contents (UGC) to make purchase decisions for travels. Travelers tend to seek advice from ratings and reviews prior to booking accommodations. Hotel managers utilize UGC to predict different facets of business performance and web traffic volume to predict hotel demand.

While a number of tourism websites provide information about destinations, accommodation and route selection, integrating and comparing different types of information from many contributors require significant time and effort. The number of choices makes it very difficult for consumers to find what they are looking for. Most tourists usually seek for information in three aspects before their travels: **hotels to stay in**, **places to visit**, and **routes that connect hotels and attractions**.

We aim to develop a geospatial analytical tool to assist decision-making in city-tour planning. We identified multidimensional characteristics of hotels from [TripAdvisor](https://www.tripadvisor.com) with natural language processing (NLP), extracted tourist hotspots from [Flickr](https://www.flickr.com) images with geospatial data mining techniques, and recommended travel routes and sequences based on [Uber](https://www.uber.com) with graph analysis.

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
- Xingjian Liu, **Mingshu Wang**. (2016).[How polycentric is urban China and why? A case study of 318 cities.]({{< ref "publication/land2016.md" >}}) *Landscape and Urban Planning*, *151*, 10-20 (equal contribution, co-first author).
- Xingjian Liu, Ben Derudder, **Mingshu Wang**. (2017). [Polycentric urban development in China: A multi-scale analysis.]({{< ref "publication/epb2017.md" >}}) *Environment and Planning B: Urban Analytics and City Science*, [DOI](https://doi.org/10.1177/2399808317690155).