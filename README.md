# **UFO Sightings**

## Overview of Project

### Summary ### 
The objective of this project is to create and deploy a web page using some basic html programming and using JavaScript to provide a searchable table.
The goals are to:
* Deploy the [“UFO Sightings” web app](https://mrmarken.github.io/UFOs/) 
* Create four additional filters to search the UFO data
* Use JavaScript to allow users to use filters to view UFO data 

### Data Sources
The data sources to complete this project are outlined below:
* [UFO Data](https://github.com/mrmarken/UFOs/blob/main/static/js/data.js)
* [HTML Code](https://github.com/mrmarken/UFOs/blob/main/index.html)

### Software Used
Visual Studio Code Version: 1.70.2, JavaScript 1.5


## Results 
A filter was successfully added to the web app.  It allows the user to filter through UFO Sightings throughout the cities in the US and Canada.  The filters allow the user to use a set of five variables to narrow down their search.
* Date
* City
* State
* Country
* Shape of Sighting

### A Filter for Various Parameters
The following items have been completed as seen on the respective following screenshots:
 * The list element that creates the button is removed, and there are five list elements for filtering in the index.html file.

| ![Figure1](https://github.com/mrmarken/UFOs/blob/main/static/images/new_filters.png) |
| :---: |
| **Figure 1.** Filters Added |

 * The filterTable() function loops through all of the filters and keeps any data that matches the filter values.
 * The webpage filters the table correctly based on user input.

| ![Figure2](https://github.com/mrmarken/UFOs/blob/main/static/images/three_filters.png) |
| :---: |
| **Figure 2.** Three Filters in Action |


 * The updateFilters() function saves the element, value, and the id of the filter that was changed.
 * The event listener is modified to detect changes to each filter in the app.js file. 

| ![Figure3](https://github.com/mrmarken/UFOs/blob/main/static/images/filter_id_(console).png) |
| :---: |
| **Figure 3.** Console Output |

 
## Summary
This exercise culminated with a web page that allows users to filter through UFO Sightings data.  The user is able to use the filters to narrow down their search by date, state, city, country and shape of the observed flying anomaly.

### Limitation(s)
While this new function works well, there is one major limitation:
 * The filters are case sensitive and will not provide results if the incorrect lower case is not used.  For example, if we use “CA” instead of “ca” in the “State” field, no results will be shown:

| ![Figure4](https://github.com/mrmarken/UFOs/blob/main/static/images/case_sentitivyty.png) |
| :---: |
| **Figure 4.** Case Sensitivity |

### Recommendations
1. Add code that allows the input of case-insensitive entries (similar logic to [JavaScript — Double Equals vs. Triple Equals](https://codeburst.io/javascript-double-equals-vs-triple-equals-61d4ce5a121a))
2. Use more up-to-date public data to review UFO sightings (the data is currently limited to 2 weeks in January 2010 and only for US and two Canadian cities)
3. Link to other sites and/or publications that reference recent UFO sightings for a "latest news" approach
