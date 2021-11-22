---
title: catAPI
position_number: 1.0
type: get
description: To get a random cat photo
parameters:
  - name: rest
    content: Get a random cat photo
  - name: restId
    content: Gets a cat photo by ID number
content_markdown: |-
left_code_blocks:
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://thatcopy.pw/catapi/rest/'
    title: Random
    language: bash
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://thatcopy.pw/catapi/restId/(ID)'
    title: By ID
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "id": 19,
          "title": "https://i.thatcopy.pw/cat/LsSZNPk.jpg",
          "webpurl": "https://i.thatcopy.pw/cat-webp/LsSZNPk.webp",
          "x": 43.4
          "y": 44.97
        }
    title: Random
    language: json
  - code_block: |-
      {
          "id": 1,
          "title": "https://i.thatcopy.pw/cat/3UJTX32.jpg",
          "webpurl": "https://i.thatcopy.pw/cat-webp/3UJTX32.webp",
          "x": 60.27
          "y": 46.98
      }
    title: By ID
    language: json
---
