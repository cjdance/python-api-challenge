# python-api-challenge

## Description of WeatherPy

This project utilised the Open Weather API and the Google Places API to extract the current weather from a randomly generated set of latitudes and longitudes.

The latitudes and longitudes were run through the citipy library to locate the nearest city name which was then put through the Open Weather API in a series of requests where failed requests were removed from the results.

Using the current weather data, a series of scatter plots were generated to examine any correlation between the latitude of cities and the eather conditions they were experiencing.

## Description of VacationPy

The data generated in WeatherPy was then used as the coordinates for the gmaps library to generate heat maps based on humidity for the cities located in the API requests.

Using the Google Places API, it was then required to locate the nearest hotel within 5000m of the city coordinates, and return these in a separate column on the dataframe.

As an exercise, parameters for ideal holiday conditions were then set so that we could reduce the hotel dataframe down to between 5-10 cities and plot these over the heatmap in a marker layer containing the Hotel Name, City Name and Country Code from the Open Weather API data.
