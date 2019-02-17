[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kafonek/vast/master)

### Ocearch Shark data analysis

The [Ocearch site](https://www.ocearch.org/) compiles information about Shark locations by tagging individual sharks with trackers that 'ping' with their location.  There are hundreds of sharks tracked, and tens of thousands of locational pings in total.

This Binder-enabled Github repo offers three levels of challenges to analyze the Shark data.  


### Easy Challenge

The easy challenge offers you already-cleaned data and asks five questions that can be answered with basic Pandas methods.

Easy questions:

 1. How many total pings are in the Ocearch data?
 2. How many unique species of sharks are in the data set?
 3. What is the name, weight, and species of the heaviest shark?
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

The hard challenge asks you to pull and parse data from the Ocearch api directly before answering the Easy, Intermediate, and Hard questions.  The Hard questions will be added in a future date.

