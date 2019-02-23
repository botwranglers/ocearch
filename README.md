[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/botwranglers/ocearch/master)

### Ocearch Shark data analysis

The [Ocearch site](https://www.ocearch.org/) compiles information about Shark locations by tagging individual sharks with trackers that 'ping' with their location.  There are hundreds of sharks tracked, and tens of thousands of locational pings.

This Binder-enabled Github repo offers three levels of challenges to analyze the Shark data.  Click the "Launch Binder" badge on this page to launch a Jupyter instance with the Challenge notebooks on the MyBinder cloud.  The Jupyter instance offers Python3 and R kernels, as well as the jupyter-contrib-nbextensions with `toc2`, `ExecuteTime`, and `collapsible_headings` enabled.  For Python, it has `pandas`, `requests`, and `folium` pre-installed.  For R, it has `tidyverse` and `leaflet`.

Each challenge asks both harder questions and asks you to do more data cleaning.  If you want to skip the data cleaning and just try to tackle the harder questions, feel free to just read in `data/sharks_cleaned.csv` for each challenge.  


### Easy Challenge

The easy challenge uses already-cleaned data and asks five questions that can be answered with basic Pandas methods.

Easy questions:

 1. How many total pings are in the Ocearch shark data?
 2. How many unique species of sharks are in the data set?
 3. What is the name, weight, and species of the heaviest shark(s)?
 4. When and where was the very first ping?
 5. Excluding results with 0 distance traveled: what's the minimum, average, and maximum travel distances?


### Intermediate Challenge

The intermediate challenge uses data that needs some cleaning before being able to answer the Easy Challenge questions.  Furthermore, it asks five questions that require more complex analysis, in particular using `groupby`.

Intermediate questions:

 1. Which shark had the most pings?
 2. Which shark has been pinging the longest, and how long has that been?
 3. Which shark species has the most individual sharks tagged?
 4. What is the average length and weight of each shark species?
 5. Which shark has the biggest geographic box (largest distance from min lat/lon to max lat/lon, not dist_traveled)?
 
 
### Hard Challenge

The hard challenge makes a request straight to the Ocearch API, you'll have to parse the response and clean the data from there.  Along with answering the Easy and Intermediate questions, the Hard questions deal with time-series analysis, interpolating missing data, and plotting locations in an interactive map.

Hard questions:

 1. Use folium/leaflet to plot the first ping, last ping, and a line connecting each ping for the Tiger shark Emma.  Make the first ping marker a 'play' icon, and last ping icon a 'stop' icon.
 2. Resample Emma data to have a daily lat/lon average, and interpolate missing results.  Plot a marker for each day, and color them blue for hard data, green for interpolated lat/lons
 3. Resample all shark data for daily lat/lon averages, and interpolate missing results
 4. Calculate distance between Emma and other sharks on a daily basis
 5. Identify the shark that has the shortest average distance to Emma per day (minimum 50 days of pings with Emma)
 6. Plot Emma and her closest buddy: interpolated results for each in green, Emma as circle icons and her buddy as square icons

### Emma-shark

In the Hard challenge, you analyze the data for the shark named Emma.  Our own Jon Ainsworth dove with the team that tagged Emma, and captured some beautiful underwater video of Emma-shark. Check it out here: https://gfycat.com/jollybeautifulgalapagostortoise
