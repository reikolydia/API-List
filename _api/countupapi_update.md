---
title: CountAPI/:Update
position_number: 3.6
type: get
description:
parameters:
content_markdown: |-
  ### /update/:namespace?/:key?amount=:amount ###

  Updates a key with +/- amount. Optionally specify the namespace.
  
  The amount **must** be within update_lowerbound and update_upperbound specified during the creation of the key.
left_code_blocks:
  - code_block: |-
       https://api.countapi.xyz/update/test?amount=5
    title: Test
    language: bash
  - code_block: |-
       https://api.countapi.xyz/update/mysite.com/test?amount=-7
    title: mysite.com Test
    language: bash
right_code_blocks:
  - code_block: |-
        (value was 42)
        {
          "value": 47
        }
    title: Test
    language: json
  - code_block: |-
        (value was 53)
        {
          "value": 46
        }
    title: mysite.com Test
    language: json
  - code_block: |-
        https://api.countapi.xyz/update/outofrange?amount=3
        (value was 47, update_upperbound=2)
        {
          "value": 47
        }
    title: Error 403
    language: json
  - code_block: |-
        https://api.countapi.xyz/update/nonexisting?amount=1
        {
          "value": null
        }
    title: Error 404
    language: json
---