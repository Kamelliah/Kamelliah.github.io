---
title: "Kamellia Hyacinth"
summary: ""
date: 2026-01-05
type: landing

design:
  spacing: "0"

sections:
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hi, I'm"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "My work focuses on"
        strings:
          - "public health systems improvement."
          - "healthcare quality and compliance."
          - "health policy and population health."
          - "community health impact."
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: "View Experience"
          url: "#experience"
          icon: arrow-down
        - text: "Contact Me"
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

  - block: portfolio
    id: projects
    content:
      title: "Selected Work"
      subtitle: "Public health, healthcare administration, and systems improvement projects"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: "All"
          tag: "*"
        - name: "Public Health"
          tag: "Public Health"
        - name: "Health Policy"
          tag: "Health Policy"
        - name: "Healthcare Operations"
          tag: "Healthcare Operations"
        - name: "Quality Improvement"
          tag: "Quality Improvement"
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: tech-stack
    id: skills
    content:
      title: "Core Competencies"
      subtitle: "Healthcare administration, public health policy, and regulatory compliance expertise"
      categories:
        - name: "Policy & Compliance"
          items:
            - name: "Regulatory Compliance"
              icon: hero/shield-check
            - name: "Policy Analysis"
              icon: hero/document-magnifying-glass
            - name: "Regulatory Gap Analysis"
              icon: hero/clipboard-document-check
            - name: "Policy Implementation"
              icon: hero/document-text
        - name: "Healthcare Administration"
          items:
            - name: "Healthcare Operations"
              icon: hero/building-office-2
            - name: "Clinical Workflow Coordination"
              icon: hero/cog-6-tooth
            - name: "Quality Improvement"
              icon: hero/arrow-path
            - name: "Program Coordination"
              icon: hero/briefcase
        - name: "Research & Data"
          items:
            - name: "Program Evaluation"
              icon: hero/chart-bar
            - name: "Data Analysis"
              icon: hero/chart-pie
            - name: "Reporting & Documentation"
              icon: hero/document-chart-bar
            - name: "Population Health Analysis"
              icon: hero/circle-stack
        - name: "Leadership & Collaboration"
          items:
            - name: "Project Coordination"
              icon: hero/calendar-days
            - name: "Stakeholder Engagement"
              icon: hero/user-group
            - name: "Strategic Communication"
              icon: hero/chat-bubble-left-right
            - name: "Health Equity Advocacy"
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

  - block: resume-experience
    id: experience
    content:
      title: "Experience"
      date_format: "Jan 2006"
      items:
        - title: "Community Health & Policy Intern (Incoming)"
          company: "Children's Wisconsin"
          company_url: "https://childrenswi.org"
          company_logo: "childrens-wisconsin.png"
          location: "Wisconsin"
          date_start: "2026-05-01"
          date_end: ""
          description: |-
            Incoming beginning May 2026.
            Selected to support community health and policy initiatives focused on prevention, population health, and community-based improvement efforts.
            Expected responsibilities include supporting community health needs assessment activities, policy research, program implementation support, and health equity initiatives.
        - title: "Audiology Clinical Operations Coordinator"
          company: "SSM Health"
          company_url: "https://www.ssmhealth.com"
          company_logo: ""
          location: "Madison, Wisconsin"
          date_start: "2025-07-28"
          date_end: "2026-02-13"
          description: |-
            Coordinated clinical operations supporting patient scheduling, provider workflow efficiency, and daily service delivery.
            Supported operational compliance, administrative coordination, and process improvement efforts within a healthcare setting.
            Contributed to clinic efficiency and continuity of care through organized workflow support and accurate documentation.
        - title: "CBRF Compliance & Policy Intern"
          company: "Circle of Hope Inc. II"
          company_url: ""
          company_logo: ""
          location: "Wisconsin"
          date_start: "2020-01-01"
          date_end: "2021-05-31"
          description: |-
            Supported internal compliance efforts through policy review, documentation updates, and workforce process improvement.
            Assisted with onboarding materials, employee policy development, and organizational alignment with regulatory expectations.
            Contributed to administrative systems improvement supporting staff operations and compliance readiness.
    design:
      columns: "1"
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: collection
    id: blog
    content:
      title: "Recent Writing"
      subtitle: "Public health policy, healthcare systems, and population health perspectives"
      text: ""
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

  - block: contact-info
    id: contact
    content:
      title: "Contact"
      subtitle: "Professional connections and collaboration opportunities"
      text: |-
        I welcome opportunities to contribute to public health initiatives, healthcare systems improvement efforts, and policy development work.
        I am especially interested in roles involving healthcare quality, regulatory compliance, and population health improvement.
        Feel free to reach out regarding collaboration, professional opportunities, or shared interests in healthcare and public health.
      email: "kamelliahyacinth@gmail.com"
      autolink: true
    design:
      columns: "1"
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: cta-card
    content:
      title: "Open to Public Health & Healthcare Opportunities"
      text: |-
        Currently pursuing opportunities in public health policy, healthcare administration, and health systems improvement.
        Interested in roles involving healthcare quality, compliance, and population health strategy.
      button:
        text: "Download Resume"
        url: "uploads/resume.pdf"
        new_tab: true
    design:
      card:
        css_class: "bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700"
        text_color: dark
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---
