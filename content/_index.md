---
title: ''
date: 2025-11-12
type: landing
design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      css_class: hbx-bg-gradient
      avatar:
        size: xl
        shape: circle
  
  - block: markdown
    content:
      title: 'Professional Focus'
      subtitle: ''
      text: |-
        I am a dual-degree graduate student pursuing my Master of Healthcare Administration (MHA) and Master of Public Health (MPH), with a focus on advancing health equity, improving healthcare operations, and strengthening community health systems. Through my capstone work and professional experience, I apply evidence-based strategies to address healthcare challenges and promote organizational excellence.
    design:
      columns: '1'
  
  - block: collection
    id: projects
    content:
      title: Capstone Projects
      filters:
        folders:
          - projects
    design:
      view: card
      columns: 2
  
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      count: 5
      filters:
        folders:
          - news
        exclude_featured: false
        exclude_future: false
        exclude_past: false
      offset: 0
      order: desc
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]
  
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle: ''
      text: "I'm available for collaboration, consultation, and professional opportunities in healthcare administration and public health."
      email: kamelliahyacinth@gmail.com
      phone: 608-571-8876
      address:
        street: ''
        city: Fitchburg
        region: WI
        postcode: '53713'
        country: United States
        country_code: US
      office_hours:
        - 'Monday - Friday: 9:00 AM - 3:00 PM'
        - 'Saturday: Closed'
        - 'Sunday: Closed'
      contact_links:
        - icon: linkedin
          icon_pack: fab
          name: LinkedIn
          link: https://www.linkedin.com/in/kamellia
      autolink: true
    design:
      columns: '2'
---
