# Weather Dashboard

## Assignment 1: Weather Dashboard

### Objective
Create a weather dashboard that displays the current weather and a 5-day forecast for a given city. The application will use the OpenWeatherMap API to fetch weather data and a JSON server to store and retrieve a list of favorite cities.

### Features
- Search for a city's weather data, including the current weather and a 5-day forecast.
- Save cities to a list of favorites for quick access.
- Remove cities from the favorites list.
- Display weather information for the cities stored in favorites.
- Toggle between Celsius and Fahrenheit for temperature display.

### Technologies Used
- **React**: A front-end JavaScript library to create reusable components for the dashboard.
- **OpenWeatherMap API**: To fetch weather data for the selected cities.
- **JSON Server**: Simulated backend to store and manage favorite cities.
- **CSS**: Styling for a visually appealing and user-friendly interface.

### Components
1. **Main Dashboard Component**: Displays the weather dashboard.
2. **Search Component**: Allows users to search for a city's weather.
3. **Weather Display Component**: Shows the current weather and the 5-day forecast for the selected city.
4. **Favorite Cities Component**: Displays and manages a list of favorite cities.

### Features Breakdown

1. **Weather Search Functionality**:
   - Users can enter a city name in the search component.
   - The current weather and 5-day forecast for the city are displayed using the OpenWeatherMap API.

2. **Favorite Cities**:
   - Users can add cities to a list of favorites.
   - The favorite cities are stored on the JSON server.
   - CRUD (Create, Read, Update, Delete) operations are implemented to manage favorite cities.
   - Users can remove cities from the favorites list.

3. **Weather Display for Favorite Cities**:
   - Weather data for favorite cities is fetched and displayed in the dashboard.

4. **Bonus Features**:
   - **Local Storage**: The last searched city is remembered using local storage.
   - **Temperature Toggle**: Users can switch between Celsius and Fahrenheit for weather data.

### Setup Instructions

1. Clone the repository:
    ```bash
    git clone <repository-url>
    ```

2. Install the dependencies:
    ```bash
    npm install
    ```

3. Start the JSON server:
    ```bash
    json-server --watch db.json --port 5000
    ```

4. Start the React development server:
    ```bash
    npm start
    ```

5. Obtain an API key from [OpenWeatherMap](https://openweathermap.org/api) and add it to your `.env` file:
    ```env
    REACT_APP_WEATHER_API_KEY=<your-api-key>
    ```

6. Open the application in your browser at:
    ```
    http://localhost:3000
    ```

### JSON Server (Favorites Management)
The JSON server will handle storing, retrieving, and managing the user's favorite cities. It supports full CRUD operations:
- **Create**: Add a new city to the favorites list.
- **Read**: Display the list of favorite cities.
- **Update**: Edit or update the favorite city list.
- **Delete**: Remove a city from the favorites list.

### API Usage

- **OpenWeatherMap API**: 
    - Current Weather: `https://api.openweathermap.org/data/2.5/weather?q=<city>&appid=<your-api-key>`
    - 5-Day Forecast: `https://api.openweathermap.org/data/2.5/forecast?q=<city>&appid=<your-api-key>`

### Screenshots

_Add screenshots of your app here_

### Future Enhancements
- Add detailed weather information (humidity, wind speed, etc.).
- Add the ability to sort favorite cities.
- Implement more user-friendly error handling.

### License
This project is licensed under the MIT License.
