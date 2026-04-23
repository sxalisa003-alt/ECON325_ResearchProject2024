# ECON325_ResearchProject2024


## Table of Contents

1. [Introduction](#introduction)  
2. [Literature Review](#literature-review)  
   - [Hedonic Pricing and Property Features](#hedonic-pricing-and-property-features)  
   - [Factors Specific to Host and Platform](#factors-specific-to-host-and-platform)  
   - [Market Saturation and Competition](#market-saturation-and-competition)  
3. [Model Specification and Data Description](#model-specification-and-data-description)  
   - [Description of Variables and Data](#description-of-variables-and-data)  
4. [Priori Expectations](#priori-expectations)  
   - [Host Characteristics](#host-characteristics)  
   - [Property Characteristics](#property-characteristics)  
   - [Location Indicators](#location-indicators)  
5. [Regression Model Analysis](#regression-model-analysis)  
   - [EViews Results and Analysis](#eviews-results-and-analysis)  
   - [Coefficient Interpretation and Evaluation](#coefficient-interpretation-and-evaluation)  
   - [P-Value Interpretation](#p-value-interpretation)  
   - [R-Squared, Adjusted R-Squared and F-Statistic Interpretation](#r-squared-adjusted-r-squared-and-f-statistic-interpretation)  
6. [Interactive Term Regression Model](#interactive-term-regression-model)  
   - [Coefficient Interpretation](#coefficient-interpretation)  
   - [P-Value](#p-value)  
   - [R-Squared, Adjusted R-Squared and F-Statistic Interpretation](#r-squared-adjusted-r-squared-and-f-statistic-interpretation-1)  
7. [Conclusion](#conclusion)  
8. [Recommendations](#recommendations)  
9. [Reference List](#reference-list)  

 
## Introduction

Airbnb, launched in 2008, is a digital marketplace that connects people who want to rent out their properties with people who are seeking to book accommodation for a short-term. The introduction of a digital marketplace has brought about a big evolution in the hospitality industry, transforming it from a traditional and rigid structure to a more flexible, peer-to-peer, and personalised structure. This evolution has changed the way accommodation services are being offered to tourists worldwide. The Cape Town tourism and hospitality industry has seen an influx of tourists ever since Airbnb was introduced to the city. However, the pricing dynamics of Airbnb have proven to be a challenge for hosts as they must consider a multitude of elements such as amenities, location advantages and disadvantages, and current prevailing local market trends to determine the rental rates effectively. This research report seeks to establish the aspects that impose the prices of Airbnb’s in Cape Town by investigating the factors that influence those prices using econometric models to explain variation in prices.

It is most critical that we understand the elements that influence the pricing of Airbnb’s in Cape Town, not only for the benefit of hosts who are seeking to maximise their profits but also for tourists who seek to find the best holiday destination at the most affordable price. This research utilises economic theories such as the hedonic pricing model, which, according to Montero and Fernández-Avilé (2023) is an economic model that suggests that the pricing of a good is dependent on its characteristics. It will also use econometric techniques to analyse an Airbnb dataset for Cape Town listings to estimate the relationship between various independent variables and the dependent variable (Price). 
The significance of this study lies in firstly providing insights into the pricing strategies within the short-term rental market, which can better inform hosts’ pricing tactics. Secondly, the results of this study can aid in having more informed discussions on the factors that influence Airbnb prices. Furthermore, pave way to making recommendations to improve rental and pricing strategies.

## LITERATURE REVIEW

#### <ins>Hedonic Pricing and Property Features</ins>

Using the hedonic pricing theory this study suggests that the prices of Airbnb’s are influenced by a variety of property-specific characteristics like amenities, listing type (room or home), parking, Wi-Fi, etc and external factors such as neighbourhood safety and proximity to attractions and commercial centres. A study conducted by Wen et al. (2021) has proved that elements like guest reviews and host reputation play a significant role in the price determination of Airbnb listings. Wen et al. (2021) also discovered that host comments, booking history and the “superhost” status can have a positive impact on the pricing as these attributes could be seen as high-quality service.
Research conducted by Zhang et al. (2019) shows that spatial features like proximity to tourist spots, commercial areas, and access to public transport play a significant role in price determination. These findings are relevant to Cape Town due to its dependence on tourism.

#### <ins>Factors specific to the host and platform</ins>

According to Teubner et al. (2017), trust indicators such as verified identity, positive reviews, high quality images of the Airbnb space have a huge impact on Airbnb rates. The study provides support for Ert et al. (2016) findings, which reported that a guest willing to pay more can also depend on the reputation of the host. This means that when customers are looking for accommodation, they also consider the hosts’ reputation as well as the property itself.

#### <ins>Market Saturation and Competition</ins>

In the context of the Cape Town market, supply and demand will have a role in the price determination process due to how competitive the Airbnb market has become. According to Zervas et al. (2017), properties that are in regions that have high Airbnb bookings are subjected to lower pricing because the market in that region is too competitive. This is essentially true for Cape Town, where the Airbnb market is rapidly increasing, leading to market saturation.

## MODEL SPECIFICATION AND DATA DESCRIPTION

To estimate the determinants of Airbnb prices in Cape Town this study will make use of a multiple linear regression model and an interactive term regression model. Price will be the dependent variable (Y), and the independent variables(X) could be locational factors, property features, host characteristics, etc. This model is designed to depict how these variables affect Airbnb prices. The dataset that will be used to estimate the pricings will consist of 2000 observations of Airbnb listings in Cape Town.  

#### <ins>Regression Equation</ins>:

 Price=β0+β1dumhome+β2dumfemale+β3dummale+β4hostlist+β5avail365+β6minnights+β7numreviews+β8revpm+β9chappoint+β10clifhout+β11melkstrandvals+β12waterfront+e
 
Where:
       * β0: intercept 
       * β1 – β12: coefficient of the independent variables
       * e: this is the error term

<ins>Description of Variables and Data</ins>

1.	Dependent Variable

   *	Price: The price per night for each Airbnb listing (in Rand).
     
2.	Independent Variables:
   
  *	dumhome: A dummy variable that will be used to differentiate between a home/apartment (1) and a room (0). 
  *	dumfemale: A dummy variable that will be used to differentiate between a female host (1) and a male host or agency (0). 
  *	dummale: A dummy variable that will be used to differentiate between a male host (1) and a female host or agency (0).	
  *	hostlist: The number of listings managed by the host, which may indicate the professionalism of the host.
  *	avail365: The number of days the listing is available per year, indicating its accessibility to guests.
  *	minnights: The minimum number of nights required per booking, which might influence guest preferences.
  *	numreviews: The total number of reviews received, reflecting the popularity of the listing. 
  *	revpm: The number of reviews received per month, indicating the recent activity of the listing.
    
3. Location Dummy Variables:
   
  *	chappoint: Dummy variable for listings located in Chapmanspeak and Cape Point.
  *	clifhout: Dummy variable for listings located in Clifton and Hout Bay.
  *	melkstrandvals: Dummy variable for listings located in Melkbosstrand, Strand, and False Bay.
  *	waterfront: Dummy variable for listings located at the Waterfront.

## PRIORI EXPECTATIONS 

<ins>Host Characteristics<ins>

*	Hostlist
A host or agency managing multiple listings can be perceived as experienced and professional which can lead to higher booking on any of the hosts’ properties. This can result in the host increasing their prices across their properties due to the increase in demand. However, managing multiple listings can have a negative effect as it can reduce the service quality or lead hosts to reduce individual property prices to maximize occupancy thus, making owners of less listings charge more because their properties are more well maintained and personal. Hence the relationship between the price and hostlist can be seen as ambiguous or slightly positive.

*	Dumfemale and dummale 
Public opinion has shown that the hosts’ gender may have an influence on the trust and comfort levels of customers. In this case it is likely that female hosts will earn more than males due to the perception of increased safety, trustworthiness and hospitality. Therefore, the dumfemale variable is expected to have a positive relationship with price while dummale is expected to have a negative relationship.

<ins>Property Characteristics</ins>

*	Minnights 
 The minimum nights required variable is expected to have a slightly positive relationship with price. If a property has a long minimum stay quota this can increase their pricings as they would be attracting customers that are willing to pay more for longer term stays.

*	Numreviews and revpm 
A high number of reviews per month or a day will generally lead to a higher perceived value unless the reviews are negative. Therefore, the relationship between the total number of reviews and the number of reviews per month is expected to be positive

*	Dumhome 
If the property is a home, it will be priced higher than a room as it has more privacy, more space for larger groups of people who are willing and prepared to pay a premium. The relationship between the dumhome variable and price is expected to be positive if the listed property is a home.

<ins>Location Indicators</ins>

*	Chappoint 
Chappoint relationship with price is expected to be positive because Cape point and Chapmanspeak are closer to tourist attractions and have beautiful views of nature making them likely to charge premium prices.

*	Clifhout
Clifhout relationship with price is expected to be strongly positive because Clifton and Hout Bay are both luxury destinations

* Melkstrandvals 
Melkstrandvals relationship with price is expected to be slightly positive because Melkboostrand, Strand and False Bay may be located near the coast, but their demand might not be as high as places like Clifton and Hout Bay therefore their prices may be less than compared to the prime lux locations.

*	Waterfront 
Waterfront relationship with price is expected to be positive because it is the most popular tourist area. Due to its central location and its proximity to malls and entertainment properties situated in or near will charge high prices.


## Regression Model Analysis
EViews Results and Analysis


<ins>Estimated Regression Equation</ins>

Price=β0+β1dumhome+β2dumfemale+β3dummale-β4hostlist+β5avail365+β6minnights+β7numreviews-β8revpm+β9chappoint+β10clifhout+β11melkstrandvals+β12waterfront+e

Price=1254.09+1088.98dumhome+191.78dumfemale-105.18dummale-2.87hostlist-1.44avail365+19.06minnights+0.43numreviews-332.33revpm+517.95chappoint+1018.97clifhout+88.12melkstrandvals+70.25waterfront+e

<ins>Coefficient Interpretation and Evaluation</ins>

 * Intercept(β0=1254.09): The intercept indicates that the base price rate per night is R1254.09 when all independent variables are equal to zero. 

 * Dumhome(β1=1088.98): For every additional home/apartment listed the prices of Airbnb’s in Cape Town increase by R1088.98, ceteris paribus

 * Dumfemale(β2=191.78): Females charge R191.78 more than males and agencies, ceteris paribus.

 * Dummale(β3=105.18): Males charge R105.18 less than females and agencies, ceteris paribus.

 * Hostlist(β4=2.87): For every additional property managed by a host the pricing of Airbnb’s decreases by R2.87, ceteris paribus.

 * Avail365(β5=1.44): For every additional day a property is available throughout the year the price of an Airbnb decreases by R1.44, ceteris paribus.

 * Minnights(β6=19.06): The longer the minimum nights required for a booking the price of Airbnb’s increases by R19.06, ceteris paribus.

 * Numreviews(β7=0.43): For every additional review on a property the prices of Airbnb’s increases by R0.43, ceteris paribus.

 * Revpm(β8=332.33): For every additional review a month on a property the price decreases by R332.33.

**Chappoint(β9=517.95)** : A property located in either Chapmanspeak or Cape Point they will charge R517.95 more than inland properties, ceteris paribus 

**Clifhout(β10=1018.97)** : A property located in either Clifton or Hout Bay the host can charge R1018.97 more than inland properties, ceteris paribus

**Melkstrandvals(β11=88.12)** : A property located in either Melkboostrand, Strand and False Bay the host can charge R88.12 more than inland properties, ceteris paribus
 
**Waterfront (β12=70.25)** : A property located in Waterfront the host can charge R70.25 more than inland properties, ceteris paribus.
 
Before running a regression an increase in revpm was expected to lead to an increase in Airbnb prices. The assumption was based on the idea that a high number of reviews would be an indicator of high demand and popularity. The difference between the priori expectation and the regression results could be a result of variable omission 

### P-Value Interpretation

<ins>Statistically Insignificant Variables</ins>: Waterfront, Numreviews, Minnights, Melkstrandvals, Hostlist, Dummale, and Dumfemale

The p-value is higher than the acceptable 5% therefore the dumfemale variable is statistically insignificant. Do not reject the H0, there is insufficient evidence that these variables have impact on the prices.

<ins>Statistically Significant</ins>: Revpm, Dumhome, Clifhout, Chappoint, Avail364

The p-value is lower than the acceptable 5% therefore the dumhome variable is statistically significant. Reject the H0, the variables have a positive significant impact on price.

<ins>R-Squared, Adjusted R-Squared and F-Statistic Interpretation</ins>

R-squared (0.093) indicates that approximately 9.3% of the variation in Airbnb prices is explained by the model. Adjusted R-squared (0.086) indicates that approximately 8.6% of the variation in Airbnb prices is explained by the model. The model does not capture much of the variation in price.

F-Statistic (0.00%) therefore reject H0, and the model is statistically significantly.

Overall, the model is statistically significant but explain little of the variation in price and only a few independent variables are statistically significant.

### <ins>Interactive Term Regression Model</ins>

This study will also investigate the interaction between dummy variables and other variables, this is done to capture more nuanced effects that a single variable alone may not be able to explain. 

<ins>Regression equation with interactive dummies</ins>

Price=β0+β1dumhome+β2dumfemale+β3dummale+β4hostlist+β5avail365+β6minnights+β7numreviews+β8revpm+β9chappoint+β10clifhout+β11melkstrandvals+β12waterfront+β13(dumfeamle×revpm) +β14(dummale×hostlist) +β15(Dumhome×minnights) +β16(waterfront×avail365) +e

Where:

 * dumfeamle×revpm=Female_Reviews

 * dummale×hostlist=Male_Host
 
 * Dumhome×minnights=Home_Nights
 
 * waterfront×avail365=Water_Avail365
 
**dumfemale×revpm:**  measures how much the relationship between price and revpm varies depending on the host’s gender. 

**dummale×hostlist:**  measures the relationship between price and hostlist depending on the host’s gender.

**dumhome×minnights:** measures the relationship between the minimum nights required and price depending on whether the listing is an apartment/home or not.

**waterfront×avail365:**  measures the relationship of a listing’s availability throughout the year and price if the listing is in Waterfront.




### <ins>Estimated Regression Equation</ins>
Price=1306.89+805.55dumhome+699.90dumfemale+102.31dummale-0.46hostlist-1.77avail365-140.58minnights+10.88numreviews-237.06revpm+579.36chappoint+1025.15clifhout+73.59melkstrandvals-374.62waterfront-352.36(dumfemale×revpm) -9.08(dummale×hostlist) +161.42(dumhome×minnights) +1.96(waterfront×avail365) +e

### <ins>Coefficient Interpretation</ins>

 * Intercept(β0=1306.89): The intercept indicates that the base price rate per night is R1254.09 when all independent variables and interactive terms are equal to zero. 

 * Dumhome(β1=805.55): If the listing is a home or apartment, the price will increase by R805.55, ceteris paribus. 

 * Dumfemale(β2=699.90): Females charge R69.90 more than males and agencies, ceteris paribus.

 * Dummale(β3=102.31): Males charge R102.31 less than females and agencies, ceteris paribus.

 * Hostlist(β4=0.46): For every additional property managed by a host the pricing of Airbnb’s decreases by R0.46, ceteris paribus.

 * Avail365(β5=1.77): For every additional day a property is available throughout the year the price of an Airbnb decreases by R1.77, ceteris paribus.

 * Minnights(β6=140.58): For every additional night required for a booking the price of Airbnb’s increases by R140.58, ceteris paribus

 * Numreviews(β7=10.88): For every additional review on a property the prices of Airbnb’s increases by R10.88, ceteris paribus.

 * Revpm(β8=237.06): For every additional review a month on a property the price decreases by R237.06.

 * Chappoint(β9=579.36): A property located in either Chap or point they will charge R579.36 more than inland properties, ceteris paribus

 * Clifhout(β10=1025.15): A property located in either Clifton or Hout Bay the host can charge R1025.15 more than inland properties, ceteris paribus

 *  Melkstrandvals(β11=73.59): A property located in either Melkboostrand, Strand and False Bay the host can charge R73.59 more than inland properties, ceteris paribus.
 
 *  Waterfront (β12=374.62): A property located in Waterfront the host can charge R7374.62 less than inland properties, ceteris paribus.
 
 * Dumfemale×revpm(β13=352.36): If the host is a female and the reviews per month increase then the price charged by female hosts will increase by 352.36 more than male hosts or agencies.

 * Dummale×hostlist(β14=9.08): If the male host has multiple listings the prices, they charge will decrease by R9.08 less that female hosts or agencies

 * Dumhome×minnights(β15=161.42): If the listing is a home, then for every increase in the minimum nights required the price will increase by R161.42, ceteris paribus.

 * Waterfront×Avail365(β16=1.96): If the listing is in Waterfront the higher it’s availability throughout the year the price of the listing increases by R1.96, ceteris paribus.

## <ins>P-Value</ins>
<ins> Statistically Insignificant Variables</ins> : Waterfront, Numreviews, Minnights, Melkstrandvals, Hostlist, dummale, dumhome×minnights, dummale×hostlist, Revpm, waterfront×avail365

The p-value is higher than the acceptable 5% therefore the dumfemale variable is statistically insignificant. Do not reject the H0, there is insufficient evidence that these variables have impact on the prices.
<ins>Statistically Significant</ins>: Dumfemale, Dumhome, Clifhout, Chappoint, Avail365, Dumfemale×revpm
The p-value is lower than the acceptable 5% therefore the dumhome variable is statistically significant. Reject the H0, the variables have a positive significant impact on price.

***R-Squared, Adjusted R-Squared and F-Statistic Interpretation***

R-squared (0.1037) indicates that approximately 10.37% of the variation in Airbnb prices is explained by the model. Adjusted R-squared (0.0937) indicates that approximately 9.37% of the variation in Airbnb prices is explained by the model. The model does not capture much of the variation in price.
F-Statistic (0.00%) therefore reject H0, and the model is statistically significantly.
Overall, the model is statistically significant but explain little of the variation in price and only a few independent variables are statistically significant.

## <ins>Conclusion</ins> 

Models used to investigate the determinants of Airbnb price are both statistically significant, yet the r-squared values of both models suggest that the models are ill-fitting or that they can only account for a small portion of the variation in price. The failure to explain the variation in price could be due to the omission of important variables that may have an impact on prices or the presence of nonlinearity between variables or a weak relationship between price and independent variables. The inclusion of interactive terms has not improved the results as expected, because the model itself poorly explains the variation in price.

### <ins>Recommendations</ins>

*	The model can be redefined by removing insignificant variables from the model to limit the distorting effect such variables cause.
*	Check if there is multicollinearity between the variables because the presence of multicollinearity can inflate variable coefficients.
*	More relevant and important variables that affect the prices must be added e.g., seasonal pricing trends, neighbourhood safety rate, market demand, etc.
*	A survey can be conducted among travellers, and they can indicate what they look for when they book accommodation and what amenities or features are they willing to pay extra on.
  
In conclusion, the model is incomplete or underfitting and for future studies the model should be refined by adding more relevant and nuanced variables, use alternative modelling techniques that support the exploration of non-linear relationships to better capture and explain the complexity of the pricing strategy in Airbnb listings.


## <ins>Reference List</ins> 
Montero, JM., Fernández-Avilés, G. 2023. Hedonic Price Model. In: Maggino, F. (eds) Encyclopaedia of Quality of Life and Well-Being Research. https://doi.org/10.1007/978-3-031-17299-1_1279  date of access: 27 Sep.2024

Ert, E., Fleischer, A., & Magen, N.2016. Trust and reputation in the sharing economy: The role of personal photos in Airbnb. Tourism Management, 55: 62-73.

Teubner, T., Hawlitschek, F., & Dann, D. 2017. Price determinants on Airbnb: How reputation pays off in the sharing economy. Journal of Self-Governance and Management Economics, 5(3):53-80.

 Wen, H., Xie, K., & Ye, S. 2021. Airbnb pricing determinants: Beyond property characteristics. Journal of Hospitality & Tourism Research, 45(3):404-421.
 
Zhang, L., Wang, Y., & Li, H.2019. Spatial determinants of Airbnb prices in Beijing: A hedonic pricing model. International Journal of Hospitality Management, 79:103-113.

 Zervas, G., Proserpio, D., & Byers, J.W. 2017. The rise of the sharing economy: Estimating the impact of Airbnb on the hotel industry. Journal of Marketing Research, 54(5):687-705. 
  


