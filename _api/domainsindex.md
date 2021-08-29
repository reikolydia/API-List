---
title: Domains DB
position_number: 1.7
type: get
description: To get information about a domain name
parameters:
  - name: api_key
    content: API key
  - name: date
    content: Request date
  - name: page
    content: Search page to request
  - name: limit
    content: Results per page
  - name: domain
    content: Domain includes
  - name: zone
    content: In Zone
  - name: country
    content: Hosting Country
  - name: isDead
    content: Dead or Notm default not
  - name: A
    content: A record includes
  - name: NS
    content: NS record includes
  - name: CNAME
    content: CNAME record includes
  - name: MX
    content: MX record includes
  - name: TXT
    content: TXT record includes
content_markdown: |-
left_code_blocks:
  - code_block: |-
      $ Invoke-RestMethod -Uri 'https://api.domainsdb.info/v1/domains/search?api_key=(api)&date=(date)&page=(page)&limit=(1)&domain=(google.com)&zone=(zone)&country=(country)&isDead=(false)&A=(A)&NS=(NS)&CNAME=(CNAME)&MX=(MX)&TXT=(TXT)'
    title:
    language: bash
right_code_blocks:
  - code_block: |-
        {
          "domains": [
            {
              "domain": "authentication-google.com",
              "create_date": "2020-07-24T04:59:54.337578",
              "update_date": "2021-07-03T05:48:25.980412",
              "country": "US",
              "isDead": false,
              "A": [
                "34.98.99.30"
              ],
              "NS": [
                "ns51.domaincontrol.com",
                "ns52.domaincontrol.com"
              ],
              "CNAME": null,
              "MX": null,
              "TXT": null
            },
            ...
          ],
          "total": 929,
          "time": 361,
          "next_page": null
        }
    title: Response
    language: json

---