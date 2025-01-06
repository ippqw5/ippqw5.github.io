---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      image:
        filename: logo_tail.png
      cta:
        label: Meet Us  
        url: people
      text: |
        TIC is a laboratory dedicated to trustworthy artificial intelligence research, affiliated with the School of Software Engineering at East China Normal University. Our goal is to develop safe, reliable, and transparent AI systems.

        Our research directions include:
        - Neural network robustness
        - Robustness of reinforcement learning systems
        - Large model testing

    # design:
    #   # Choose an optional background color, gradient, image, or video
    #   background:
    #     gradient_end: '#1976d2'
    #     gradient_start: '#004ba0'
    #     text_color_light: true

  - block: collection
    content:
      title: Latest News
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
      view: card
      columns: '1'
  
  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image: 
          filename: disei.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen
---
