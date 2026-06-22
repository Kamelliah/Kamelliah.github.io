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
    id: seo-person
    content:
      title: ""
      text: |-
        {{< rawhtml >}}
        <script type="application/ld+json">
        {
          "@context": "https://schema.org",
          "@type": "Person",
          "name": "Kamellia Hyacinth",
          "url": "https://kamelliah.github.io",
          "email": "kamelliahyacinth@gmail.com",
          "jobTitle": "Public Health Policy, Systems & Compliance Professional",
          "description": "MPH candidate, Army veteran, and public health policy professional based in Fitchburg, WI. Focused on regulatory compliance, health systems, and Wisconsin state health policy.",
          "image": "https://kamelliah.github.io/media/icon_hu_52c4a216464a8cfe.png",
          "alumniOf": [
            {"@type": "EducationalOrganization", "name": "University of Wisconsin Milwaukee", "url": "https://uwm.edu"},
            {"@type": "EducationalOrganization", "name": "University of Wisconsin La Crosse", "url": "https://www.uwlax.edu"},
            {"@type": "EducationalOrganization", "name": "St. George's University", "url": "https://www.sgu.edu"}
          ],
          "sameAs": [
            "https://www.linkedin.com/in/kamellia/",
            "https://github.com/kamelliah",
            "https://www.instagram.com/kamelliah/"
          ]
        }
        </script>
        {{< /rawhtml >}}
    design:
      spacing:
        padding: ["0", "0", "0", "0"]
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
  - block: portfolio
    id: blog
    content:
      title: "Recent Writing"
      subtitle: "Public health policy, healthcare systems, and population health perspectives"
      count: 0
      filters:
        folders:
          - blog
      buttons:
        - name: "All"
          tag: "*"
        - name: "Public Health"
          tag: "Public Health"
        - name: "Health Equity"
          tag: "Health Equity"
        - name: "Policy"
          tag: "Policy"
        - name: "Systems Design"
          tag: "Systems Design"
    design:
      columns: 3
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  - block: markdown
    id: contact
    content:
      title: ""
      text: |-
        {{< rawhtml >}}
        <style>
          .kh-contact-section {
            max-width: 860px;
            margin: 0 auto;
            text-align: center;
          }
          .kh-status-pill {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            background: rgba(34,197,94,0.12);
            border: 1px solid rgba(34,197,94,0.3);
            color: #16a34a;
            font-size: 0.75rem;
            font-weight: 600;
            letter-spacing: 0.08em;
            text-transform: uppercase;
            padding: 0.35rem 1rem;
            border-radius: 9999px;
            margin-bottom: 1.75rem;
          }
          .dark .kh-status-pill {
            color: #4ade80;
            background: rgba(74,222,128,0.1);
            border-color: rgba(74,222,128,0.25);
          }
          .kh-contact-heading {
            font-size: clamp(2.25rem, 5vw, 3.5rem);
            font-weight: 800;
            letter-spacing: -0.02em;
            line-height: 1.1;
            margin: 0 0 1rem;
            background: linear-gradient(135deg, #1e293b 0%, #475569 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
          }
          .dark .kh-contact-heading {
            background: linear-gradient(135deg, #f8fafc 0%, #94a3b8 100%);
            -webkit-background-clip: text;
            background-clip: text;
          }
          .kh-contact-sub {
            font-size: 1.1rem;
            color: #64748b;
            max-width: 520px;
            margin: 0 auto 3rem;
            line-height: 1.65;
          }
          .dark .kh-contact-sub { color: #94a3b8; }
          .kh-cards-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1.25rem;
            margin-bottom: 2rem;
          }
          @media (max-width: 560px) {
            .kh-cards-grid { grid-template-columns: 1fr; }
          }
          .kh-card {
            display: flex;
            align-items: center;
            gap: 1rem;
            padding: 1.4rem 1.5rem;
            border-radius: 1rem;
            background: #ffffff;
            border: 1px solid rgba(0,0,0,0.07);
            box-shadow: 0 1px 3px rgba(0,0,0,0.06), 0 4px 16px rgba(0,0,0,0.04);
            text-decoration: none;
            color: inherit;
            transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
            text-align: left;
          }
          .kh-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 8px 30px rgba(0,0,0,0.12);
            border-color: rgba(99,102,241,0.3);
            text-decoration: none;
            color: inherit;
          }
          .dark .kh-card {
            background: rgba(255,255,255,0.04);
            border-color: rgba(255,255,255,0.08);
            box-shadow: 0 1px 3px rgba(0,0,0,0.3);
          }
          .dark .kh-card:hover {
            background: rgba(255,255,255,0.07);
            border-color: rgba(139,92,246,0.4);
            box-shadow: 0 8px 30px rgba(0,0,0,0.4);
          }
          .kh-card-icon {
            width: 48px;
            height: 48px;
            border-radius: 0.75rem;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.4rem;
            flex-shrink: 0;
          }
          .kh-card-label {
            font-size: 0.7rem;
            font-weight: 600;
            letter-spacing: 0.1em;
            text-transform: uppercase;
            color: #94a3b8;
            margin-bottom: 0.2rem;
          }
          .kh-card-value {
            font-size: 0.95rem;
            font-weight: 600;
            color: #1e293b;
          }
          .dark .kh-card-value { color: #f1f5f9; }
          .kh-card-arrow {
            margin-left: auto;
            color: #cbd5e1;
            font-size: 1.1rem;
            transition: transform 0.2s ease, color 0.2s ease;
          }
          .kh-card:hover .kh-card-arrow {
            transform: translateX(3px);
            color: #6366f1;
          }
          .dark .kh-card:hover .kh-card-arrow { color: #818cf8; }
          .kh-location-strip {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 0.85rem;
            color: #94a3b8;
            margin-top: 0.5rem;
          }
        </style>

        <div class="kh-contact-section">
          <div><span class="kh-status-pill">&#9679; Open to Opportunities</span></div>
          <h2 class="kh-contact-heading">Let&rsquo;s Connect</h2>
          <p class="kh-contact-sub">
            Available for roles in public health policy, healthcare administration, and regulatory compliance.
            Open to remote and Wisconsin-based opportunities.
          </p>

          <div class="kh-cards-grid">

            <a href="mailto:kamelliahyacinth@gmail.com" class="kh-card">
              <div class="kh-card-icon" style="background:rgba(239,68,68,0.1);">✉️</div>
              <div>
                <div class="kh-card-label">Email</div>
                <div class="kh-card-value">kamelliahyacinth@gmail.com</div>
              </div>
              <span class="kh-card-arrow">›</span>
            </a>

            <a href="https://www.linkedin.com/in/kamellia/" target="_blank" rel="noopener noreferrer" class="kh-card">
              <div class="kh-card-icon" style="background:rgba(10,102,194,0.1);">
                <svg width="22" height="22" viewBox="0 0 24 24" fill="#0a66c2"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
              </div>
              <div>
                <div class="kh-card-label">LinkedIn</div>
                <div class="kh-card-value">linkedin.com/in/kamellia</div>
              </div>
              <span class="kh-card-arrow">›</span>
            </a>

            <a href="/uploads/resume.pdf" target="_blank" rel="noopener noreferrer" class="kh-card">
              <div class="kh-card-icon" style="background:rgba(16,185,129,0.1);">📄</div>
              <div>
                <div class="kh-card-label">Resume</div>
                <div class="kh-card-value">Download PDF</div>
              </div>
              <span class="kh-card-arrow">›</span>
            </a>

            <a href="https://www.instagram.com/kamelliah/" target="_blank" rel="noopener noreferrer" class="kh-card">
              <div class="kh-card-icon" style="background:rgba(217,70,239,0.1);">📸</div>
              <div>
                <div class="kh-card-label">Instagram</div>
                <div class="kh-card-value">@kamelliah</div>
              </div>
              <span class="kh-card-arrow">›</span>
            </a>

          </div>

          <div class="kh-location-strip">
            <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
            Fitchburg, Wisconsin &nbsp;&middot;&nbsp; Remote-friendly
          </div>
        </div>
        {{< /rawhtml >}}
    design:
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["5rem", "0", "5rem", "0"]
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
            "St. George's University": "https://www.sgu.edu",
            "Children's Wisconsin": "https://childrenswi.org",
            "SSM Health": "https://www.ssmhealth.com",
            "MKE FreshAir Collective": "https://www.mkefreshair.com",
            "Circle Of Hope Inc. II": "https://circleofhopell.com"
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
