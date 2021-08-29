---
title: TLE API Record
position_number: 1.4
type: get
description: The TLE API provides up to date two line element set records, the data is updated daily from CelesTrak. A two-line element set (TLE) is a data format encoding a list of orbital elements of an Earth-orbiting object for a given point in time.
parameters:
  - name: id (required)
    content: Satellite ID
content_markdown: |-
  Return single TLE Model for requested satellite ID.
left_code_blocks:
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://tle.ivanstanojevic.me/api/tle/(id)'
    title: 
    language: bash
right_code_blocks:
  - code_block: |-
      {
        "@context": "https://www.w3.org/ns/hydra/context.jsonld",
        "@id": "https://tle.ivanstanojevic.me/api/tle/43638",
        "@type": "TleModel",
        "satelliteId": 43638,
        "name": "1998-067PN",
        "date": "2021-02-16T06:41:41+00:00",
        "line1": "1 43638U 98067PN  21047.27895714  .00025925  00000-0  18734-3 0  9990",
        "line2": "2 43638  51.6322 151.1192 0001883 262.5831  97.4954 15.73313437134937"
      }
    title: Response
    language: json
---