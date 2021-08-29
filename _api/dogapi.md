---
title: DogAPI
position_number: 1.1
type: get
description: To get a random dog photo
content_markdown: |-
left_code_blocks:
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://dog.ceo/api/breeds/image/random/'
    title:
    language: bash
right_code_blocks:
  - code_block: |-
      {
        "message": "https://images.dog.ceo/breeds/vizsla/n02100583_10388.jpg",
        "status": "success",
      }
    title: Response
    language: json
---