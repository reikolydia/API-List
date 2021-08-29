---
title: CountAPI/:hit
position_number: 3.7
type: get
description:
parameters:
content_markdown: |-
  ### /hit/:namespace?/:key ###

  An easier way to track incrementing by one keys. This endpoint will create a key if it doesn't exists and increment it by one on each subsequent request. Optionally specify a namespace.

  The key created has the following properties:

  - enable_reset to 0 (false)
  - update_lowerbound to 0
  - update_upperbound to 1

  Effectively making the key only incrementable by one.
left_code_blocks:
  - code_block: |-
       https://api.countapi.xyz/hit/mysite.com/visits
    title: Test
    language: bash
  - code_block: |-
       https://api.countapi.xyz/hit/nonexisting
    title: Non existing
    language: bash
right_code_blocks:
  - code_block: |-
        (value was 35)
        {
          "value": 36
        }
    title: Test
    language: json
  - code_block: |-
        (key is created)
        {
          "value": 1
        }
    title: Non existing
    language: json
---