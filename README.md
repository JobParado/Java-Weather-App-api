
# Java Weather API GUI

## Overview

This project is a Java-based graphical user interface (GUI) application that retrieves and displays real-time weather data for a user-specified city. It uses a public weather API to fetch data such as temperature, humidity, pressure, wind speed, cloudiness, visibility, sunrise, and sunset times.

The application demonstrates how to:
- Build a simple GUI using Java Swing
- Integrate with a RESTful API
- Parse JSON responses
- Securely manage API keys using `.env` files and the `dotenv` library

---

## Features

- Input field for city name
- Displays weather data including:
  - Temperature and "feels like" temperature
  - Humidity, pressure, wind speed
  - Cloudiness, visibility, sunrise and sunset times
- Error handling for invalid city names or API failures
- Confirmation message on successful data retrieval

---

## Technologies Used

- Java (JDK 24)
- Netbeans IDE 25
- Swing (GUI)
- `org.json` for JSON parsing
- `dotenv-java` for environment variable management
- OpenWeatherMap API (or similar)

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/java-weather-api-gui.git
cd java-weather-api-gui
```


## How the API Call Works

The application sends a GET request to the weather API using the city name entered by the user. The response is parsed and displayed in the GUI.

Example endpoint:

```
https://api.openweathermap.org/data/2.5/weather?q=USA&appid=your_api_key&units=metric
```

The response is parsed using `org.json.JSONObject`, and relevant fields are extracted and displayed.

---

## Learning Focus: Handling APIs with `.env`

This project is designed to help you learn:
- How to integrate external APIs into a Java application
- Why storing API keys in `.env` files improves security
- How to use the `dotenv-java` library to access environment variables
- How to structure your code to separate logic, UI, and configuration

---

## License

This project is open-source under the MIT License.

---

