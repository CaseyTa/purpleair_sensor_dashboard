# PurpleAir Sensor Dashboard

A simple, single-page web application to display real-time air quality and environmental data from a specific PurpleAir sensor. 

## Description

This project provides a user-friendly interface to monitor data from any public PurpleAir sensor. It fetches a few fields and applies Lance Wallace's environmental correction formulas to provide more accurate estimations of ambient temperature and humidity. The data is color-coded to provide a quick visual assessment of air quality and data freshness.

### Features

* Real-time Data: Fetches and displays the latest sensor readings.
* Specific Sensor Tracking: Easily configurable to monitor any PurpleAir sensor by its index.
* Corrected Environmental Data: Applies Lance Wallace's correction formulas for more accurate temperature and humidity readings.
* Dynamic Color Coding:
  * Particulate Matter (PM1.0, PM2.5, PM10.0): Values are colored from green (good) to red (hazardous) based on common air quality thresholds.
  * Temperature & Humidity: Uses a color gradient to visually represent the readings (e.g., blue for cold, red for hot).
  * Data Freshness: The "Last Seen" timestamp changes color to indicate how recently the data was updated, from green (under 10 minutes) to red (over 6 hours).
  * Responsive Design: The layout is optimized for viewing on desktops, tablets, and mobile devices.
  * Efficient API Calls: Requests only the necessary data fields from the PurpleAir API to minimize overhead.
  * Custom Icon: Features the PurpleAir cloud icon as the browser tab's favicon.

## How to Use

1. Clone or Download: Get the `purpleair_monitor.html` file.
1. Edit Configuration: Open the `purpleair_monitor.html` file in a text editor and locate the configuration section within the `<script>` tag at the bottom.
1. Set Your API Key: Replace `'YOUR_API_KEY_HERE'` with your own PurpleAir "Read" API key. You can request one from the PurpleAir website.
1. Set Sensor Index: Replace the example `'SENSOR_INDEX'` value with the index of the sensor you wish to monitor. You can find the index by clicking a sensor on the PurpleAir map and looking at the number in the URL.
1. Open in Browser: Save your changes and open the `purpleair_monitor.html` file in any modern web browser. The data will load automatically.


## Credits

This project (both the web app and readme) was primarily written by Google Gemini 2.5 Pro.
