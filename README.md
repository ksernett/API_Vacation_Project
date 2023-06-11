# API Vacation Project
Utilizing two different API sources to collect information, identify ideal vacation spots based on weather and local hotels. 

### API Keys
Two API keys are needed for this project
1. The first will be used to collect weather data and can be created at https://openweathermap.org/
    - Once the key is generated it will need to be added to the Weather API key python file here: 'WeatherPy/weather_api_key.py'
2. The second will be used to find hotels and tourist attractions and can be created at https://www.geoapify.com/
    - Once the key is generated it will need to be added to the Geoapify API key python file here: 'VacationPy/geoapify_api_key.py'

#### Part 1: WeatherPy
- Using numpy and citypy, generate a list of cities to use for data extraction
- Connect to the OpenWeatherMap API and use JSON to parse out latitude, longitude, max temp, humidity, cloudiness, wind speed, country, and date for each city
- Export the data into a CSV for use in part 2

#### Part 2: VacationPy
- Read in the CSV data
- Plot the cities using hvplot
- Narrow down the cities based on 'ideal' weather conditions
- Connect to the Geoapify API to find a nearby hotel and restaurant; eliminate the options that do not have both
- Plot the final list of cities using hvplot
