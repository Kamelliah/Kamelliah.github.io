---
title: "About"
type: landing
design:
  spacing: "0"
sections:
  - block: dev-hero
    id: about-hero
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
          - "regulatory compliance and strategy."
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: "My Experience"
          url: "#about-experience"
          icon: arrow-down
        - text: "Contact Me"
          url: "/#contact"
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

  - block: markdown
    id: about-countdown
    content:
      title: ""
      text: |-
        {{< rawhtml >}}
        <div class="kh-cd-wrap">
          <p class="kh-cd-label">🎓 MPH Graduation &middot; May 17, 2027</p>
          <div id="about-mph-countdown" class="kh-cd-grid">
            <div class="kh-cd-cell"><span id="acd-days"  class="kh-cd-num">--</span><span class="kh-cd-unit">Days</span></div>
            <div class="kh-cd-cell"><span id="acd-hours" class="kh-cd-num">--</span><span class="kh-cd-unit">Hours</span></div>
            <div class="kh-cd-cell"><span id="acd-mins"  class="kh-cd-num">--</span><span class="kh-cd-unit">Mins</span></div>
            <div class="kh-cd-cell"><span id="acd-secs"  class="kh-cd-num">--</span><span class="kh-cd-unit">Secs</span></div>
          </div>
        </div>
        <script>
        (function(){
          var target = new Date('2027-05-17T10:00:00');
          function pad(n){ return String(n).padStart(2,'0'); }
          function tick(){
            var diff = target - new Date();
            if(diff <= 0){
              document.getElementById('about-mph-countdown').innerHTML =
                '<span style="font-size:1.25rem;font-weight:700;color:#6366f1;">🎓 Graduated!</span>';
              return;
            }
            document.getElementById('acd-days').textContent  = pad(Math.floor(diff/86400000));
            document.getElementById('acd-hours').textContent = pad(Math.floor(diff%86400000/3600000));
            document.getElementById('acd-mins').textContent  = pad(Math.floor(diff%3600000/60000));
            document.getElementById('acd-secs').textContent  = pad(Math.floor(diff%60000/1000));
          }
          tick(); setInterval(tick,1000);
        })();
        </script>
        {{< /rawhtml >}}
    design:
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["2rem", "0", "2rem", "0"]

  - block: resume-experience
    id: about-experience
    content:
      title: "Experience"
      items:
        - title: "Community Health & Policy Intern"
          company: "Children's Wisconsin"
          company_url: "https://childrenswi.org"
          date_start: 2026-06-01
          description: |-
            Supported community health and prevention initiatives through program coordination and policy research.
            Assisted with community needs assessments, data analysis, and reporting to support population health strategies.
            Contributed to initiatives addressing health disparities and improving access to care.

        - title: "Public Policy & Community Health Intern"
          company: "MKE FreshAir Collective"
          company_url: "https://www.mkefreshair.com"
          date_start: 2026-06-01
          description: |-
            Analyzed air quality sensor data across Milwaukee's marginalized neighborhoods to identify environmental health disparities.
            Drafted policy briefs and research summaries translating findings into advocacy materials.
            Led community engagement and managed air sensor network operations.

        - title: "Audiology Clinical Operations Coordinator"
          company: "SSM Health"
          company_url: "https://www.ssmhealth.com"
          date_start: 2025-07-28
          date_end: 2026-02-13
          description: |-
            Coordinated clinical workflows, scheduling operations, and patient service processes.
            Supported operational efficiency and compliance with healthcare organizational standards.

        - title: "CBRF Compliance & Policy Intern"
          company: "Circle Of Hope Inc. II"
          company_url: "https://circleofhopell.com"
          date_start: 2024-01-01
          date_end: 2025-05-31
          description: |-
            Assisted with compliance review and organizational policy development including employee handbook improvements.
            Supported workforce system improvements related to onboarding, staff policies, and regulatory compliance.
    design:
      columns: "1"
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: markdown
    id: about-cta
    content:
      title: ""
      text: |-
        **Want to connect or collaborate?** [Get in touch](/#contact) or [download my resume](/uploads/resume.pdf).
    design:
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["2.5rem", "0", "4rem", "0"]
---
