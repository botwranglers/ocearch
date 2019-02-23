[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/botwranglers/ocearch/master)

### Ocearch Shark data analysis

The [Ocearch site](https://www.ocearch.org/) compiles information about Shark locations by tagging individual sharks with trackers that 'ping' with their location.  There are hundreds of sharks tracked, and tens of thousands of locational pings in total.

This Binder-enabled Github repo offers three levels of challenges to analyze the Shark data.  Click the "Launch Binder" badge on this page to launch a Jupyter instance with the Challenge notebooks on the MyBinder cloud.  

Each challenge asks both harder questions and asks you to do more data cleaning.  If you want to skip the data cleaning, feel free to just read in `data/sharks_cleaned.csv` and use that to answer the intermediate and hard questions. 


### Easy Challenge

The easy challenge offers you already-cleaned data and asks five questions that can be answered with basic Pandas methods.

Easy questions:

 1. How many total pings are in the Ocearch shark data?
 2. How many unique species of sharks are in the data set?
 3. What is the name, weight, and species of the heaviest shark(s)?
 4. When and where was the very first ping?
 5. Excluding results with 0 distance traveled: what's the minimum, average, and maximum travel distances?


### Intermediate Challenge

The intermediate challenge forces you to do some data cleaning before being able to answer the Easy Challenge questions, and asks five more questions that require more complex Pandas methods, in particular using `groupby`.

Intermediate questions:

 1. Which shark had the most pings?
 2. Which shark has been pinging the longest, and how long has that been?
 3. Which shark species has the most individual sharks tagged?
 4. What is the average length and weight of each shark species?
 5. Which shark has the biggest geographic box (largest distance from min lat/lon to max lat/lon, not dist_traveled)?
 
 
### Hard Challenge

The hard challenge forces you to read data straight from the Ocearch API and transform it into useful, cleaned data.  It asks challenging questions that involve timeseries and geolocation analysis, as well as using `folium` for visualization.

Hard questions:

 1. Use folium to plot the first ping, last ping, and a line connecting each ping for the Tiger shark Emma.  Make the first ping marker a 'play' icon, and last ping icon a 'stop' icon.
 2. Resample Emma data to have a daily lat/lon average, and interpolate missing results.  Plot a marker for each day, and color them blue for hard data, green for interpolated lat/lons
 3. Resample all shark data for daily lat/lon averages, and interpolate missing results
 4. Calculate distance between Emma and other sharks on a daily basis
 5. Identify the shark that has the shortest average distance to Emma per day (minimum 50 days of pings with Emma)
 6. Plot Emma and her closest buddy: interpolated results for each in green, Emma as circle icons and her buddy as square icons

### Emma-shark

In the Hard challenge, you analyze the data for the shark named Emma.  Our own Jon Ainsworth dove with the team that tagged Emma, and captured some beautiful underwater video of Emma-shark.  Check out a gif of one of his videos here: https://gfycat.com/jollybeautifulgalapagostortoise