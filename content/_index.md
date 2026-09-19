---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: slider
    content:
      # Append the newest publications after the welcome slide at build time.
      latest_publication:
        enable: true
        count: 3
      slides:
      - title: 👋 Welcome to 솜씨 랩
        content: "성균관대학교 소셜빅데이터 연구실"
        align: center
        background:
          image:
            filename: skkubg.jpg
            filters:
              brightness: 0.7
          position: right
          color: '#666'
        link:
          icon: graduation-cap
          icon_pack: fas
          text: Members
          url: ../people/
        
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: ''
      is_fullscreen: true
      # Hide the previous/next arrows while keeping autoplay and indicators.
      show_controls: false
      # Automatically transition through slides?
      loop: true
      # Duration of transition between slides (in ms)
      interval: 5000

  - block: collection
    content:
      title: 최신 뉴스
      subtitle:
      text:
      count: 5
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: showcase
      columns: '1'
  
  - block: collection
    content:
      title: Latest Publications
      text: ""
      count: 5
      filters:
        folders:
          - publication

    design:
      view: citation
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the Members →" %}}
    design:
      columns: '1'
---
