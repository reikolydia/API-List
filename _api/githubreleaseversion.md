---
title: Github Release
position_number: 3.2
type: get
description: Get the latest releases' version number from a Github repository.
parameters:
content_markdown: |-
left_code_blocks:
  - code_block: |-
       echo $(curl -s https://api.github.com/repos/fish-shell/fish-shell/releases | grep -o 'tag/[v.0-9]*' | awk -F/ '{print $2}' | head -1)
    title: Bash
    language: bash
right_code_blocks:
  - code_block: |-
        3.3.1
    title: Response
    language: JavaScript
---