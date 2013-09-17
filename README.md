Locator
=======

Locator is a JavaScript store/location locator script using Google Maps Javascript API v3, Google Geocoding API, and jQuery. 

# Live Demo

http://wheatdesign.com/demos/locator/

# Overview

* To use Locator, add your locations to the storeLocations array. The only requirement is that the last five characters of each array member must end in a five-digit zipcode. 
* By default, Locator matches the first three characters of the user-supplied zipcode. If you'd prefer an exact match, there's a section of code you can uncomment (and comment out the fuzzy match). 

# Lifecycle

Locator starts with the storeLocations array. When the user submits a zipcode, Locator checks the last five characters of each element in the storeLocations array against the user-submitted zipcode. Matches are pushed into resultsArray. 

Each item in resultsArray is then sent to the Google Geocoding API, which returns a latitude and longitude for each. These latitudes and longitudes are then sent to the Google Maps API, which plots them as markers, populating their titles and infowindows with the formatted address. 


