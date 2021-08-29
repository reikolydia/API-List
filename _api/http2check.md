---
title: HTTP/2 API
position_number: 4.1
type: get
description:
parameters:
content_markdown: |-
  You can use this simple API to check if your HTTP client supports HTTP2.

  | **Key** | **Description** |
  | --- | --- |
  | http2 | 	Whether HTTP/2 was used for the connection. Possible values are 0 (HTTP/2 was used) and 1 (HTTP/2 was not used). |
  | protocol | 	The actual protocol used for the connection. Possible values include HTTP/2.0, HTTP/1.1 and HTTP/1.0. |
  | push | 1 if the client indicated it supports HTTP/2 push. 0 otherwise. |
  | user_agent | The User Agent string sent to the API as-is. An empty string if the client did not send the user agent header. |
left_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://http2.pro/api/v1'
    title: Powershell
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "http2": 1,
          "protocol": "HTTP/2.0",
          "push": 1,
          "user_agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36 Edg/92.0.902.84"
        }
    title: Response
    language: json
---