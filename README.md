# Frontend Mentor - Weather App

![Design preview for the Weather App challenge](./assets/images/preview.jpg)

## Welcome! 👋

Thanks for checking out my solution to the **Frontend Mentor Weather App Challenge**.  

This project was part of the **30-Day Hackathon** on Frontend Mentor. The goal was to build a fully responsive weather app using the **Open-Meteo API** and match the provided design as closely as possible.

---

## Table of Contents

- [Overview](#overview)  
- [My Process](#my-process)  
- [Built With](#built-with)  
- [What I Learned](#what-i-learned)  
- [Continued Development](#continued-development)  
- [Useful Resources](#useful-resources)  
- [Author](#author)  
- [Acknowledgments](#acknowledgments)  

---

## Overview

### The Challenge

Users should be able to:  

- Search for weather information by entering a location in the search bar  
- View current weather conditions including temperature, weather icon, and location details  
- See additional metrics like “feels like” temperature, humidity, wind speed, and precipitation  
- Browse a 7-day forecast with daily highs/lows and icons  
- View an hourly forecast with day selection  
- Toggle between Imperial and Metric units  
- Switch between Celsius/Fahrenheit for temperature and km/h or mph for wind  
- See responsive layouts for mobile and desktop  
- See hover and focus states for interactive elements  

---

### Screenshot

![Desktop Screenshot](./assets/images/desktop-preview.jpg)  
*Add additional screenshots as needed.*

---

### Links

- Solution URL: [Add your GitHub repo link here](https://github.com/)  
- Live Site URL: [Add your live site URL here](https://your-live-site-url.com)  

---

## My Process

### Planning

Before writing any code, I:  

1. Reviewed the **FEM brief and assets**.  
2. Created a **project folder** with separate subfolders for `assets`, `styles`, and `scripts`.  
3. Designed a **mobile-first CSS Grid layout** that adapts to desktop using media queries.  
4. Planned **JS functions** for fetching and displaying weather data dynamically.  

### Building the App

- Built **semantic HTML** for structure and accessibility.  
- Styled components using **CSS Grid & Flexbox** for responsive layouts.  
- Fetched data from the **Open-Meteo API** and dynamically rendered:  
  - Current weather  
  - Hourly forecast  
  - 7-day forecast  
- Implemented **unit toggles** (Metric ↔ Imperial).  
- Added **hover and focus states** for better UX.  

---

## Built With

- HTML5  
- CSS3 (Grid & Flexbox, Custom Properties)  
- JavaScript (ES6+)  
- Open-Meteo API  
- Google Fonts: DM Sans, Bricolage Grotesque  

---

## What I Learned

During this project, I learned:  

- How to structure a **responsive layout using CSS Grid** for complex designs.  
- Dynamically updating the DOM with **API data**.  
- How to implement a **unit toggle system** for temperature, wind, and precipitation.  
- Best practices for **project organization** and clean code.  

```js
// Example: Fetch current weather for a location
async function fetchWeather(lat, lon) {
  const response = await fetch(`https://api.open-meteo.com/v1/forecast?latitude=${lat}&longitude=${lon}&current_weather=true`);
  const data = await response.json();
  console.log(data);
}


## Continued Development

I plan to improve this project by:

- Adding geolocation detection for first-time users
- Implementing dark/light mode
- Showing animated backgrounds based on weather conditions
- Adding sunrise/sunset and UV index data

## Useful Resources

- [Open-Meteo API Documentation](https://open-meteo.com/) – helped me understand how to fetch weather data.
- [CSS Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/) – reference for responsive layouts.
- [Frontend Mentor](https://www.frontendmentor.io/) – for challenge setup and asset files.

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://twitter.com/yourusername)

## Acknowledgments

Thanks to **Frontend Mentor** for providing the challenge and assets.  
Special thanks to the **community** for inspiration and guidance.
