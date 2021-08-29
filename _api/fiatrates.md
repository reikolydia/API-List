---
title: Fiat Rates
position_number: 2.3
type: get
description: To get Currency to Currency Exchange Rates
parameters:
  - name: from
    content: From currency
  - name: to
    content: To Currency
content_markdown: |-
left_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://cdn.jsdelivr.net/gh/fawazahmed0/currency-api@1/latest/currencies/(from)/(to).json'
    title: Powershell
    language: bash
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://cdn.jsdelivr.net/gh/fawazahmed0/currency-api@1/latest/currencies/AUD/SGD.json'
    title: Example
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "date": "2021-08-29",
          "sgd": 0.984199
        }
    title: AUD to SGD
    language: json
  - code_block: |-
        {
          "date": "2021-08-29",
          "sgd": 1.016055
        }
    title: SGD to AUD
    language: json
---