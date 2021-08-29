---
title: Getting Started
position_number: 1
parameters:
  - name:
    content:
content_markdown: |-

  A good place to start is the [httpbin.org service](https://httpbin.org/).

  ### To use Windows Powershell: ###

  HTTP **GET**

  ```
  Invoke-RestMethod -Uri ' endpoint URL ' -Method GET
  ```

  HTTP **POST**

  ```
  Invoke-WebRequest -Uri ' rest url ' -Method POST -Body @{ post_header='postbody' }
  ```

  HTTP **DELETE**

  ```
  Invoke-RestMethod -Uri ' endpoint URL ' -Method DELETE
  ```

  HTTP **PATCH**

  ```
  Invoke-RestMethod -Uri ' endpoint URL ' -Method PATCH -Body @{ patch_header='patchbody' }
  ```

  HTTP **PUT**

  ```
  Invoke-RestMethod -Uri ' endpoint URL ' -Method PUT -Body @{ put_header='putbody' }
  ```

left_code_blocks:
  - code_block:
    title:
    language:
right_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri ' endpoint URL '
    title: GET
    language: bash
  - code_block: |-
       $ Invoke-WebRequest -Uri ' rest url ' -Method POST -Body @{ post_header='postbody' }
    title: POST
    language: bash
  - code_block: |-
       $ Invoke-RestMethod -Uri ' endpoint URL ' -Method DELETE
    title: DELETE
    language: bash
  - code_block: |-
       $ Invoke-RestMethod -Uri ' endpoint URL ' -Method PATCH -Body @{ patch_header='patchbody' }
    title: PATCH
    language: bash
  - code_block: |-
       $ Invoke-RestMethod -Uri ' endpoint URL ' -Method PUT -Body @{ put_header='putbody' }
    title: PUT
    language: bash
---