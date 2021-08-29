---
title: CountAPI
position_number: 3.3
type: get
description: This API allows you to create simple numeric counters. IaaS, Integer as a Service.
parameters:
  - name: namespace
    content: The namespace should be unique, so its recommend using your site's domain
  - name: key
    content: Each counter is identified inside a namespace with a key
content_markdown: |-
  ## Endpoints ##
  All requests support cross-origin resource sharing (CORS) and SSL.
  You can use JSONP sending the callback parameter. JSONP requests will never fail, they will include the HTTP code in the response.
  Also a 1x1 GIF image is supported sending ?img.

  Base API path: https://api.countapi.xyz

  In the case of a server failure, the API will send an error 500.
left_code_blocks:
right_code_blocks:
  - code_block: |-
        {
          "error": "Error description"
        }
    title: Error 500
    language: json
---