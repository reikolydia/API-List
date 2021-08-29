---
title: CountAPI/:set
position_number: 3.5
type: get
description:
parameters:
content_markdown: |-
  ### /set/:namespace?/:key?value=:value ###

  Set the value of a key. Optionally specify the namespace.
  
  The key **must** be created with enable_reset set to 1 (true).

  This endpoint will return the previous value before the assignation.
left_code_blocks:
  - code_block: |-
       https://api.countapi.xyz/set/test?value=69
    title: Test
    language: bash
  - code_block: |-
       https://api.countapi.xyz/mysite.com/test?value=96
    title: mysite.com Test
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "old_value": 42,
          "value": 69
        }
    title: Test
    language: json
  - code_block: |-
        {
          "old_value": 24,
          "value": 96
        }
    title: mysite.com Test
    language: json
  - code_block: |-
        https://api.countapi.xyz/set/resetdisabled?value=33
        {
          "old_value": 1234,
          "value": 1234
        }
    title: Error 403
    language: json
  - code_block: |-
        https://api.countapi.xyz/set/nonexisting?value=33
        {
          "old_value": null,
          "value": null
        }
    title: Error 404
    language: json
---