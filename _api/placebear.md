---
title: placebear
position_number: 1.3
type: get
description: To get a random placeholder picture of a bear
parameters:
  - name: width
    content: Width in pixels
  - name: height
    content: Height in pixels
content_markdown: |-
    The response will be in a image of jpeg format.
left_code_blocks:
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://placebear.com/(width)/(height).jpg'
    title: Powershell
    language: bash
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://placebear.com/200/300.jpg'
    title: Example
    language: bash
right_code_blocks:
  - code_block: |-
      Content-type: image/jpeg
    title: Response
    language: json
---