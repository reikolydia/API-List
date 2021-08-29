---
title: ipinfo.io
position_number: 3.0
type: get
description: Get geolocation data for the target IP address, which includes country, region, city, and postal code.
parameters:
  - name: ip
    content: Target IP Address
content_markdown: |-
left_code_blocks:
  - code_block: |-
       $ curl ipinfo.io/(ip)
    title: curl
    language: bash
  - code_block: |-
       $ curl ipinfo.io/8.8.8.8
    title: Example
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "ip": "8.8.8.8",
          "hostname": "dns.google.com",
          "anycast": "true",
          "city": "Mountain View",
          "region": "California",
          "country": "US",
          "loc": "37.4056,-122.0775",
          "org": "AS15169 Google LLC",
          "postal": "94043",
          "timezone": "America/Los_Angeles"
        }
    title: Response
    language: json
---