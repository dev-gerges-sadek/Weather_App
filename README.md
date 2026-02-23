 🌤 Weather App

A Flutter application that shows the **current weather** for any city using a public Weather API. Users can search for a city and get the temperature, weather condition, humidity, and more in a clean and responsive UI.

## Features

- Search for weather by city name
- Display temperature, weather condition, and humidity
- Show weather icon based on condition
- Clean and responsive UI
- Error handling for invalid city or API issues
- Uses a public Weather API

## Built With

- Flutter
- Dart
- http (for API requests)
- flutter_bloc or provider (optional for state management)
- flutter_screenutil (optional for responsive UI)
- cupertino_icons


## Screens Overview



### HomeScreen
- Search bar to enter city name
- Displays current temperature, weather condition, humidity, and icon
- Updates automatically when searching a new city

### WeatherDetailScreen
- Optional screen for more detailed info like wind speed, pressure, sunrise & sunset

## Getting Started

This project uses a Weather API. You need an API key from [OpenWeatherMap](https://openweathermap.org/api) or any public weather API.

Steps to Run:

1. Clone the repository:
   git clone https://github.com/your-username/weather_app.git
2. Navigate to the project folder:
   cd weather_app
3. Install dependencies:
   flutter pub get
4. Add your API key in `weather_service.dart` or `.env` file (depending on implementation)
5. Run the app:
   flutter run

## Example API Usage

```dart
// Example call in weather_service.dart
final response = await http.get(Uri.parse("https://api.openweathermap.org/data/2.5/weather?q=$city&appid=YOUR_API_KEY"));


