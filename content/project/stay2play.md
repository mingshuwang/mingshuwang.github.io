+++
# Date this page was created.
date = 2017-04-01T00:00:00

# Project title.
title = "Plan Your City Trip based on User-generated Contents"

# Project summary to display on homepage.
summary = "This project proposes a travel planner for city trips by integrating multiple crowdcoursed user-generated contents to provide cutomized information for tourists. We harvested hotel reviews from [TripAdvisor](https://www.tripadvisor.com), photos from [Flickr](https://www.flickr.com), and travel costs from [Uber](https://www.uber.com)."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "ag2017_gui.jpg"

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

##### Where to Stay? --Natural Language Processing from TripAdvisor Reviews

Many products and services offered by hotels are intangible, which leads to information asymmetry between hotels and customers about the quality of products and services. Signal theory describes the signal behavior between two parties where information asymmetry exists. 

What customers write (i.e., the **contents**) and how customers write (i.e., the **linguistic style**) signal their satisfaction or dissatisfaction with hotel product and service attributes. It also serves as an indirect communication approach to hotel managers and future customers about the perceptions of their hotel stay.

While most studies only focus on numeric review ratings (e.g., rating scores or review volume) and/or sentiment analysis of the review content, we first investigated the role of **linguistic style** of review contents in predicting customers' satisfaction.

- **Findings**:
    + Higher **subjectivity** <-> lower satisfaction
    + Higher **readability** (Gunning Fog Index) <-> lower satisfaction
    + Longer **length** of textual review <-> lower satisfaction
    + Higher **lexical diversity** <-> higher satisfaction
    + Higher review involvement <-> higher satisfaction


Then, we extracted multidimensional hotel information from review contents based on [Stanford CoreNLP](https://stanfordnlp.github.io/CoreNLP/). Adapted from the Criteria for Hotel Operators and Quality Grading (Northernireland Tourist Board, 1982), we summarized the qualities of hotels into seven dimensions (i.e., facilities, bedroom, restroom, service, food, location, and overall). For each hotel, sentiment analysis was applied to all the seven dimensions:

![ag2017_nlp](/img/ag2017_nlp.jpg)

***

##### Where to Play? --Geospatial Data Mining from Flickr

Urban tourist destinations are increasingly interwoven into residents' living space, leading to socio-spatial interactions between **tourists** and **locals**. These sociospatial interactions between tourists and residents have significant implications for planning, especially in cities popular with tourists. Importantly, the mix of locals and visitors at the city and the neighborhood scales and such chance encounters may influence peoples' experience. With geo-tagged Flickr images, we mapped the spatial distribution of tourists and locals in ten US cities:
![cities2018_flickr](/img/cities2018_flickr.png)

Second, we generated location-based tag cloud for tourists and residents. In the location-based tag cloud, the size of the labels denotes the relative frequencies of the keyword at the particular location in Flickr. Orange represents more tourists and green represents more locals:
![cities2018_tag](/img/cities2018_tag.png)

Finally, we integrated the textual tags, the geographic locations, and the timestamps of Flickr to delineate the **potential locations** of tourist hotspots and rank the **popularitiy** of those hotspots.


***

##### What is the OPTIMAL Route Connecting Tourist Attractions and Hotels?

To simplify the model, we used average Uber cost to recommend travel sequences that connect attractions and hotels based on heuristically minimized travel cost. 

- **System Inputs**:
    + Hotel: Customer's weight (0 to 100) on the seven quality dimensions
    + Tourist Spots: Our recommendation based on polularity OR self-selected spots
    + The maximum distance a customer would like to walk
    + The number of days a customer would like to span in the city

![ag2017_gui](/img/ag2017_gui.jpg)

- **System Outputs**:
    + A recommended hotel
    + A route sequences that connects each spots and the recommended hotel
    + The estimated transportation cost (based on Uber)

![ag2017_simulation](/img/ag2017_simulation.jpg)


***

##### References
- Yabing Zhao, Xun Xu, **Mingshu Wang**. (2019).[Predicting overall customer satisfaction: Big data evidence from hotel online textual reviews]({{< ref "publication/ijhm2019.md" >}}) *International Journal of Hospitality Management*, *76*, *Part A*, 111-121.
- Dongying Li, Xiaolu Zhou, **Mingshu Wang**. (2018). [Analyzing and visualizing the spatial interactions between tourists and locals: A Flickr study in ten US cities.]({{< ref "publication/cities2018.md" >}}) *Cities*, *74*, 249-258.
- Xiaolu Zhou, **Mingshu Wang**, Dongying Li. (2017). [From stay to play – A travel planning tool based on crowdsourcing user-generated contents.]({{< ref "publication/ag2017.md" >}}) *Applied Geography*, *78*, 1-11.
- **Mingshu Wang**, Xiaolu Zhou. (2016). [Geography matters in online hotel reviews.]({{< ref "publication/isprsa2016.md" >}}) *ISPRS - International Archives of the Photogrammetry, Remote Sensing and Spatial Information Sciences*, *XLI-B2*, 573-576.