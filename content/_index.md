---
# Leave the homepage title empty to use the site title
title: 'Kamellia Hyacinth'
summary: ''
date: 2026-01-05
type: landing

design:
  # Default section spacing
  spacing: '0'

sections:

  # Developer Hero - Gradient background with name, role, social, and CTAs
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hi, I'm"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "I focus on"
        strings:
          - "public health systems"
          - "healthcare quality"
          - "policy and compliance"
          - "community health impact"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: View My Work
          url: "#projects"
          icon: arrow-down
        - text: Get In Touch
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]

  # Filterable Portfolio
  - block: portfolio
    id: projects
    content:
      title: "Featured Projects"
      subtitle: "A selection of my recent work"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
        - name: Full-Stack
          tag: Full-Stack
        - name: Frontend
          tag: Frontend
        - name: Backend
          tag: Backend
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Core Competencies
  - block: tech-stack
    id: skills
    content:
      title: "Core Competencies"
      subtitle: "Public health policy, healthcare operations, and regulatory compliance expertise"

      categories:
        - name: Policy & Compliance
          items:
            - name: Regulatory Compliance
              icon: hero/shield-check
            - name: Policy Analysis
              icon: hero/document-magnifying-glass
            - name: Regulatory Gap Analysis
              icon: hero/clipboard-document-check
            - name: Policy Implementation
              icon: hero/document-text

        - name: Healthcare Operations
          items:
            - name: Clinical Operations
              icon: hero/building-office-2
            - name: Workflow Coordination
              icon: hero/cog-6-tooth
            - name: Process Improvement
              icon: hero/arrow-path
            - name: Program Administration
              icon: hero/briefcase

        - name: Research & Data
          items:
            - name: Program Evaluation
              icon: hero/chart-bar
            - name: Data Analysis
              icon: hero/chart-pie
            - name: Reporting & Documentation
              icon: hero/document-chart-bar
            - name: Systems Implementation
              icon: hero/circle-stack

        - name: Leadership & Collaboration
          items:
            - name: Project Coordination
              icon: hero/calendar-days
            - name: Stakeholder Engagement
              icon: hero/user-group
            - name: Strategic Communication
              icon: hero/chat-bubble-left-right
            - name: Health Equity
              icon: hero/scale

    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Experience Timeline
  - block: resume-experience
    id: experience
    content:
      title: Experience
      date_format: Jan 2006
      items:
        - title: Community Health & Policy Intern 
          company: Children's Wisconsin
          company_url: 'https://childrenswi.org'
          company_logo: ''
          location: Remote
          date_start: '2023-01-01'
          date_end: ''
          description: |2-
            * Conduct policy research and environmental scans supporting youth vaping prevention initiatives and school health policy development.
            * Support Community Health Needs Assessment (CHNA) Implementation Strategy initiatives focused on population health improvement and community benefit priorities.
            * Contribute to development, implementation, and evaluation of evidence-based community health programs addressing youth risk behaviors.
            * Tech stack: React, Node.js, PostgreSQL, AWS
        - title: Clinical Operations Coordinator
          company: SSM Health
          company_url: 'https://www.ssmhealth.com'
          company_logo: ''
          location: Madison, WI
          date_start: '2021-06-01'
          date_end: '2022-12-31'
          description: |2-
            * Served as sole operations support for two audiology providers, independently managing daily clinic workflow.
            * Collaborated with design team on UI/UX improvements
            * Tech stack: Next.js, Express, MongoDB, Docker
        - title: CBRF Compliance & Policy Intern 
          company: Circle of Hope Inc. II
          company_url: ''
          company_logo: ''
          location: Eau Claire, WI
          date_start: '2020-01-01'
          date_end: '2021-05-31'
          description: |2-
            * Developed client websites using modern web technologies
            * Maintained and updated legacy codebases
            * Participated in code reviews and agile ceremonies
            * Tech stack: React, WordPress, PHP, MySQL

    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Recent Blog Posts
  - block: collection
    id: blog
    content:
      title: Recent Posts
      subtitle: 'Thoughts on web development, tech, and more'
      text: ''
      filters:
        folders:
          - blog
        exclude_featured: false
      count: 3
      order: desc

    design:
      view: card
      columns: 3
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Contact Section
  - block: contact-info
    id: contact
    content:
      title: Get In Touch
      subtitle: "Let's connect on public health and healthcare initiatives"
      text: |-
        I'm always interested in opportunities to contribute to public health and healthcare improvement initiatives.
        Whether you're interested in collaboration, professional connections, or discussing shared interests in healthcare and policy, feel free to reach out.
      email: kamelliahyacinth@gmail.com
      autolink: true

    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # CTA Card
  - block: cta-card
    content:
      title: "Open to Opportunities"
      text: |-
        I'm currently seeking opportunities to contribute to public health, healthcare systems improvement, and policy development.

        Let's connect and discuss how I can help your team.
      button:
        text: 'Download Résumé'
        url: uploads/resume.pdf
        new_tab: true

    design:
      card:
        css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
        text_color: dark

      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"

      spacing:
        padding: ["4rem", "0", "6rem", "0"]

---
