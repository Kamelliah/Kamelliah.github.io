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
          .kh-contact-wrap {
            width: min(1100px, calc(100vw - 3rem));
            position: relative;
            left: 50%;
            transform: translateX(-50%);
            text-align: center;
          }
          .kh-contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.5rem;
            text-align: left;
          }
          @media (max-width: 700px) {
            .kh-contact-grid { grid-template-columns: 1fr; }
          }
          .kh-map-panel {
            border-radius: 1.5rem;
            overflow: hidden;
            border: 1px solid rgba(0,0,0,0.08);
            box-shadow: 0 4px 6px rgba(0,0,0,0.04), 0 20px 60px rgba(0,0,0,0.07);
            min-height: 420px;
          }
          .dark .kh-map-panel {
            border-color: rgba(255,255,255,0.08);
            box-shadow: 0 4px 6px rgba(0,0,0,0.3), 0 20px 60px rgba(0,0,0,0.4);
          }
          #kh-map { width: 100%; height: 100%; min-height: 420px; }
          .kh-contact-heading {
            font-size: clamp(1.9rem, 4vw, 2.8rem);
            font-weight: 800;
            letter-spacing: -0.02em;
            line-height: 1.1;
            margin: 0 0 0.75rem;
            color: #0f172a;
          }
          .dark .kh-contact-heading { color: #f1f5f9; }
          .kh-contact-sub {
            font-size: 1rem;
            color: #64748b;
            margin: 0 auto 2.5rem;
            line-height: 1.7;
            max-width: 480px;
          }
          .dark .kh-contact-sub { color: #94a3b8; }
          .kh-box {
            position: relative;
            border-radius: 1.5rem;
            background: #fff;
            border: 1px solid rgba(0,0,0,0.08);
            box-shadow: 0 4px 6px rgba(0,0,0,0.04), 0 20px 60px rgba(0,0,0,0.07);
            overflow: hidden;
          }
          .dark .kh-box {
            background: rgba(255,255,255,0.03);
            border-color: rgba(255,255,255,0.08);
            box-shadow: 0 4px 6px rgba(0,0,0,0.3), 0 20px 60px rgba(0,0,0,0.4);
          }
          .kh-box-glow {
            position: absolute;
            top: -60px; left: 50%;
            transform: translateX(-50%);
            width: 400px; height: 200px;
            background: radial-gradient(ellipse, rgba(99,102,241,0.15) 0%, transparent 70%);
            pointer-events: none;
          }
          .dark .kh-box-glow {
            background: radial-gradient(ellipse, rgba(139,92,246,0.2) 0%, transparent 70%);
          }
          .kh-box-inner {
            position: relative;
            padding: 2rem 2rem 1.75rem;
            display: flex;
            flex-direction: column;
            gap: 2rem;
          }
          .kh-box-left { text-align: center; }
          .kh-box-tag {
            display: inline-flex;
            align-items: center;
            gap: 0.4rem;
            font-size: 0.7rem;
            font-weight: 700;
            letter-spacing: 0.1em;
            text-transform: uppercase;
            color: #22c55e;
            background: rgba(34,197,94,0.1);
            border: 1px solid rgba(34,197,94,0.2);
            padding: 0.25rem 0.75rem;
            border-radius: 9999px;
            margin-bottom: 1rem;
          }
          .dark .kh-box-tag {
            color: #4ade80;
            background: rgba(74,222,128,0.08);
            border-color: rgba(74,222,128,0.2);
          }
          .kh-box-title {
            font-size: 1.35rem;
            font-weight: 700;
            color: #0f172a;
            margin: 0 0 0.75rem;
            line-height: 1.3;
          }
          .dark .kh-box-title { color: #f1f5f9; }
          .kh-box-text {
            font-size: 0.9rem;
            color: #64748b;
            line-height: 1.7;
            margin: 0 0 1.5rem;
          }
          .dark .kh-box-text { color: #94a3b8; }
          .kh-email-btn {
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            background: #0f172a;
            color: #fff;
            font-size: 0.875rem;
            font-weight: 600;
            padding: 0.65rem 1.25rem;
            border-radius: 0.625rem;
            text-decoration: none;
            transition: background 0.2s, transform 0.15s;
          }
          .kh-email-btn:hover { background: #1e293b; transform: translateY(-1px); text-decoration: none; color: #fff; }
          .dark .kh-email-btn { background: #f1f5f9; color: #0f172a; }
          .dark .kh-email-btn:hover { background: #fff; }
          .kh-box-right { text-align: left; }
          .kh-links-label {
            font-size: 0.7rem;
            font-weight: 700;
            letter-spacing: 0.1em;
            text-transform: uppercase;
            color: #94a3b8;
            margin-bottom: 0.9rem;
          }
          .kh-links-list {
            display: flex;
            flex-direction: column;
            gap: 0.6rem;
          }
          .kh-link-row {
            display: flex;
            align-items: center;
            gap: 0.85rem;
            padding: 0.7rem 0.85rem;
            border-radius: 0.75rem;
            text-decoration: none;
            color: #1e293b;
            border: 1px solid rgba(0,0,0,0.06);
            background: rgba(0,0,0,0.02);
            transition: background 0.15s, border-color 0.15s, transform 0.15s;
            font-size: 0.875rem;
            font-weight: 500;
          }
          .kh-link-row:hover {
            background: rgba(99,102,241,0.06);
            border-color: rgba(99,102,241,0.2);
            transform: translateX(3px);
            text-decoration: none;
            color: #1e293b;
          }
          .dark .kh-link-row {
            color: #e2e8f0;
            background: rgba(255,255,255,0.03);
            border-color: rgba(255,255,255,0.07);
          }
          .dark .kh-link-row:hover {
            background: rgba(139,92,246,0.08);
            border-color: rgba(139,92,246,0.25);
            color: #e2e8f0;
          }
          .kh-link-icon {
            width: 32px; height: 32px;
            border-radius: 0.5rem;
            display: flex; align-items: center; justify-content: center;
            font-size: 1rem;
            flex-shrink: 0;
          }
          .kh-link-meta { flex: 1; }
          .kh-link-name { font-weight: 600; font-size: 0.85rem; display: block; }
          .kh-link-handle { font-size: 0.75rem; color: #94a3b8; }
          .kh-link-arrow { color: #cbd5e1; font-size: 0.85rem; transition: transform 0.15s; }
          .kh-link-row:hover .kh-link-arrow { transform: translateX(2px); color: #6366f1; }
          .dark .kh-link-row:hover .kh-link-arrow { color: #818cf8; }
          .kh-box-footer {
            border-top: 1px solid rgba(0,0,0,0.06);
            padding: 1rem 2.5rem;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
            font-size: 0.8rem;
            color: #94a3b8;
          }
          .dark .kh-box-footer { border-color: rgba(255,255,255,0.06); }
        </style>

        <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"/>
        <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>

        <div class="kh-contact-wrap">
          <h2 class="kh-contact-heading">Get in Touch</h2>

          <div class="kh-contact-grid">
          <div class="kh-box">
            <div class="kh-box-glow"></div>
            <div class="kh-box-inner">

              <div class="kh-box-left">
                <div class="kh-box-tag">
                  <svg width="7" height="7" viewBox="0 0 8 8"><circle cx="4" cy="4" r="4" fill="currentColor"/></svg>
                  Open to Opportunities
                </div>
                <div class="kh-box-title">Public Health &amp; Healthcare Opportunities</div>
                <p class="kh-box-text">
                  Currently pursuing opportunities in public health policy, healthcare administration, and health systems improvement.
                  Interested in roles involving healthcare quality, compliance, and population health strategy.
                </p>
                <div style="display:grid; grid-template-columns:1fr 1fr; gap:0.6rem; margin-bottom:1.5rem;">
                  <a href="mailto:kamelliahyacinth@gmail.com" class="kh-email-btn" style="justify-content:center;">
                    <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-10 7L2 7"/></svg>
                    Send an Email
                  </a>
                  <a href="/uploads/resume.pdf" target="_blank" rel="noopener noreferrer" class="kh-email-btn" style="background:#1e3a5f; justify-content:center;">
                    <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 00-2 2v16a2 2 0 002 2h12a2 2 0 002-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="12" y1="18" x2="12" y2="12"/><polyline points="9 15 12 18 15 15"/></svg>
                    Download Resume
                  </a>
                </div>
              </div>

              <div class="kh-box-right">
                <div class="kh-links-label">Find me on</div>
                <div class="kh-links-list">

                  <a href="https://www.linkedin.com/in/kamellia/" target="_blank" rel="noopener noreferrer" class="kh-link-row">
                    <div class="kh-link-icon" style="background:rgba(10,102,194,0.1);">
                      <svg width="16" height="16" viewBox="0 0 24 24" fill="#0a66c2"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
                    </div>
                    <div class="kh-link-meta">
                      <span class="kh-link-name">LinkedIn</span>
                      <span class="kh-link-handle">linkedin.com/in/kamellia</span>
                    </div>
                    <span class="kh-link-arrow">›</span>
                  </a>

                  <a href="https://github.com/kamelliah" target="_blank" rel="noopener noreferrer" class="kh-link-row">
                    <div class="kh-link-icon" style="background:rgba(0,0,0,0.06);">
                      <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.374 0 0 5.373 0 12c0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23A11.509 11.509 0 0112 5.803c1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576C20.566 21.797 24 17.3 24 12c0-6.627-5.373-12-12-12z"/></svg>
                    </div>
                    <div class="kh-link-meta">
                      <span class="kh-link-name">GitHub</span>
                      <span class="kh-link-handle">github.com/kamelliah</span>
                    </div>
                    <span class="kh-link-arrow">›</span>
                  </a>

                  <a href="https://www.instagram.com/kamelliah/" target="_blank" rel="noopener noreferrer" class="kh-link-row">
                    <div class="kh-link-icon" style="background:rgba(217,70,239,0.08);">
                      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#d946ef" stroke-width="2"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.5" cy="6.5" r="0.5" fill="#d946ef"/></svg>
                    </div>
                    <div class="kh-link-meta">
                      <span class="kh-link-name">Instagram</span>
                      <span class="kh-link-handle">@kamelliah</span>
                    </div>
                    <span class="kh-link-arrow">›</span>
                  </a>

                </div>
              </div>
            </div>

            <div class="kh-box-footer">
              <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
              Fitchburg, Wisconsin &nbsp;&middot;&nbsp; Open to remote &amp; local opportunities
            </div>
          </div>

          <div class="kh-map-panel">
            <div id="kh-map"></div>
          </div>
          </div>
        </div>

        <script>
        document.addEventListener('DOMContentLoaded', function() {
          var lat = 43.0067, lng = -89.4670;
          var map = L.map('kh-map', {
            center: [lat, lng],
            zoom: 13,
            zoomControl: true,
            scrollWheelZoom: false
          });

          var light = L.tileLayer('https://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}{r}.png', {
            attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OSM</a> &copy; <a href="https://carto.com/attributions">CARTO</a>',
            subdomains: 'abcd', maxZoom: 19
          });
          var dark = L.tileLayer('https://{s}.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}{r}.png', {
            attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OSM</a> &copy; <a href="https://carto.com/attributions">CARTO</a>',
            subdomains: 'abcd', maxZoom: 19
          });

          function isDark() { return document.documentElement.classList.contains('dark'); }
          (isDark() ? dark : light).addTo(map);

          var pin = L.circleMarker([lat, lng], {
            radius: 10, fillColor: isDark() ? '#818cf8' : '#6366f1',
            color: '#fff', weight: 3, fillOpacity: 1
          }).addTo(map).bindPopup('<b>Fitchburg, WI 53713</b>');

          new MutationObserver(function() {
            if (isDark()) { map.removeLayer(light); dark.addTo(map); pin.setStyle({fillColor: '#818cf8'}); }
            else           { map.removeLayer(dark); light.addTo(map); pin.setStyle({fillColor: '#6366f1'}); }
          }).observe(document.documentElement, { attributes: true, attributeFilter: ['class'] });

          setTimeout(function() { map.invalidateSize(); }, 300);
        });
        </script>
        {{< /rawhtml >}}
    design:
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["5rem", "0", "5rem", "0"]
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
