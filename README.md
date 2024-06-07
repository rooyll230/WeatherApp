# WeatherApp
# Weather Information App

This Java-based desktop application provides weather information for a given location using the OpenWeatherMap API. It displays current weather conditions and an 8-day weather forecast. Users can also switch between Celsius and Fahrenheit units and view their search history.

## Features

- Fetches current weather information for a specified location.
- Displays an 8-day weather forecast.
- Allows switching between Celsius and Fahrenheit units.
- Maintains a search history for quick access to previously searched locations.

## Prerequisites

- Java Development Kit (JDK) 8 or higher.
- OpenWeatherMap API key.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-repo/weather-app.git
    cd weather-app
    ```

2. Replace the `API_KEY` in `WeatherAPIService.java` with your OpenWeatherMap API key.

## Usage

1. Compile the Java files:
    ```sh
    javac WeatherApp.java WeatherAPIService.java
    ```

2. Run the application:
    ```sh
    java WeatherApp
    ```

## Class Descriptions

### `WeatherApp`

This class creates the GUI for the application using Swing. It includes:

- `locationField` for entering the location.
- `weatherInfoArea` for displaying current weather information.
- `iconLabel` for displaying weather icons.
- `forecastLabel` for displaying the weather forecast.
- `unitComboBox` for switching between Celsius and Fahrenheit.
- `searchHistoryList` for displaying the search history.

### `WeatherAPIService`

This class handles the API requests to the OpenWeatherMap API. It includes methods to:

- `getWeather(String location)`: Fetch current weather data for the specified location.
- `getForecast(String location)`: Fetch weather forecast data for the specified location.

## Example

Here is an example of the application in use:

1. Enter a location (e.g., "London") in the text field.
2. Click the "Search" button to fetch the weather data.
3. The current weather information will be displayed, including temperature, humidity, wind speed, and conditions.
4. The weather forecast will also be displayed below the current weather information.
5. Use the combo box to switch between Celsius and Fahrenheit units.
6. View previous searches in the search history list and double-click an entry to view its weather information again.

## Contributing

Feel free to fork the repository and submit pull requests for improvements and new features.

## License

This project is licensed under the MIT License.
