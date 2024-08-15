---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
sections:
  - block: slider
    content:
      slides:
      - title: 👋 Welcome to SKKU LAB
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
      # Automatically transition through slides?
      loop: false
      # Duration of transition between slides (in ms)
      interval: 2000

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
      title: Latest Preprints
      text: ""
      count: 5
      filters:
        folders:
          - publication
        publication_type: 'article'
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
