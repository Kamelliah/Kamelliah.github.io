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
  - block: markdown
    id: countdown
    content:
      title: ""
      text: |-
        {{< rawhtml >}}
        <div style="text-align:center; padding:0.5rem 0;">
          <p style="font-size:0.75rem; font-weight:600; letter-spacing:0.12em; text-transform:uppercase; opacity:0.5; margin:0 0 1.25rem;">MPH Graduation &middot; May 17, 2027</p>
          <div id="mph-countdown" style="display:inline-flex; gap:1rem; flex-wrap:wrap; justify-content:center;">
            <div style="display:flex;flex-direction:column;align-items:center;background:rgba(128,128,128,0.08);border:1px solid rgba(128,128,128,0.15);border-radius:0.75rem;padding:1.25rem 1.75rem;min-width:88px;">
              <span id="cd-days"  style="font-size:2.75rem;font-weight:700;line-height:1;font-variant-numeric:tabular-nums;letter-spacing:-0.02em;">--</span>
              <span style="font-size:0.7rem;font-weight:600;letter-spacing:0.1em;text-transform:uppercase;opacity:0.5;margin-top:0.4rem;">Days</span>
            </div>
            <div style="display:flex;flex-direction:column;align-items:center;background:rgba(128,128,128,0.08);border:1px solid rgba(128,128,128,0.15);border-radius:0.75rem;padding:1.25rem 1.75rem;min-width:88px;">
              <span id="cd-hours" style="font-size:2.75rem;font-weight:700;line-height:1;font-variant-numeric:tabular-nums;letter-spacing:-0.02em;">--</span>
              <span style="font-size:0.7rem;font-weight:600;letter-spacing:0.1em;text-transform:uppercase;opacity:0.5;margin-top:0.4rem;">Hours</span>
            </div>
            <div style="display:flex;flex-direction:column;align-items:center;background:rgba(128,128,128,0.08);border:1px solid rgba(128,128,128,0.15);border-radius:0.75rem;padding:1.25rem 1.75rem;min-width:88px;">
              <span id="cd-mins"  style="font-size:2.75rem;font-weight:700;line-height:1;font-variant-numeric:tabular-nums;letter-spacing:-0.02em;">--</span>
              <span style="font-size:0.7rem;font-weight:600;letter-spacing:0.1em;text-transform:uppercase;opacity:0.5;margin-top:0.4rem;">Minutes</span>
            </div>
            <div style="display:flex;flex-direction:column;align-items:center;background:rgba(128,128,128,0.08);border:1px solid rgba(128,128,128,0.15);border-radius:0.75rem;padding:1.25rem 1.75rem;min-width:88px;">
              <span id="cd-secs"  style="font-size:2.75rem;font-weight:700;line-height:1;font-variant-numeric:tabular-nums;letter-spacing:-0.02em;">--</span>
              <span style="font-size:0.7rem;font-weight:600;letter-spacing:0.1em;text-transform:uppercase;opacity:0.5;margin-top:0.4rem;">Seconds</span>
            </div>
          </div>
        </div>
        <script>
        (function(){
          var target = new Date('2027-05-17T10:00:00');
          function pad(n){ return String(n).padStart(2,'0'); }
          function tick(){
            var diff = target - new Date();
            if(diff <= 0){
              document.getElementById('mph-countdown').innerHTML =
                '<span style="font-size:1.25rem;font-weight:600;">🎓 Graduated!</span>';
              return;
            }
            document.getElementById('cd-days').textContent  = pad(Math.floor(diff/86400000));
            document.getElementById('cd-hours').textContent = pad(Math.floor(diff%86400000/3600000));
            document.getElementById('cd-mins').textContent  = pad(Math.floor(diff%3600000/60000));
            document.getElementById('cd-secs').textContent  = pad(Math.floor(diff%60000/1000));
          }
          tick();
          setInterval(tick,1000);
        })();
        </script>
        {{< /rawhtml >}}
    design:
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["2rem", "0", "3rem", "0"]
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
        - name: "Healthcare Administration"
          tag: "Healthcare Administration"
        - name: "Operations Improvement"
          tag: "Operations Improvement"
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
        - title: "Community Health & Policy Intern"
          company: "Children's Wisconsin"
          company_url: "https://childrenswi.org"
          company_logo: "childrens-wisconsin.png"
          location: "Wisconsin"
          date_start: "2026-06-01"
          description: |-
            Supported community health and prevention initiatives through program coordination and policy research.
            Assisted with community needs assessments, data analysis, and reporting to support population health strategies.
            Contributed to initiatives addressing health disparities and improving access to care.
        - title: "Public Policy & Community Health Intern"
          company: "MKE FreshAir Collective"
          company_url: ""
          company_logo: ""
          location: "Milwaukee, Wisconsin"
          date_start: "2026-06-01"
          description: |-
            Analyzed air quality sensor data across Milwaukee's marginalized neighborhoods to identify environmental health disparities.
            Drafted policy briefs and research summaries translating findings into advocacy materials.
            Led community engagement and managed air sensor network operations.
        - title: "Audiology Clinical Operations Coordinator"
          company: "SSM Health"
          company_url: "https://www.ssmhealth.com"
          company_logo: ""
          location: "Madison, Wisconsin"
          date_start: "2025-07-28"
          date_end: "2026-02-13"
          description: |-
            Coordinated clinical workflows, scheduling operations, and patient service processes.
            Supported operational efficiency and compliance with healthcare organizational standards.
        - title: "CBRF Compliance & Policy Intern"
          company: "Circle of Hope Inc. II"
          company_url: ""
          company_logo: ""
          location: "Wisconsin"
          date_start: "2024-01-01"
          date_end: "2025-05-31"
          description: |-
            Assisted with compliance review and organizational policy development including contributions to employee handbook improvements.
            Supported workforce system improvements related to onboarding processes, staff policies, and regulatory compliance requirements.
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
  - block: markdown
    content:
      title: ""
      text: |-
        {{< rawhtml >}}
        <script>
        document.addEventListener('DOMContentLoaded', function() {
          var links = {
            "University of Wisconsin Milwaukee": "https://uwm.edu",
            "University of Wisconsin La Crosse": "https://www.uwlax.edu",
            "St. George’s University": "https://www.sgu.edu",
            "Children’s Wisconsin": "https://childrenswi.org",
            "SSM Health": "https://www.ssmhealth.com",
            "MKE FreshAir Collective": "https://www.mkefreshair.com"
          };
          document.querySelectorAll('p').forEach(function(p) {
            var text = p.textContent.trim();
            if (links[text]) {
              var a = document.createElement('a');
              a.href = links[text];
              a.target = '_blank';
              a.rel = 'noopener noreferrer';
              a.textContent = text;
              a.style.color = 'inherit';
              a.style.textDecoration = 'underline';
              a.style.textDecorationColor = 'rgba(128,128,128,0.35)';
              a.style.textUnderlineOffset = '2px';
              while (p.firstChild) p.removeChild(p.firstChild);
              p.appendChild(a);
            }
          });
        });
        </script>
        {{< /rawhtml >}}
    design:
      spacing:
        padding: ["0", "0", "0", "0"]
---
