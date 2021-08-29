---
title: CountAPI/:get
position_number: 3.4
type: get
description:
parameters:
content_markdown: |-
  ### /get/:namespace?/:key ###

  Get the value of a key. Optionally specify the namespace.
left_code_blocks:
  - code_block: |-
       https://api.countapi.xyz/get/test
    title: Test
    language: bash
  - code_block: |-
       https://api.countapi.xyz/get/mysite.com/test
    title: mysite.com Test
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "value": 42
        }
    title: Test
    language: json
  - code_block: |-
        {
          "value": 24
        }
    title: mysite.com Test
    language: json
  - code_block: |-
        https://api.countapi.xyz/get/nonexisting
        {
          "value": null
        }
    title: Error 404
    language: json
---