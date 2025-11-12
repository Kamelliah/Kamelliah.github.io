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
  
  - block: markdown
    id: contact
    content:
      title: Contact
      text: |-
        **Get in Touch**
        
        I'm available for collaboration, consultation, and professional opportunities in healthcare administration and public health.
        
        📧 **Email:** [kamelliahyacinth@gmail.com](mailto:kamelliahyacinth@gmail.com)
        
        📞 **Phone:** 608-571-8876
        
        📍 **Location:** Fitchburg, WI 53713
        
        ⏰ **Hours:** Monday - Friday, 9:00 AM - 3:00 PM
        
        🔗 **LinkedIn:** [linkedin.com/in/kamellia](https://www.linkedin.com/in/kamellia)
        
        ---
        
        [Visit my full contact page →](/contact/)
    design:
      columns: '1'
---
