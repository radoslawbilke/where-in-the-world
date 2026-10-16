# Where In The World

Explore countries of the world and check the current weather in their capitals.

**Live demo: [radoslawbilke.github.io/where-in-the-world](https://radoslawbilke.github.io/where-in-the-world/)**

Based on the [REST Countries API with color theme switcher](https://www.frontendmentor.io/challenges/rest-countries-api-with-color-theme-switcher-5cacc469fec04111f7b848ca) challenge from Frontend Mentor, extended with a Weather App.

## Features

### Countries App

- List of 250 countries with flag, population, region and capital
- Search by country name and filter by region
- Country details: native name, sub region, top level domain, currencies, languages
- Border countries linked to their own detail pages
- Link to the weather in the country's capital

### Weather App

- List of 245 capital cities with current temperature and conditions
- Search by city or country name and filter by region
- Weather is loaded only for visible tiles, more cities load while scrolling
- City details: feels like temperature, humidity, wind, precipitation, local time
- 7-day forecast

### General

- Light and dark theme
- Responsive layout for mobile and desktop

## Built with

- [Nuxt 2](https://v2.nuxt.com/) (Vue 2, Vuex), generated as a static site
- SCSS
- [Font Awesome](https://fontawesome.com/) icons
- [Axios](https://axios-http.com/)

## Data sources

- **Countries** - `static/data.json`, the dataset provided with the
  Frontend Mentor challenge (REST Countries v2 format). It is served locally because the
  original `restcountries.com/v2` API has been shut down.
- **Weather** - [Open-Meteo](https://open-meteo.com/), free for non-commercial use, no API key needed.
- **Capital coordinates** - `static/capitals.json`, generated once
  with the Open-Meteo geocoding API by `scripts/build-capitals.js`:

  ```bash
  node scripts/build-capitals.js
  ```

- **Flags** - [flagcdn.com](https://flagcdn.com/)
