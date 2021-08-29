---
title: BTC Rates
position_number: 2.2
type: get
description: To get BTC-to-Currency exchange rates
parameters:
content_markdown: |-
left_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://api.coingecko.com/api/v3/exchange_rates'
    title: Powershell
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "rates": {
            "btc": {
              "name": "Bitcoin",
              "unit": "BTC",
              "value": 1,
              "type": "crypto"
            },
            "eth": {
              "name": "Ether",
              "unit": "ETH",
              "value": 15.198,
              "type": "crypto"
            },
            ...
        }
    title: Response
    language: json
---