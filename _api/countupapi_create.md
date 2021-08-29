---
title: CountAPI/:create
position_number: 3.8
type: get
description:
parameters:
content_markdown: |-
  ### /create ###

  Creates a key.
  All parameters are optional

  | **name** | **default** | **description** |
  | --- | :---: | --- |
  | key | New UUID | Name of the key |
  | namespace | default | Namespace to store the key |
  | value | 0 | The initial value stored |
  | enable_reset | 0 | Allows the key to be resetted with **/set** |
  | update_lowerbound | -1 | Restrict update to not subtract more than this number. This number **must** be negative or zero. |
  | update_upperbound | 1 | Restrict update to not add more than this number. This number **must** be positive or zero. |

  Note about **expiration**: Every time a key is updated its expiration is set to **6 months**. So don't worry, if you still using it, it won't expire.
  {: .info}

  Keys and namespaces must have at least 3 characters and less or equal to 64. Keys and namespaces must match: **^[A-Za-z0-9_\-.]{3,64}$**
  {: .info}
left_code_blocks:
  - code_block: |-
       https://api.countapi.xyz/create
    title: Create
    language: bash
  - code_block: |-
       https://api.countapi.xyz/create?namespace=mysite.com&value=42
    title: Create mysite.com
    language: bash
  - code_block: |-
       https://api.countapi.xyz/create?key=counter&expiration=60
    title: Create with expiration
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "namespace": "default",
          "key": "6d5891ff-ebda-48fb-a760-8549d6a3bf3a",
          "value": 0
        }
    title: Create
    language: json
  - code_block: |-
        {
          "namespace": "mysite.com",
          "key": "33606dbe-4800-4228-b042-5c0fb8ec8f08",
          "value": 42
        }
    title: Create mysite.com
    language: json
  - code_block: |-
        {
          "namespace": "default",
          "key": "counter",
          "value": 42
        }
    title: Create with expiration
    language: json
  - code_block: |-
        https://api.countapi.xyz/create?name=alreadycreated
        (the key already existed)
        {
          "namespace": null,
          "key": null,
          "value": null
        }
    title: Error 409
    language: json
---