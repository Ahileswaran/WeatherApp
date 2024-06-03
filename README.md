# WeatherApp

## Features
- Displays current latitude and longitude in decimal degrees format.
- Shows the reverse geo-coded address of your location.
- Displays the current system time.
- Provides weather information including temperature, humidity, and weather description.

## Setup Instructions
1. **Clone the Repository:**
   ```sh
   git clone https://github.com/your-username/WeatherApp.git


Explanation :

1. Package and Imports
    The package and necessary imports are included to handle location services, networking, and JSON parsing.

3. Class Declaration
    MainActivity extends AppCompatActivity.

3. Fields
    FusedLocationProviderClient fusedLocationClient: Used to access the device's location.
    TextView fields: Used to display latitude, longitude, address, time, temperature, humidity, and weather description.

4. onCreate Method
    Initialization: Sets the content view and initializes TextView fields.
    Location Services: Initializes the FusedLocationProviderClient and calls getLocation() to start the process of getting location data.

5. getLocation Method
    Permission Check: Checks if location permissions are granted. If not, requests them.
    Location Fetching: Uses fusedLocationClient to get the last known location.
    UI Update: Updates UI elements with latitude and longitude, and calls methods to get the address, weather data, and current time.

6. getAddress Method
    Reverse Geocoding: Uses Geocoder to convert latitude and longitude into a human-readable address.
    UI Update: Updates the textAddress field with the address or an error message if the address cannot be determined.

7. getWeatherData Method
    Retrofit Initialization: Sets up Retrofit to make a network request to the OpenWeatherMap API.
    API Call: Makes an asynchronous API call to fetch weather data.
    Response Handling: Parses the JSON response and updates the UI with temperature (converted from Kelvin to Celsius), humidity, and description.
   
9. displayCurrentTime Method
    Time Formatting: Uses SimpleDateFormat to format the current time.
    UI Update: Updates the textTime field with the formatted time.


## OpenWeatherMap
    API Key: To use OpenWeatherMap, you need to sign up for an API key.
    API Endpoint: The weather data can be accessed using endpoints such as https://api.openweathermap.org/data/2.5/weather.

## Retrofit
   Retrofit is a type-safe HTTP client for Android and Java. It simplifies the process of making network requests and handling responses.

## Dependencies
    AndroidX Libraries: Core libraries for building Android applications.
    Google Play Services Location: Used to obtain the device's location.
    Retrofit: A type-safe HTTP client for Android and Java.
    Gson Converter: A library to convert JSON to Java objects.

## Additional Features Implemented
    Error Handling: Gracefully handles errors such as network failures or location services being disabled.
    Responsive UI: UI is responsive and provides a good user experience on different screen sizes and orientations.
    

## Screenshots & Video Demo
[Link](https://drive.google.com/drive/folders/1qm6XO4Fc7jir2zPbhylbIFiqnP1M6YEG?usp=sharing)


    
