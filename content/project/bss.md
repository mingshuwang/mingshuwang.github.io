+++
# Date this page was created.
date = 2017-11-30T00:00:00

# Project title.
title = "Bike-sharing Systems & Congestion"

# Project summary to display on homepage.
summary = "In the past decades, there has been a resurgence of public bike-sharing systems (BSSs). While it is claimed that social and environmental benefits are associated with the implementation of BSSs, few empirical studies have investigated the actual effect of BSSs on cities."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "JTG2017.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`

tags = ["urban_mobilities","United_States"]

# Optional external URL for project (replaces project detail page).
# external_link = {{< ref "project/bss.md" >}}

# Does the project detail page use math formatting?
math = false

+++
A resurgence of (public) bike-sharing systems (BSSs) has been witnessed around the world in the past decades. Although the idea of BSSs has been around for almost half a century, it is only recently that such systems have been strategized as sustainable transportation means worldwide.

Contemporary internet and communication technologies (ICTs) are typically embedded into BSSs to facilitate program management and operation. For instance, smartphone apps are developed and provided to the end-user to enable bike check-out and return. The global positioning system (GPS) units are also adopted in some BSSs to track bike locations. Geographic information system (GIS) has also been introduced to monitor and allocate bikes across different docking stations.

Although the explicit goals of the introduction of individual BSSs may be different, BSSs are associated with social, environmental, and health benefits, including but not limited to (1) congestion, emission, air pollution, and noise reductions, (2) flexible mobility, transportation connection improvement, (3) consumer financial savings, and (4) health promotion. Nevertheless, there is limited empirical evidence about the actual effects of BSSs on cities.

***

##### Bike-sharing Systems (BSSs) VS Congestion

With a panel dataset of 96 urban areas in the US from 2005 to 2014, we employed a difference-in-differences (DID) model with two-way fixed-effects panel regression with propensity score matching (PSM).

**Findings**:

- BSSs can reduce rush hour congestion.
- BSSs benefit larger cities more than smaller ones in congestion reduction.
- Wealthier cities tend to get worse off with the introduction of BSSs.


Bike-sharing systems (BSSs) in US urban areas (2005–2014)
![cues2018](/img/JTG2017.jpg)

***

##### References
- **Mingshu Wang**, Xiaolu Zhou. (2017).[Bike-sharing systems and congestion: Evidence from US cities.]({{< ref "publication/2017_JTG.md">}}) *Journal of Transport Geography*, *65*, 147-154.