---
title: Getting Started
position_number: 1
parameters:
  - name:
    content:
content_markdown: |-
  To use Windows Powershell:

  HTTP **GET**

  Invoke-RestMethod -Uri ' endpoint URL '

  HTTP **POST**

  Invoke-WebRequest -Uri ' rest url ' -Method POST -Body @{ post_header='postbody' }

left_code_blocks:
  - code_block:
    title:
    language:
right_code_blocks:
  - code_block: |2-
       $ Invoke-RestMethod -Uri ' endpoint URL '
    title: GET
    language: bash
  - code_block: |2-
       Invoke-WebRequest -Uri ' rest url ' -Method POST -Body @{ post_header='postbody' }
    title: POST
    language: bash
---