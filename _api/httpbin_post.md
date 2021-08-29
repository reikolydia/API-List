---
title: httpbin/:post
position_number: 4.6
type: post
description: A simple HTTP Request & Response Service.
parameters:
content_markdown: |-
  Test a **POST** request.
left_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://httpbin.org/post' -Method POST
    title: Powershell
    language: bash
  - code_block: |-
       $ curl -X DELETE "https://httpbin.org/post" -H "accept: application/json"
    title: cURL
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "args": {},
          "data": "",
          "files": {},
          "form": {},
          "headers": {
            "Accept": "application/json",
            "Accept-Encoding": "gzip, deflate, br",
            "Accept-Language": "en-US,en;q=0.9",
            "Dnt": "1",
            "Host": "httpbin.org",
            "Origin": "https://httpbin.org",
            "Referer": "https://httpbin.org/",
            "Sec-Ch-Ua": "\"Chromium\";v=\"92\", \" Not A;Brand\";v=\"99\", \"Microsoft Edge\";v=\"92\"",
            "Sec-Ch-Ua-Mobile": "?0",
            "Sec-Fetch-Dest": "empty",
            "Sec-Fetch-Mode": "cors",
            "Sec-Fetch-Site": "same-origin",
            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36 Edg/92.0.902.84",
            "X-Amzn-Trace-Id": "Root=1-612c0cb9-0524cfe1547937940c790183"
          },
          "json": null,
          "origin": "127.0.0.1",
          "url": "https://httpbin.org/post"
        }
    title: Response
    language: json
---