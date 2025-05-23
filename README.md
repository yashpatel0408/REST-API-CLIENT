# REST-API-CLIENT
COMPANY: CODTECH IT SOLUTIONS

NAME: YASHKUMAR PATEL

INTERN ID: CT04DL1118

DOMAIN: JAVA PROGRAMMING

DURATIONS: 4 WEEKS

MENTOR: NEELA SANTOSH

DESCRIPTION: #WeatherApiData - java

Got it. Here's a more natural, human-written version of the same explanation — like how someone might explain it in a report or during a conversation with a mentor or teammate:

---

This Java project is a simple console-based application that lets users check the current weather conditions of any city they enter. It uses the Open-Meteo API to get both the location details and real-time weather data. The main idea behind this code is to show how to work with web APIs in Java, how to parse JSON responses, and how to display meaningful information to the user based on live data.

The program starts by asking the user to type the name of a city. If the user types "No", the program stops running. Otherwise, it takes the city name and sends a request to the Open-Meteo Geocoding API, which returns information like the latitude and longitude of the city. This is handled by a method called `getLocationData`. The method formats the city name for the URL, makes an HTTP GET request, reads the response, and then extracts the coordinates from the JSON data.

Once the latitude and longitude are available, the program uses them to make another API call—this time to the weather forecast endpoint of Open-Meteo. That part is handled by the `displayWeatherData` method. It fetches and displays the current temperature, relative humidity, wind speed, and the time at which this data was recorded.

To manage the network part of the program, two helper methods are used. `fetchApiResponse` sets up the HTTP connection, and `readApiResponse` reads the response and turns it into a string. The JSON data is then parsed using the JSON.simple library, which helps in extracting only the fields we’re interested in, like temperature and humidity.

The code is structured in a way that makes it easy to understand and expand. For example, if you wanted to show a 3-day forecast instead of just current weather, you could add a few more parameters to the API call and update the way data is displayed. Also, since the code handles API errors and unexpected responses using try-catch blocks, it won’t crash if something goes wrong, like an invalid city name or network issue.

Overall, this project is a good example of how to build a basic but functional weather app using Java. It covers practical topics like making HTTP requests, handling user input, parsing JSON data, and working with external services. It also lays the foundation for more advanced features, such as adding a GUI, storing history, or even integrating multiple APIs.

This kind of project is great for learning because it touches on real-world tasks developers often deal with, like consuming public APIs and turning raw data into user-friendly output. Plus, it gives a hands-on introduction to how backend services like weather apps actually work behind the scenes.
