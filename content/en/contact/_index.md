---
title: Contact
date: 2025-01-11

type: landing

sections:
  - block: contact
    content:
      title: Contact
      # text: test test test
      email: xxx@163.com
      #phone: 888 888 88 88
      address:
        street: 111 Nan Mu road
        city: Shanghai
        region: Pudong
        # postcode: '94305'
        country: China
        country_code: CN
      coordinates:
        latitude: '30.902773'
        longitude: '121.918800'
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      office_hours:
        - 'Monday 10:00 to 13:00'
        - 'Wednesday 09:00 to 10:00'
      # appointment_url: 'https://calendly.com'
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
  
      # Automatically link email and phone or display as text?
      autolink: true
  
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
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
          filename: ECNU_DISEI.png
          filters:
            brightness: 1
          parallax: false
          # position: center
          # size: fix
          # text_color_light: true
      # spacing:
        # padding: ['20px', '0', '20px', '0']
      # css_class: fullscreen
---
