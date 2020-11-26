# Data Biography

## Student Number: 19035452

---

### 1. Who collected the data?

Inside Airbnb collects the data, and it provides, compiles and analyzes public available information about a city's Airbnb's listings. Murray Cox founded this independent, non-commercial site.

---

### 2. Why did they collect it?

They look forward to the data’s completeness and accuracy and let people know about Airbnb were used in cities around the world well. They did some public analysis, discussion and community benefit. Because Airbnb rarely releases raw data and listings in a city that is usually within 10% of the correct number[1].

---

### 3. How was it collected?

Using python as source code scrapes data from the Airbnb web-site for London, and stores the result in a database system(PostgreSQL). Using some Open Source technologies(Crossfilter,Leaflet, Bootstrap, jQuery,etc.) utilizing public information from Airbnb and also "copied and pasted" from the internet for various uses[2]. After verified, cleansed, analyzed and aggregated, they completed data. Like their own “occupancy model”, which can be used to estimate how often an Airbnb listing is being rented out, and also approximate a listing's income.

---

### 4. What useful information does it contain?

Useful information includes real and reliable data that has been processed and can support some follow-up analysis. I divided these data into eight categories: house(name, description, neighborhood etc.), host(id,location,since etc.),facilities time, book, review, calculated_host and others. After sorting this effective information, we can find the information we need more quickly and accurately for different analyses.

Please click the link to view specific information: 

---

### 5. What useful information is it missing?

Missing means some columns that lack data are incomplete and structurally biased. Such as the column of license, a lot of data are blank, which means there is no information of housing certificates.
The column about host(response_rate, acceptance_ rate, about) is dropped. That means even if combined with other data, it is still impossible to analyze related issues.

---

### 6. To what extent is the data 'complete'?

Some elements look right but may in the wrong places，since data integrity should be viewed from different angles.

From the data source, although insideAirbnb data is relatively accurate, that doesn’t mean all official data are true. Airbnb hid over 1000 listings and misled the media, public and New York Government[3]. In some cases the total number of listings in a city is accurate within 10% or 20%[1]. 

Judging from the data content, the whole is complete but some are missing. First, some columns are structural missing #5. Second, some rows need to be cleaned, such as 3559 is NaN. Problems>7 are most likely to be problematic. Third, some key information lacks. In terms of reservation rules, customers do not know whether they need to provide a photo or phone number. And information about customers and review details, the policy of cancellation, house safety factor, surrounding traffic and so on also lack.

---

### 7. What kinds of analysis would this support?

Different data can be combined with each other for analyzing from different perspectives. The following analyzes are mainly from the company perspective.

First of all, the factor analysis of popular listings. By analyzing the characteristics of high-occupancy houses, reviewing situation, and hosts' situation, we can understand the reasons and factors of popularity. Second, it is easy to know the reasons why unpopular houses have not been selected for a long time. Third, predicting the rental situation in London of the next month, such as popular booking times and locations, will help Airbnb adjust its marketing strategy. Finally, when combined with other data, it can analysis  about impact on society, such as economy, housing prices and policies. For example, it can analyze the impact on the local economy and government, policies and environment on the occupancy of houses. 

Please click the link to view specific information: 

---

### 8. What kinds of analysis would it _not_ support?

Analysis that cannot be performed due to a lack of data structure: 
A lack of 'license', customers cannot make judgments about the safety of the house. They don't know whether the host really has the property rights of the house and whether the host has the lease condition.
A lack of information about the hosts(#5). For shared house customers, they cannot know more about hosts. For example, customers cannot use 'host_response_rate' to judge whether the landlord is enthusiastic person and willing to answer questions. It is also impossible to judge the landlord's low tolerance through low 'host_acceptance_rate'.

---

### 9. Which of the uses presented in Q.7 and Q.8 are _ethical_?

Although Airbnb advocates ‘sharing’, all premises are driven by profit.[4] Therefore, to get greater benefits,there are many ethical issues involved in data analysis. Below I will analyze from perspectives of individual, government and the public

First, when analyzing hosts and customers in #7, will use a lot of personal information that has been approved. Although self-managed privacy is laudable, it is rarely achieved. Because of ‘aggregation effect’, this makes it very hard to assess whether revealing any piece of information will sometime later on, when combined with other data, reveal something sensitive[5]. This is why we receive some harassing emails and phone calls, because of our age and asset status, all kinds of private information are exposed. In most cases, the risks outweigh the benefits.

Secondly, even if the use of personal information in #7 and #8 are within a reasonable range, data discrimination still exists. Hosts and guests will choose and reject each other based on their picture, race, religious belief, sexual orientation, etc. This means that this public information will put people at risk of discrimination.

Third, in the analysis of various factors of housing，house_type and listing in #7, although there are real internal data, in order to have better cooperation with the local government or explain social and economic issues such as housing price growth, there is also a risk of data tampering. In addition to the New York case mentioned above, similar cases have occurred many times in Paris, San Francisco and other places[1].

In conclusion, although some unethical behaviors can help some analysis to achieve the expected results, such behaviors that deceive the public and the media cannot help an enterprise obtain long-term benefits and good development.

---

### Reference

[1] T. Slee. 2019. “Airbnb Data Collection: Methodology and Accuracy.”[Online]
   Available:https://tomslee.net/airbnb-data-collection-methodology-and-accuracy 

[2] Cox. M. 2015.  “Inside Airbnb-Behind.” Inside Airbnb[Online]
    Available: https://insideairbnb.com/about.html
		
[3] Cox.M. and T. Slee. 2016. “How Airbnb’s Data Hid the Facts in New York City.” Inside Airbnb. 
    Available: http://insideairbnb.com/reports/how-airbnbs-data-hid-the-facts-in-new-york-city.pdf. 
		
[4] G.Quattrone, D.Proserpio, D.Quercia, L.Capra, M.Musolesi. 2016,Apr.“Who Benefits from the ‘Sharing’ Economy of Airbnb?”

[5] Crawford, K., and M. Finn. 2015. “The Limits of Crisis Data: Analytical and Ethical Challenges of Using Social and Mobile Data to Understand Disasters.” GeoJournal 80 (4): 491–502.

---
