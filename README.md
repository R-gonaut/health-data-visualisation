# health-data-visualisation

This project accompanies the project poster produced 'THE TIDES OF TOURISM', plus a presentation video hosted on youtube. The poster is not included in this repository as it is subject to marking and cannot be shared publicly.

The video presentation can be accessed via a private link by scanning the QR code on the poster itself. This is the only way to view the video presentation.

Author: Adam Moore

# Sources

Road traffic collision data was aquired from UK Government data (UK.Data.Gov) accessed via Stats19, the 'Road Safety - Collisions last 5 years' data file was used: https://www.data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-safety-data

LSOA boundary data was acquired from Data Map Wales: https://datamap.gov.wales/layers/geonode:lsoa_2021_w_hwm

Information regarding tourism in Pembrokeshire, including the statistic on the poster (66% returning tourists) was aquired from Visit Pembrokeshire: https://www.visitpembrokeshire.com/industry/research-and-statistics

# Rationale

As a Pembrokeshire resident, and national health service employee in the region, I am often confronted with the idea and concept that the area has extremely high levels of summer tourism, and that this tourism has a suathe of negative impacts that more than offset the positive economic impacts. I do not hold strong views on this supposed issue, and thoroughly enjoy services throughout the year that would likely not be sustainable or realistic without high levels of tourism in the summer that generate revenue. 

I do however, have a distinct curiosity as to whether or not such claims have merit. Do families travelling to holiday here really have clear negative impacts? Increased levels of traffic appear clear, though stats19 data with respect to this is presently not available. True negative impacts, such as potential increased collisions and casualties though can be investigated. The summer months yield far kinder driving conditions, with lighter, drier, less windy, less hazardous roads. These conditions will offset any increase. There are also many, many other factors that could contribute to any observed increase, such as increased agricultural activity, loose animals, mud or debris on roads (often due to agriculture), more young drivers on the road outside of school term times, more young drivers on roads outside of University term times and so on.

Many of these angles are speculative and are not underpinned in this analysis by evidence; there are too many variables and not enough granular data to account for each variable in a truly robust way. For this reason, a more simplistic approach will be taken and the analysis will simply look to determine whether there is an increase, and if so how Pembrokeshire (the most visited county, with lower than average agriculture across those looked at) stacks up against other coastal local authorities in west wales. We can draw some insight from visualising the relative differences between peak season and off season collision rates. I expect to see relatively higher casualties across Pembrokeshire, particularly along the coastline, and fewer further in-land away from tourist residences and camping sites. I would also expect Pembrokeshire to have a greater relative rate increase than all other counties. These expectations are somewhat generalistic, and do not properly account for how generally treachorous particular roads are, how much travelling is done on particular types of roads, or the speeds of those roads. Some broad insight can be inferred, however, and the strong views I have encountered from Pembrokeshire residents and NHS colleagues would certainly be called into question if anything but the aforementioned specualations are clearly observed. 

Visually, Wales' distinct geography was a core part of the design concept.

# Methodology

The true tourism peak season is a complex concept, with half-terms, bank holidays, summer breaks, and so on, contributing to tourism. These are often asynchronous between England and Wales, and the weather on each occassion has a significant impact on the extent of any tourism. Rather than identifying a robust methodology to classify individual dates as 'peak' and 'off' season, the period June to August (3 months) annually will be considered 'peak' season, and the remaining nine months will be considered 'off' season. This is potentially flawed, but clearly more simple with less risk of error involved.

A monthly average volume of casualties for each LSOA during both peak and off seasons are calculated, and then made equivalent by dividing the sum of the peak season casualties by 15 (as there are 15 peak season months across five years), and the off season is calculated by dividing the sum of the off season casualties by 45 (as there are 45 off season months). This yields a monthly average casualty number for each LSOA for both peak and off season months.

An additional field is calculated by subtracting the off season average monthly casualties from the peak season casualties. This field has both positive and negative values, with positive values representing LSOAs with relatively more casualties during peak season, and negative values representing LSOAs with relatively fewer during peak season. This is used to plot the spatial map of West Wales on the poster.

In addition to this, by dividing the monthly average off season casualties at a local authority level from the monthly average peak season casualties at a local authority level, a relative increase can be ascertained. This was then plotted in a radial bar chart. 

Much further analysis was completed, exploring the impacts of an array of other variables, however the more granular the data was explored, the less rational it seemed to draw conclusions without vital contextual data (such as traffic data) to complement it. Sticking to the brief and keeping the analysis simple enabled more robust conclusions, even though the conclusion was both heavily caveated and not at all groundbreaking. Honesty and responsibility was prioritised ahead of shock value and deep-dive analysis in this project.

# Conclusion

No robust conclusions can be drawn from this work alone, as there are simply far too many variables that are not accounted for nor considered. The methodology is somewhat flawed in that, at this level of granularity (LSOA) there are not that many collisions and so other factors, such as simply how treacherous roads are in general could be having disproportionate impacts on how the spatial data has been visualised and presented.

The work does, however, challenge conventional views held by some Pembrokeshire residents in particular. Comprehensive and robust analysis could further unpick and explain this increase and determine why this increase occurs, and why it is lower in Pembrokeshire than other similar counties. As the most visited county, Pembrokeshire is heavily relied on as a proxy for the impact of tourism alone. This is not unreasonable, but is limited in validity with respect to concluding that tourism does not have a signicant impact on the rate of collisions. This absolutely remains unclear despite this work.
