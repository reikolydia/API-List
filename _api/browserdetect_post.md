---
title: Browser Detect
position_number: 2.7
type: post
description: A fast user-agent lookup API that detects Browser, OS, Device Type and other attributes from user-agent
parameters:
  - name: ua
    content: A JSON object with user agent string
content_markdown: |-
  If you prefer working with POST APIs, you can use this API - it works very similar to GET API, and accepts user agent string in **ua** key in the input JSON and returns the JSON object with parsed data.
left_code_blocks:
  - code_block: |-
       $ Invoke-WebRequest -Uri 'https://api.apicagent.com' -Method POST -Body @{'ua'=(ua)}
    title: Powershell
    language: bash
  - code_block: |-
       $ Invoke-WebRequest -Uri 'https://api.apicagent.com' -Method POST -Body @{'ua'='Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.114 Safari/537.36'}
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