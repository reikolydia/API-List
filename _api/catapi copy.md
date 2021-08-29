---
title: mail.tm/:Accts
position_number: 1.8
type: post
description: To create a temporary mail.tm account
parameters:
  - name: address
    content: user@example.com
  - name: password
    content: Password of desired account
content_markdown: |-
left_code_blocks:
  - code_block: |-
      Invoke-WebRequest -Uri 'https://api.mail.tm/accounts' -Method POST -Body @{address='tempuser@trythe.net'; password='temppassword'} -Headers @{'Content-Type'='application/json'}
    title: Random
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "@context": "/contexts/Account",
          "@id": "/accounts/612bbbbbc90fae3bde3e6056",
          "@type": "Account",
          "id": "612bbbbbc90fae3bde3e6056",
          "address": "tempuser@trythe.net",
          "quota": 40000000,
          "used": 0,
          "isDisabled": false,
          "isDeleted": false,
          "createdAt": "2021-08-29T16:54:19+00:00",
          "updatedAt": "2021-08-29T16:54:19+00:00"
        }
    title: Response
    language: json
---