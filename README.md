# WEATHER-WEB-APPLICATION

## OVERVIEW

This project is a Weather Web Application that allows users to check the current weather conditions of various countries/cities. The application utilizes the OpenWeatherMap API to fetch real-time weather data and displays it in a user-friendly format.

## PREREQUISITES

Make sure you have account on [OpenWeatherMap website](https://openweathermap.org/)

Internet connection to fetch real-time weather data from the OpenWeatherMap API. Web browser to run the application.

## SCREENSHOT

![USER INTERFACE](/USER%20INTERFACE.png)

## FEATURES

The features of this Weather Web Application are as follows:

1. **Current Weather Information:** The application provides real-time weather information for multiple cities, including the current temperature, humidity percentage, and wind speed.

2. **City/Country Selection:** Users can search for weather data for a specific country/city of their choice. The application allows them to enter the name of the country/city they want to check the weather for.

3. **Dynamic Weather Icons:** The application dynamically displays weather icons based on the current weather conditions, such as rain, clouds, clear sky, drizzle, mist, and snow. These icons visually represent the weather status for each country/city.

4. **Error Handling and Local Storage:** The application incorporates error handling for API calls. If the API call fails due to internet connection issues, it displays an error message. In such cases, the application falls back to using the last saved weather data from local storage to ensure a smooth user experience.

5. **Responsive Design:** The web application is designed with responsive CSS, ensuring that it adapts and displays properly on various devices, including desktops, tablets, and mobile phones.

## GETTING STARTED

To get started with the Weather App, follow these steps:

1. Clone the repository: `git clone https://github.com/MehmoodSheikh/WEATHER-WEB-APPLICATION.git`
   
2. Open the project directory.
   
3. Launch the app by opening the `main.html` file in a web browser.
   
4. On the main page, you will see weather cards displaying weather information for three default cities (London, London, and London). The information includes the 
   city name, temperature in Celsius, humidity percentage, and wind speed in km/hr. The weather icon in each card visually represents the current weather 
   conditions.
   
5. To view weather information for a different city:

    A. Locate the search input field on the top-center weather card of the page.
   
    B. Enter the name of the city you want to check the weather for.
   
    C. Click the search icon.
   
    D. A new tab will open, displaying the `weather.html` page with weather information for the specified city.
   
7. On the weather.html page:

    A. The page will display detailed weather information for the searched city, including the city name, temperature, humidity, and wind speed.
   
    B. The weather icon will visually represent the current weather conditions.
   
9. If the API call fails due to internet connection issues, the application will display the last saved weather data from local storage.
    
10. If no data is available in local storage, an error message will be shown.

## CONFIGURATION

To configure the app, you need to provide an API key from OpenWeatherMap. Follow these steps:

1. **Sign Up for a New API:** Choose an alternative weather API that suits your needs. Many weather APIs offer free or paid plans with different levels of access and features. Sign up for an account on the chosen API provider's website to obtain an API key.

2. **Replace the API Key:** Once you have the API key from your new weather API provider, locate the getWeatherData function in the app.js file of your project.

3. **Update API Endpoint:** In the $.ajax call within the getWeatherData function, replace the existing API endpoint URL with the endpoint URL provided by your new weather API provider. The URL should point to the API's weather data endpoint.

4. **Update the appid Parameter:** Inside the $.ajax call within the getWeatherData function, find the data object that contains the parameters being sent to the API. Look for the appid property and replace its value with the new API key you obtained from the new API provider.

    The code snippet should look like this:
    
    ```javascript
    data: {
        q: city,
        units: "metric",
        appid: "YOUR_NEW_API_KEY_HERE" // Replace with your new API key
    },
    ```
    
## TECHNOLIGIES USED

HTML
CSS
JavaScript
jQuery
OpenWeatherMap API

## CREDITS

Weather icons from Iconfinder
jQuery library from jQuery
Weather data powered by OpenWeatherMap

## LICENSE

This project is licensed under the MIT License.

## ACKNOWLEDGEMENTS

Special thanks to the developers of the jQuery library, OpenWeatherMap API, and Iconfinder for providing valuable resources to create this web application.

