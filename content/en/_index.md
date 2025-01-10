---
# Leave the homepage title empty to use the site title
title: home
type: landing

sections:
  - block: slider
    content:
      slides:
        - title: Welcome to TIC LAB
          # content: Take a look at what we're working on...
          align: center
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: dishuihu.jpg
              filters:
                brightness: 0.7
            position: right
            color: '#666'
        - title: TIC LAB ☕️
          content: 'Share your knowledge with the group and explore exciting new topics together!'
          align: right
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: disei.jpg
              filters:
                brightness: 0.5
            position: center
            color: '#333'
          link:
            icon: graduation-cap
            icon_pack: fas
            text: Our Research Topics
            url: topic
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: '300px'
      # Make the slides full screen within the browser window?
      is_fullscreen: false
      # Automatically transition through slides?
      loop: false
      # Duration of transition between slides (in ms)
      interval: 2000

  - block: hero
    content:
      image:
        filename: logo_tail.png
      cta:
        label: Meet Us  
        url: people
      text: |
        **TIC** is a laboratory dedicated to trustworthy artificial intelligence research, affiliated with the School of Software Engineering at East China Normal University. Our goal is to develop safe, reliable, and transparent AI systems.

        Our research directions include:
        - Robustness verification and training of deep neural networks
        - Reliability training and verification of reinforcement learning system
        - LLM Testing
  
  - block: collection
    content:
      title: Latest Publications
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        # The folders to display content from
        folders:
          - publication
        author: ""
        category: ""
        tag: ""
        publication_type: ""
        featured_only: false
        exclude_featured: false
        exclude_future: false
        exclude_past: false
      # Choose how many pages you would like to offset by
      # Useful if you wish to show the first item in the Featured widget
      offset: 0
      # Field to sort by, such as Date or Title
      sort_by: 'Date'
      sort_ascending: false
    design:
      # Choose a listing view
      view: compact
      # Choose single or dual column layout
      columns: '2'
  
  - block: collection
    content:
      title: Latest News
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        # The folders to display content from
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        publication_type: ""
        featured_only: false
        exclude_featured: false
        exclude_future: false
        exclude_past: false
      # Choose how many pages you would like to offset by
      # Useful if you wish to show the first item in the Featured widget
      offset: 0
      # Field to sort by, such as Date or Title
      sort_by: 'Date'
      sort_ascending: false
    design:
      # Choose a listing view
      view: compact
      # Choose single or dual column layout
      columns: '2'


  - block: portfolio
    id: projects
    content:
      title: Main Research Topics
      filters:
        # Folders to display content from
        folders:
          - topic
      design:
        # Choose a listing view
        view: compact
        # Choose single or dual column layout
        columns: '2'
---
