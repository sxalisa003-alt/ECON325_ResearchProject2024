# ECON325_ResearchProject2024



 
Table of Contents
INTRODUCTION	3
LITERATURE REVIEW	3
Hedonic Pricing and Property Features	3
Factors specific to host and platform	4
Market Saturation and Competition	4
MODEL SPECIFICATION AND DATA DESCRIPTION	4
Description of Variables and Data:	4
PRIORI EXPECTATIONS	5
Host Characteristics	5
Property Characteristics	6
Location Indicators	6
Regression Model Analysis	7
EViews Results and Analysis	7
Coefficient Interpretation and Evaluation	7
P-Value Interpretation	8
R-Squared, Adjusted R-Squared and F-Statistic Interpretation	8
Interactive Term Regression Model	9
Coefficient Interpretation	10
P-Value	11
R-Squared, Adjusted R-Squared and F-Statistic Interpretation	11
Conclusion	11
Recommendations	11
Reference List	12


 
INTRODUCTION
Airbnb, launched in 2008, is a digital marketplace that connects people who want to rent out their properties with people who are seeking to book accommodation for a short-term. The introduction of a digital marketplace has brought about a big evolution in the hospitality industry, transforming it from a traditional and rigid structure to a more flexible, peer-to-peer, and personalised structure. This evolution has changed the way accommodation services are being offered to tourists worldwide. The Cape Town tourism and hospitality industry has seen an influx of tourists ever since Airbnb was introduced to the city. However, the pricing dynamics of Airbnb have proven to be a challenge for hosts as they must consider a multitude of elements such as amenities, location advantages and disadvantages, and current prevailing local market trends to determine the rental rates effectively. This research report seeks to establish the aspects that impose the prices of Airbnb’s in Cape Town by investigating the factors that influence those prices using econometric models to explain variation in prices.
It is most critical that we understand the elements that influence the pricing of Airbnb’s in Cape Town, not only for the benefit of hosts who are seeking to maximise their profits but also for tourists who seek to find the best holiday destination at the most affordable price. This research utilises economic theories such as the hedonic pricing model, which, according to Montero and Fernández-Avilé (2023) is an economic model that suggests that the pricing of a good is dependent on its characteristics. It will also use econometric techniques to analyse an Airbnb dataset for Cape Town listings to estimate the relationship between various independent variables and the dependent variable (Price). 
The significance of this study lies in firstly providing insights into the pricing strategies within the short-term rental market, which can better inform hosts’ pricing tactics. Secondly, the results of this study can aid in having more informed discussions on the factors that influence Airbnb prices. Furthermore, pave way to making recommendations to improve rental and pricing strategies.
 LITERATURE REVIEW
Hedonic Pricing and Property Features
Using the hedonic pricing theory this study suggests that the prices of Airbnb’s are influenced by a variety of property-specific characteristics like amenities, listing type (room or home), parking, Wi-Fi, etc and external factors such as neighbourhood safety and proximity to attractions and commercial centres. A study conducted by Wen et al. (2021) has proved that elements like guest reviews and host reputation play a significant role in the price determination of Airbnb listings. Wen et al. (2021) also discovered that host comments, booking history and the “superhost” status can have a positive impact on the pricing as these attributes could be seen as high-quality service.
Research conducted by Zhang et al. (2019) shows that spatial features like proximity to tourist spots, commercial areas, and access to public transport play a significant role in price determination. These findings are relevant to Cape Town due to its dependence on tourism.
Factors specific to the host and platform
According to Teubner et al. (2017), trust indicators such as verified identity, positive reviews, high quality images of the Airbnb space have a huge impact on Airbnb rates. The study provides support for Ert et al. (2016) findings, which reported that a guest willing to pay more can also depend on the reputation of the host. This means that when customers are looking for accommodation, they also consider the hosts’ reputation as well as the property itself.
Market Saturation and Competition
In the context of the Cape Town market, supply and demand will have a role in the price determination process due to how competitive the Airbnb market has become. According to Zervas et al. (2017), properties that are in regions that have high Airbnb bookings are subjected to lower pricing because the market in that region is too competitive. This is essentially true for Cape Town, where the Airbnb market is rapidly increasing, leading to market saturation.

