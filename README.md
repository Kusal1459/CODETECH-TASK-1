# CODETECH-TASK-1
WEATHER FORECASTING
Name: GANTA KUSAL SAI
Company: CODTECH IT SOLUTIONS
ID:CT08DS9785
DOMAIN:WEB DEVELOPMENT 
DURATION:NOVEMBER TO DECEMBER 2024

### Weather Forecast Application Documentation

---

### **Overview**
The Weather Forecast application is a responsive web application that allows users to view current weather conditions for any city. The app fetches data from the OpenWeatherMap API and displays the city name, date, temperature, weather condition description, wind speed, and an appropriate weather icon.

---

### **Features**
1. Displays current weather data, including:
   - Temperature in Celsius.
   - Weather condition description (e.g., "Clear Sky").
   - Wind speed in meters per second (m/s).
   - Current date and time.
   - Weather icon (e.g., sun, cloud, rain).
2. Fetches weather data dynamically for any user-specified city.
3. Includes animations for a smooth user experience.
4. Styled with a visually appealing and responsive design.

---

### **Files and Their Roles**
#### 1. **`index.html`**
   - Structure of the web application.
   - Contains the input field, button, and placeholders for weather data.

#### 2. **`style.css`**
   - Responsible for styling the application, including layout, colors, fonts, and hover effects.
   - Uses responsive techniques to enhance the user interface.

#### 3. **`script.js`**
   - Handles data fetching and updates the DOM with the fetched weather data.
   - Includes error handling for user input and API responses.

---

### **File Details**

#### **1. `index.html`**
- **Purpose**: Provides the skeleton of the web app.
- **Important Sections**:
  - **Weather Card**:
    - Title (`h1`): Displays "Weather-Forecast".
    - Input Field (`#city-input`): Allows users to enter a city name.
    - Button (`#city-input-btn`): Triggers the weather fetching function.
    - Weather Info Section (`#weather-info`): Displays fetched data dynamically.

---

#### **2. `style.css`**
- **Purpose**: Styles the HTML elements for a clean and modern appearance.
- **Key Features**:
  - **Background**: Gradient from blue to purple for an aesthetic feel.
  - **Weather Card**:
    - Rounded corners, shadow effects, and hover animation.
  - **Responsive Input and Button**:
    - Ensures usability across different devices.
  - **Weather Icon**:
    - Scaled for visibility.
  - **Typography**:
    - Fonts and colors are chosen for clarity and visual appeal.

---

#### **3. `script.js`**
- **Purpose**: Contains JavaScript logic for fetching and displaying weather data.
- **Functions**:
  - **`weatherFn(cName)`**:
    - Fetches weather data for the city specified in `cName`.
    - Constructs the API URL with the city name and API key.
    - Handles network errors and invalid city names gracefully.
  - **`weatherShowFn(data)`**:
    - Dynamically updates the DOM with the weather data.
    - Updates the weather icon URL using the `icon` property from the API response.
  - **`capitalizeFirstLetter(string)`**:
    - Capitalizes the first letter of the weather description.

---

### **APIs and Libraries Used**
1. **[OpenWeatherMap API](https://openweathermap.org/)**:
   - Provides current weather data.
   - Returns data such as temperature, weather conditions, and wind speed.

2. **[jQuery](https://jquery.com/)**:
   - Simplifies DOM manipulation and event handling.
   - Version used: 3.6.0.

3. **[Moment.js](https://momentjs.com/)**:
   - Formats the current date and time.
   - Used to display the current date in a readable format.

4. **[Animate.css](https://animate.style/)**:
   - Adds fade-in animation to the weather info section.

---

### **How to Run**
1. Download or clone the project files.
2. Open `index.html` in a modern browser.
3. Enter a city name in the input field and click the "Get Weather" button.
4. View the current weather data for the specified city.

---

### **Customization**
1. **Change the Default City**:
   - Update the city in the `weatherFn('Pune')` call inside `script.js`.

2. **Add More Data**:
   - Extend the `weatherShowFn` function to display additional data such as humidity or sunrise/sunset times (available in the API response).

3. **Style Enhancements**:
   - Modify `style.css` to customize colors, fonts, and layout.

---

### **Error Handling**
1. Displays a user-friendly error message if:
   - The city name is invalid.
   - There is a network issue or API error.
2. Hides the weather info section (`#weather-info`) if data is not available.

---

### **Key Considerations**
1. Ensure you replace the placeholder `apiKey` with your own API key from OpenWeatherMap.
2. This app uses metric units (Celsius). Modify the `units=metric` query parameter to `units=imperial` for Fahrenheit.

---

### **Example Output**
- **City**: Pune
- **Date**: December 7th, 2024, 4:45 PM
- **Temperature**: 28.5°C
- **Description**: Clear Sky
- **Wind Speed**: 2.5 m/s
- **Icon**: ☀️ (Sun)
sample output
![weather-forecast](https://github.com/user-attachments/assets/f5c3017e-73ef-4113-84c2-90d55995629c)
