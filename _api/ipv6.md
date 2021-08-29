---
title: IPv6 Address
position_number: 3.1
type: get
description: Get your IPv6 address.
parameters:
content_markdown: |-
left_code_blocks:
  - code_block: |-
       get_ipv6=$(wget "http://ip6.me/api" -qO- | cut -c6-)
       corrected_ipv6=${get_ipv6::-44}

       echo $corrected_ipv6
    title: Bash
    language: bash
right_code_blocks:
  - code_block: |-
        2001:db8::::ff00:42:8329
    title: Response
    language: JavaScript
---