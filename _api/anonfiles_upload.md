---
title: anonfiles
position_number: 2.0
type: post
description: To upload a file to anonfiles.com via POST
parameters:
  - name: file
    content: Path to, and full filename
content_markdown: |-
left_code_blocks:
  - code_block: |-
       $ curl -F 'file=@(path to file)\(filename).(file extension)' https://api.anonfiles.com/upload 
    title: curl
    language: bash
  - code_block: |-
       $ curl -F 'file=@C:\file.txt' https://api.anonfiles.com/upload 
    title: Example
    language: bash
right_code_blocks:
  - code_block: |-
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
  - code_block: |-
      {
          "status": false,
          "error": {
            "message": "File is too large. Max file size is 5 GiB.",
            "type": "ERROR_FILE_SIZE_EXCEEDED"
            "code": 31
          }
        }
    title: Error
    language: json
---