Weather App
This is a simple Java application that fetches and displays weather information and forecasts using the OpenWeatherMap API. The application features a graphical user interface (GUI) built with Swing, allowing users to input a location and retrieve current weather details, as well as a five-day forecast.

Features
Current Weather Information: Displays temperature, humidity, wind speed, and weather conditions for a specified location.
Five-Day Forecast: Shows the weather forecast for the next five days.
Unit Selection: Users can choose between Celsius and Fahrenheit for temperature readings.
Search History: Keeps a log of previously searched locations.
Dynamic UI: Changes background and icons based on the time of day and weather conditions.
Prerequisites
Java Development Kit (JDK) 8 or later
Internet connection (to fetch data from the OpenWeatherMap API)
An API key from OpenWeatherMap (the default key is included in the code, but you should replace it with your own for production use).
Installation
Clone or download the repository to your local machine.
Navigate to the project directory.
Open the project in your preferred IDE (e.g., IntelliJ IDEA, Eclipse).
Ensure you have the necessary libraries (like JSON) in your classpath. You may need to add a JSON library such as org.json if it's not already included in your project.
Usage
Compile and run the WeatherAppGUI class.
Enter a location (city name) in the input box and click the "Search" button.
The current weather information and five-day forecast will be displayed in the GUI.
Code Structure
Packages
weatherapp: Contains the main application classes:
WeatherAPI: Handles API requests to fetch weather data.
SearchHistory: Manages the search history entries.
WeatherAppGUI: The graphical user interface for the application.
Important Classes
WeatherAPI: Contains methods to retrieve current weather and forecast data from the OpenWeatherMap API.

retrieveWeatherInfo(String location): Fetches current weather data for a given location.
fetchForecastData(String location): Fetches the five-day weather forecast for a given location.
SearchHistory: Represents a search entry, including the location and timestamp.

WeatherAppGUI: The main GUI class where the application components are initialized and event handling occurs.

Notes
The application fetches data from the OpenWeatherMap API, so make sure your API key has sufficient quota for requests.
The GUI layout is built using Java Swing's GridBagLayout for flexible component arrangement.
The weather icon and background change dynamically based on the weather conditions and time of day.
Troubleshooting
If you encounter issues retrieving weather data, ensure your API key is valid and you have an active internet connection.
Check for exceptions in the console for any runtime errors.
