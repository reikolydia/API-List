---
title: Cloudflare Trace
position_number: 2.9
type: get
description: Get IP Address, TimeStamp, User Agent, Country Code, IATA, HTTP Version, TLS/SSL Version & more by Cloudflare.
parameters:
content_markdown: |-
left_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri 'https://1.1.1.1/cdn-cgi/trace'
    title: Powershell
    language: bash
right_code_blocks:
  - code_block: |-
        fl=47f54
        h=1.1.1.1
        ip=11.111.11.11
        ts=1597428248.652
        visit_scheme=https
        uag=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36 Edg/92.0.902.84
        colo=OH
        http=http/2
        loc=US
        tls=TLSv1.3
        sni=off
        warp=plus
        gateway=off
    title: Response
    language: JavaScript
---