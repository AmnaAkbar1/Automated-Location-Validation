# Automated-Location-Validation

# Overview
Increased reliance on services like Uber underscores the importance of gaining precise and accurate data of locations for seamless and enhanced customer experience. However, adding the locations manually poses a challenge to Uber Captains to precisely find the exact location of their passenger. In this report, I aim to present a solution to automate the process of adding the locations and validating them. The automation of location validation by means of web scraping will act as a catalyst ensuring accuracy, reliability and efficiency in Uber’s mapping services. This is a semester project, my groupmate for this project was Sana Farooq.

# Problem Statement
How can we automatically validate locations that are added manually: we also manually add certain locations that do not exist in maps platforms (Google maps etc) manually: this process is very manual, and we need ML algorithms to help us automate the process of validating the location manually.

# Introduction
With increased reliance on services like Uber, obtaining an accurate address of a location is vital as it plays a key role in efficiency of the application thereby improving user experience.However, adding new locations which are not listed to maps poses a significant challenge to the Uber Captain as it makes it difficult to find the passenger’s accurate location. In this paper we aim to discuss the solution proposed for the automation of adding new locations and validating them. Our primary goal is to create a system that is an amalgamation of advanced technology with data handling practices. Our system will gather details of locations by web scraping from sources like Facebook and integrating with platforms like Google Maps.

Web scraping allows us to gather data in a cost-effective manner from various sources available on the World Wide Web [1]. Social media websites like Facebook and Twitter are being increasingly used to capture geospatial data for data analysis. These websites have a specific structure which is useful for extracting relevant data which in our case is locations’ data [2]. Web-enabled data acquisition has empowered us to create a system which retrieves data from various Facebook pages and then compares the retrieved location with the existing location in the database and updates the location if it does not match. The ability to pinpoint the exact location of the passenger is crucial to Uber Captains to deliver a seamless experience. The current process of manual entry of locations is hampering Uber’s operational efficiency leading to frustration for both drivers and passengers. This problem when solved using web scraping will not only enhance the customer experience but also elevate the operational efficiency of Uber as web scraping will save time to gather accurate and precise data. Selenium WebDrivers are widely used to automate the process of retrieving data from Facebook and other social media platforms. Beautiful Soup is used to locate the area of interest on the webpage and thereby making it easier to record those for
further processing [3].

# Proposed Solution
![image](https://github.com/AmnaAkbar1/Automated-Location-Validation/assets/145672191/65cf3564-8b93-46aa-9046-0b0141c733a9)

![image](https://github.com/AmnaAkbar1/Automated-Location-Validation/assets/145672191/208a1a74-155e-47b8-9a96-bc80f88610ea)


The figure (Figure 2) above depicts the process followed by us to create a miniature version of the solution proposed to update and validate the locations of the businesses and other locations by web scraping Facebook. In the miniature version we have manually created a Google sheet read and stored in a DataFrame in which locations of certain offices, companies taken from Google are available and we want to validate whether on the particular locations the offices exist or have moved to some other location. Selenium’s WebDriver is used to parse the pagesof those particular offices and extract the information of their addresses. The extracted location is then compared to the location in the DataFrame. If the location matches no changes are made. If the address does not match, we update the address in the DataFrame.

# Business Benefits
By automating the validation of manually added locations, this project is expected to yield the following benefits:
● Improved Customer Experience: By obtaining accurate data of locations, we can increase customer satisfaction as it enables better service in booking a ride to a specific location as the Uber’s Captain will now be able to reach the address hassle free.
● Enhanced Accuracy and Reliability: Automated validation of location ensures that the data available on the Uber’s map is accurate and reliable.
● Improved Data Accuracy: Enhanced location validation will result in more accurate and reliable data for decision-making.
● Efficiency Gains: Reduced manual effort will lead to increased operational efficiency and cost savings.
● Competitive Advantage: Staying ahead in location data accuracy will give us a competitive edge in the market.

# Future Work
We aim to expand the scope of automated validation to cover a wide range of locations apart from offices and public places. We also aim to incorporate machine learning algorithms to refine the validation process and enhance accuracy. Moreover, real-time integration and dynamic updating mechanism for all locations, urban and rural, would fortify the reliability, accuracy and availability of the system.

# Conclusion
The project offers a strategic solution to the challenges faced in validating and adding new locations to map, within the context of Uber’s services. Web Scraping to retrieve the locations of data and validating them ensures accuracy and reliability. It helps validate whether the particular locations exist or have moved to some other location. It not only improves the operational efficiency of the company but also saves time. The outlined business benefits, encompassing improved customer satisfaction, enhanced data accuracy, and increased operational efficiency, underscore the transformative impact of automated location validation within service-driven industries. 

# References
[1]“Application of Web Scraping and Google API service to optimize convenience stores’ distribution | IEEE Conference Publication | IEEE Xplore,” ieeexplore.ieee.org. https://ieeexplore.ieee.org/abstract/document/7224841

[2]A. Brenning and S. Henn, “WEB SCRAPING: A PROMISING TOOL FOR GEOGRAPHIC DATA ACQUISITION A PREPRINT.” Accessed: Dec. 04, 2023. [Online]. Available: https://arxiv.org/pdf/2305.19893.pdf

[3]R. Morshedi, B. Graduate, B. Chu@wsp, E. Com, Huang, and L. Ivers, “Web Scraping: Applications in Infrastructure Planning,” 2019. Accessed: Dec. 04, 2023. [Online].Available: https://www.apas.org.au/files/conferences/2019/Web-ScrapingApplications-in-Infrastructure-Planning.pdf
