---
title: Nager Date API
position_number: 1.9
type: get
description: Get public holidays for a given year for a given country
parameters:
  - name: year (required)
    content: The year number in integer format
  - name: countryCode (required)
    content: Country code in ISO 3166-1 alpha-2 format
content_markdown: |-
left_code_blocks:
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://date.nager.at/api/v3/PublicHolidays/(year)/(countryCode)'
    title: Powershell
    language: bash
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://date.nager.at/api/v3/PublicHolidays/2021/AU'
    title: Example
    language: bash
right_code_blocks:
  - code_block: |-
        [
          {
            "date": "2021-01-01",
            "localName": "New Year's Day",
            "name": "New Year's Day",
            "countryCode": "AU",
            "fixed": true,
            "global": true,
            "counties": null,
            "launchYear": null,
            "types": [
              "public"
            ]
          },
          ...
          {
            "date": "2021-12-27",
            "localName": "Boxing Day",
            "name": "St. Stephen's Day",
            "countryCode": "AU",
            "fixed": false,
            "global": true,
            "counties": null,
            "launchYear": null,
            "types": [
              "public"
            ]
          }
        ]
    title: Response
    language: json
---