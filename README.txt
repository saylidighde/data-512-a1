README

Goal of the project
The goal of this project is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through September 30 2018, while following the best practices for open scientific research in design and implementation, and making it fully reproducible.
I have combined data about Wikipedia page traffic from two different Wikimedia REST API endpoints into a single dataset, performed some simple data processing steps on the data, and then analyzed that data.

License of the source data and a link to the Wikimedia Foundation REST API terms of use:
https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions

Link to API documentation
Wikimedia Legacy Pagecounts API : [https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)
Wikimedia Pageviews API : [https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)

Description of the values of all fields in the final data file.
The final data is stored in the csv file named en_wikipedia_traffic_200801-201809.csv

Column				Value
year				YYYY
month				MM
pagecount_all_views		num_views
pagecount_desktop_views		num_views
pagecount_mobile_views		num_views
pageview_all_views		num_views
pageview_desktop_views		num_views
pageview_mobile_views		num_views
	
Special notes for researchers
The data from the Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not. The period between mid-2015 till mid-2016 shows the overlapping traffic data between the two APIs. The overlap period can be seen from the surge in the plot.