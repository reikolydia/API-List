---
title: Email Validator
position_number: 2.4
type: get
description: To identify if the email is valid or not.
parameters:
  - name: email
    content: Email address to be validated
content_markdown: |-
left_code_blocks:
  - code_block: |-
       $ cURL --location --request GET 'https://api.eva.pingutil.com/email?email=(email)
    title: cURL
    language: bash
  - code_block: |-
       $ cURL --location --request GET 'https://api.eva.pingutil.com/email?email=test@mail7.io
    title: cURL Example
    language: bash
  - code_block: |-
      GET /email?email=(email) HTTP/1.1
      Host: https://api.eva.pingutil.com
    title: HTTP GET
    language: bash
  - code_block: |-
      var settings = {
        "url": "https://api.eva.pingutil.com/email?email=(email)",
        "method": "GET",
        "timeout": 0,
      };
      $.ajax(settings).done(function (response) {
        console.log(response);
      });
    title: jQuery
    language: bash
  - code_block: |-
      import http.client
      import mimetypes
      conn = http.client.HTTPSConnection("api.eva.pingutil.com")
      payload = ''
      headers = {}
      conn.request("GET", "/email?email=(email)", payload, headers)
      res = conn.getresponse()
      data = res.read()
      print(data.decode("utf-8"))
    title: Python
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "status": "success",
          "data": {
            "email_address": "test@mail7.io",
            "domain": "mail7.io",
            "valid_syntax": true,
            "disposable": true,
            "webmail": false,
            "deliverable": true,
            "catch_all": true,
            "gibberish": false,
            "spam": false
          }
        }
    title: Response
    language: json
---