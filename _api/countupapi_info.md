---
title: CountAPI/:info
position_number: 3.9
type: get
description:
parameters:
content_markdown: |-
  ### /info/:namespace?/:key ###

  Get information about a key. Optionally specify the namespace.
left_code_blocks:
  - code_block: |-
       https://api.countapi.xyz/info/test
    title: Info
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "namespace": "default",
          "key": "test",
          "ttl": 321,
          "value": 42,
          "enable_reset": false,
          "update_upperbound": 1,
          "update_lowerbound": 1
        }
    title: Info
    language: json
  - code_block: |-
        {
          "namespace": null,
          "key": null,
          "ttl": null,
          "value": null,
          "enable_reset": null,
          "update_upperbound": null,
          "update_lowerbound": null
        }
    title: Error 404
    language: json
---