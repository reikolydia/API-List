---
title: MetaWeather
position_number: 1.5
type: get
description: MetaWeather provides an API that delivers JSON over HTTPS for access to their data.
parameters:
  - name: woeid
    content: Where On Earth ID
content_markdown: |-
left_code_blocks:
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://www.metaweather.com/api/location/(woeid)'
    title: 
    language: bash
right_code_blocks:
  - code_block: |-
      {
        "Consolidated_weather": [
          {
            "id": 6413024211501056,
            "weather_state_name": "Heavy Rain",
            "weather_state_abbr": "hr",
            "wind_direction_compass": "WNW",
            "created": "2021-08-26T10:26:25.866844Z",
            "applicable_date": "2021-08-31",
            "min_temp": 14.49,
            "max_temp": 18.75,
            "the_temp": 16.72,
            "wind_speed": 8.846679988865029,
            "wind_direction": 293.5,
            "air_pressure": 1016.0,
            "humidity": 78,
            "visibility": 9.999726596675416,
            "predictability": 77
          }
        ],
        "time": "2021-08-26T18:43:37.642328+08:00",
        "sun_rise": "2021-08-26T06:39:38.085452+08:00",
        "sun_set": "2021-08-26T17:56:25.525476+08:00",
        "timezone_name": "LMT",
        "parent": {
          "title": "Australia",
          "location_type": "Country",
          "woeid": 23424748,
          "latt_long": "-24.912100,133.397552"
        },
        "sources": [
          {
            "title": "BBC",
            "slug": "bbc",
            "url": "http://www.bbc.co.uk/weather/",
            "crawl_rate": 360.0
          },
          ...
          {
            "title": "World Weather Online",
            "slug": "world-weather-online",
            "url": "http://www.worldweatheronline.com/",
            "crawl_rate": 360.0
          }
        ],
        "title": "Perth",
        "location_type": "City",
        "woeid": 1098081,
        "latt_long": "-31.953020,115.857239"
        "timezone": "Australia/Perth"
      }
    title: Response
    language: json
---