---
title: anonfiles
position_number: 2.1
type: get
description: To get a file's information from anonfiles.com
parameters:
  - name: id
    content: ID of file
content_markdown: |-
left_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://api.anonfiles.com/v2/file/vfd0C8Ebu0/info'
    title: Powershell
    language: bash
right_code_blocks:
  - code_block: |2-
        {
          "status": true,
          "data": {
            "file": {
              "url": {
                "full": "https://anonfiles.com/u1C0ebc4b0/file.txt",
                "short": "https://anonfiles.com/u1C0ebc4b0",
              },
              "metadata": {
                "id": "u1C0ebc4b0",
                "name": "file.txt",
                "size": {
                  "bytes": "6861",
                  "readable": "6.7 KB"
                }
              }
            }
          }
        }
    title: Success
    language: json
  - code_block: |2-
      {
          "status": false,
          "error": {
            "message": "File is too large. Max file size is 5 GiB.",
            "type": "ERROR_FILE_SIZE_EXCEEDED"
            "code": 31
        }
    title: Error
    language: json
---