MODEL SPECIFICATION AND DATA DESCRIPTION
To estimate the determinants of Airbnb prices in Cape Town this study will make use of a multiple linear regression model and an interactive term regression model. Price will be the dependent variable (Y), and the independent variables(X) could be locational factors, property features, host characteristics, etc. This model is designed to depict how these variables affect Airbnb prices. The dataset that will be used to estimate the pricings will consist of 2000 observations of Airbnb listings in Cape Town.  
Regression Equation:
 Price=β0+β1dumhome+β2dumfemale+β3dummale+β4hostlist+β5avail365+β6minnights+β7numreviews+β8revpm+β9chappoint+β10clifhout+β11melkstrandvals+β12waterfront+e
Where:
β0: intercept ·
β1 – β12: coefficient of the independent variables
e: this is the error term
Description of Variables and Data:
1.	Dependent Variable:
•	Price: The price per night for each Airbnb listing (in Rand).
2.	Independent Variables:
•	dumhome: A dummy variable that will be used to differentiate between a home/apartment (1) and a room (0). 
•	dumfemale: A dummy variable that will be used to differentiate between a female host (1) and a male host or agency (0). 

•	dummale: A dummy variable that will be used to differentiate between a male host (1) and a female host or agency (0). 
•	hostlist: The number of listings managed by the host, which may indicate the professionalism of the host.
•	avail365: The number of days the listing is available per year, indicating its accessibility to guests.
•	minnights: The minimum number of nights required per booking, which might influence guest preferences.
•	numreviews: The total number of reviews received, reflecting the popularity of the listing.
•	revpm: The number of reviews received per month, indicating the recent activity of the listing.
•	Location Dummy Variables:
•	chappoint: Dummy variable for listings located in Chapmanspeak and Cape Point.
•	clifhout: Dummy variable for listings located in Clifton and Hout Bay.
•	melkstrandvals: Dummy variable for listings located in Melkbosstrand, Strand, and False Bay.
•	waterfront: Dummy variable for listings located at the Waterfront.
PRIORI EXPECTATIONS 
Host Characteristics
•	Hostlist
A host or agency managing multiple listings can be perceived as experienced and professional which can lead to higher booking on any of the hosts’ properties. This can result in the host increasing their prices across their properties due to the increase in demand. However, managing multiple listings can have a negative effect as it can reduce the service quality or lead hosts to reduce individual property prices to maximize occupancy thus, making owners of less listings charge more because their properties are more well maintained and personal. Hence the relationship between the price and hostlist can be seen as ambiguous or slightly positive.
•	Dumfemale and dummale 
Public opinion has shown that the hosts’ gender may have an influence on the trust and comfort levels of customers. In this case it is likely that female hosts will earn more than males due to the perception of increased safety, trustworthiness and hospitality. Therefore, the dumfemale variable is expected to have a positive relationship with price while dummale is expected to have a negative relationship.
Property Characteristics
•	Minnights 
 The minimum nights required variable is expected to have a slightly positive relationship with price. If a property has a long minimum stay quota this can increase their pricings as they would be attracting customers that are willing to pay more for longer term stays. 
•	Numreviews and revpm 
A high number of reviews per month or a day will generally lead to a higher perceived value unless the reviews are negative. Therefore, the relationship between the total number of reviews and the number of reviews per month is expected to be positive
•	Dumhome 
If the property is a home, it will be priced higher than a room as it has more privacy, more space for larger groups of people who are willing and prepared to pay a premium. The relationship between the dumhome variable and price is expected to be positive if the listed property is a home.
Location Indicators
•	Chappoint 
Chappoint relationship with price is expected to be positive because Cape point and Chapmanspeak are closer to tourist attractions and have beautiful views of nature making them likely to charge premium prices.
•	Clifhout
Clifhout relationship with price is expected to be strongly positive because Clifton and Hout Bay are both luxury destinations
•	Melkstrandvals 
Melkstrandvals relationship with price is expected to be slightly positive because Melkboostrand, Strand and False Bay may be located near the coast, but their demand might not be as high as places like Clifton and Hout Bay therefore their prices may be less than compared to the prime lux locations.
•	Waterfront 
Waterfront relationship with price is expected to be positive because it is the most popular tourist area. Due to its central location and its proximity to malls and entertainment properties situated in or near will charge high prices.




Regression Model Analysis
EViews Results and Analysis

