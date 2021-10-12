# Analysis of Device Traffic to Wikipedia

## Goal of the Project

The goal of this project is to retrieve data from the Wikipedia API and transform that data into a workable timeseries set 
that will be used to visualize the changes in the number of users accessing Wikipedia over time.

## Data Source
[WikiMedia REST API](https://wikimedia.org/api/rest_v1/#/Pageviews%20data)  
[WikiMedia API Terms Of Use](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions)  

## Python Packages Used
notebook  
pandas  
matplotlib  
requests  
json  
datetime  

install in your CLI by running:  

`pip install {package_name}`

## Data Dictionary for en-wikipedia_traffic_200712-202108.csv

year: year in which number of users were counted in YYYY format  
month: number of month in which the number of users were counted in MM format  
pagecount_all_views: total number of views in that month recorded by Pagecount API  
pagecount_desktop_views: number of views in that month recorded by Pagecount API using a Desktop device  
pagecount_mobile_views: number of views in that month recorded by Pagecount API using a Mobile device  
pageview_all_views: total number of views in that month recorded by Pageview API  
pageview_desktop_views: number of views in that month recorded by Pageview API using a Desktop device  
pageview_mobile_views: number of views in that month recorded by Pageview API using a Mobile device  

## Other Considerations
* Data from the Pageview API excludes web crawlers, but the Pagecounts API does not. This means that the Pageview dataset has a more accurate count of real users of the site.
