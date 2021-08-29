---
title: Browser Detect
position_number: 2.6
type: get
description: A fast user-agent lookup API that detects Browser, OS, Device Type and other attributes from user-agent
parameters:
  - name: ua
    content: User agent string in url encoded format
content_markdown: |-
  This API is the simplest way to get started with apicagent's user-agent parsing API. It accepts user agent string in **ua** parameter and returns the JSON object with parsed data.
left_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://api.apicagent.com/?ua=(ua)'
    title: Powershell
    language: bash
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://api.apicagent.com/?ua=Mozilla/5.0%20(Macintosh;%20Intel%20Mac%20OS%20X%2010_15_5)%20AppleWebKit/537.36%20(KHTML,%20like%20Gecko)%20Chrome/89.0.4389.114%20Safari/537.36'
    title: Example
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "browser_family": "Chrome",
          "client": {
            "engine": "Blink",
            "engine_version": "unknown",
            "name": "Chrome",
            "type": "Browser",
            "version": "89.0.4389.114"
          },
          "device": {
            "brand": "Apple",
            "model": "unknown",
            "type": "desktop"
          },
          "os": {
            "name": "Mac",
            "platform": "unknown",
            "version": "10.15.5"
          },
          "os_family": "Mac"
        }
    title: Response
    language: json
---