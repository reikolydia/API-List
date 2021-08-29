---
title: Bored API
position_number: 2.8
type: get
description: The Bored API helps you find things to do when you're bored. There are fields like the number of participants, activity type, and more that help you narrow down your results.
parameters:
  - name: activity
    content: Description of the queried activity
  - name: key
    content: A unique numeric id
  - name: type
    content: Type of the activity
  - name: participants
    content: The number of people that this activity could involve
  - name: price
    content: A factor describing the cost of the event with zero being free
  - name: accessibility
    content: A factor describing how possible an event is to do with zero being the most accessible
content_markdown: |-
left_code_blocks:
  - code_block: |-
       $ Invoke-RestMethod -Uri 'http://www.boredapi.com/api/activity?(parameter)=(parameter)'
    title: Powershell
    language: bash
  - code_block: |-
       $ Invoke-RestMethod -Uri 'http://www.boredapi.com/api/activity?key=5881028'
    title: Example
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "activity": "Learn a new programming language",
          "accessibility": 0.25,
          "type": "education",
          "participants": 1,
          "price": 0.1,
          "key": 5881028
        }
    title: Response
    language: json
---