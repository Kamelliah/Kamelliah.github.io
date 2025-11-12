---
widget: blank
headless: true
weight: 10

title: Latest News
subtitle: ""

design:
  columns: "1"
  spacing:
    padding: ["40px", "0", "40px", "0"]
---

<style>
.news-list {
    max-width: 900px;
    margin: 0 auto;
}

.news-item {
    border-bottom: 1px solid #e0e0e0;
    padding-bottom: 40px;
    margin-bottom: 50px;
}

.news-item:last-child {
    border-bottom: none;
}

.news-date {
    color: #666;
    font-size: 0.9em;
    margin-bottom: 10px;
}

.news-title {
    font-size: 1.8em;
    font-weight: 600;
    color: #000;
    margin-bottom: 20px;
    line-height: 1.3;
}

.news-content-wrapper {
    display: flex;
    gap: 30px;
    align-items: flex-start;
}

.news-text {
    flex: 1;
}

.news-preview {
    color: #333;
    line-height: 1.7;
    font-size: 1.05em;
    margin-bottom: 15px;
}

.news-full {
    color: #333;
    line-height: 1.7;
    font-size: 1.05em;
    display: none;
    margin-bottom: 15px;
}

.news-full.visible {
    display: block;
}

.news-full p {
    margin-bottom: 15px;
}

.news-image {
    width: 250px;
    height: 180px;
    flex-shrink: 0;
    border-radius: 4px;
    overflow: hidden;
}

.news-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.read-more-btn {
    background: transparent;
    color: #c5050c;
    border: 2px solid #c5050c;
    padding: 10px 25px;
    border-radius: 4px;
    cursor: pointer;
    font-size: 0.95em;
    font-weight: 600;
    transition: all 0.2s ease;
    margin-top: 10px;
}

.read-more-btn:hover {
    background: #c5050c;
    color: white;
}

@media (max-width: 768px) {
    .news-content-wrapper {
        flex-direction: column-reverse;
    }

    .news-image {
        width: 100%;
        height: 200px;
    }

    .news-title {
        font-size: 1.4em;
    }
}
</style>

<div class="news-list">

<!-- News Item 1 -->
<div class="news-item">
    <div class="news-date">May 17, 2025</div>
    <h2 class="news-title">Turning the Tassel: Preparing for Graduation at UW-La Crosse</h2>
    <div class="news-content-wrapper">
        <div class="news-text">
            <p class="news-preview">Set to graduate with my Master's in Healthcare Administration, this milestone represents the culmination of years of hard work, leadership growth, and a deepening commitment to improving healthcare systems and advancing equity.</p>
            <div class="news-full">
                <p>This journey has been transformative, challenging me to think critically about healthcare policy, organizational leadership, and the social determinants that shape health outcomes. Through rigorous coursework, practical experiences, and collaboration with incredible peers and faculty, I've developed the skills and perspective needed to make meaningful contributions to the healthcare field.</p>
                <p>The graduate hooding ceremony at UW-La Crosse will mark not just an academic achievement, but a commitment to using this education to drive positive change. From improving access to care to championing health equity initiatives, I'm excited to apply what I've learned to real-world challenges.</p>
                <p>I'm grateful to my family, mentors, and classmates who supported me throughout this journey. As I turn the tassel, I look forward to the opportunities ahead and the impact I hope to make in healthcare administration.</p>
            </div>
            <button class="read-more-btn" onclick="toggleReadMore(this)">READ MORE</button>
        </div>
        <div class="news-image" style="background: #c5050c; display: flex; align-items: center; justify-content: center;">
            <span style="color: white; font-size: 4em;">🎓</span>
        </div>
    </div>
</div>

<!-- News Item 2 -->
<div class="news-item">
    <div class="news-date">Apr 6, 2025</div>
    <h2 class="news-title">From Student to Standard</h2>
    <div class="news-content-wrapper">
        <div class="news-text">
            <p class="news-preview">My capstone work was selected by Dr. Jodi Olmstead to serve as a model portfolio for students in HCA 789 and 790 capstone courses delivered across multiple UW campuses within the Healthcare Administration program. I'm honored to have my work featured as part of this system-wide teaching framework.</p>
            <div class="news-full">
                <p>The capstone project represented the culmination of my Master's program, integrating theoretical knowledge with practical application in addressing a real healthcare challenge. The project focused on developing strategic solutions for improving healthcare delivery while considering financial sustainability, regulatory compliance, and patient outcomes.</p>
                <p>Dr. Olmstead's decision to use my work as an exemplar reflects the quality and depth of analysis that went into the project. It demonstrates the application of healthcare administration principles including data analysis, stakeholder engagement, and evidence-based decision making.</p>
                <p>Having this work serve as a teaching tool for future healthcare administrators is incredibly rewarding. It represents not just personal achievement, but a contribution to the education of the next generation of healthcare leaders across the UW system.</p>
            </div>
            <button class="read-more-btn" onclick="toggleReadMore(this)">READ MORE</button>
        </div>
        <div class="news-image" style="background: linear-gradient(135deg, #0066cc 0%, #0099ff 100%); display: flex; align-items: center; justify-content: center;">
            <span style="color: white; font-size: 4em;">🏥</span>
        </div>
    </div>
</div>

<!-- News Item 3 -->
<div class="news-item">
    <div class="news-date">Mar 8, 2025</div>
    <h2 class="news-title">A New Chapter Begins: Accepted into the UWMPH Program</h2>
    <div class="news-content-wrapper">
        <div class="news-text">
            <p class="news-preview">Enrollment has been confirmed for the Master of Public Health program at UW–Madison, opening a new chapter focused on public health leadership, interdisciplinary collaboration, and advancing community health outcomes.</p>
            <div class="news-full">
                <p>The UW-Madison School of Medicine and Public Health is renowned for its commitment to addressing public health challenges through innovative research, community partnerships, and leadership development. This program will provide advanced training in epidemiology, health policy, program evaluation, and population health management.</p>
                <p>Public health represents a natural progression from healthcare administration, allowing me to expand my impact from organizational leadership to community and population-level interventions. The interdisciplinary nature of the program will facilitate collaboration across sectors to address the complex factors that influence health outcomes.</p>
                <p>I'm particularly excited about opportunities to engage in community-based research, policy analysis, and health equity initiatives. The skills and knowledge gained through this program will complement my healthcare administration background and enable me to drive systemic change in public health.</p>
                <p>Looking ahead, I'm eager to contribute to Wisconsin's public health landscape and work toward creating healthier, more equitable communities throughout the state and beyond.</p>
            </div>
            <button class="read-more-btn" onclick="toggleReadMore(this)">READ MORE</button>
        </div>
        <div class="news-image" style="background: #c5050c; display: flex; align-items: center; justify-content: center;">
            <span style="color: white; font-size: 4em;">📚</span>
        </div>
    </div>
</div>

<!-- News Item 4 -->
<div class="news-item">
    <div class="news-date">Feb 15, 2025</div>
    <h2 class="news-title">Research Published in Healthcare Journal</h2>
    <div class="news-content-wrapper">
        <div class="news-text">
            <p class="news-preview">My research examining the impact of telehealth implementation on rural healthcare access has been published in the Journal of Healthcare Management, contributing to the growing body of evidence on digital health solutions.</p>
            <div class="news-full">
                <p>The study analyzed telehealth adoption patterns across rural healthcare facilities in Wisconsin, examining barriers to implementation, patient outcomes, and cost-effectiveness. Key findings showed that strategic telehealth programs can significantly improve access to specialty care while reducing transportation burdens for rural patients.</p>
                <p>The research utilized mixed-methods analysis, combining quantitative data on utilization rates and health outcomes with qualitative interviews from patients and providers. This comprehensive approach provided insights into both the measurable impacts and the lived experiences of telehealth adoption.</p>
                <p>Publication in this peer-reviewed journal represents validation of the research methodology and findings, and contributes to evidence-based policy discussions around rural healthcare access. The implications extend beyond Wisconsin to other rural regions facing similar healthcare delivery challenges.</p>
            </div>
            <button class="read-more-btn" onclick="toggleReadMore(this)">READ MORE</button>
        </div>
        <div class="news-image" style="background: linear-gradient(135deg, #228B22 0%, #32CD32 100%); display: flex; align-items: center; justify-content: center;">
            <span style="color: white; font-size: 4em;">📊</span>
        </div>
    </div>
</div>

<!-- News Item 5 -->
<div class="news-item">
    <div class="news-date">Jan 20, 2025</div>
    <h2 class="news-title">Leading Healthcare Equity Initiative</h2>
    <div class="news-content-wrapper">
        <div class="news-text">
            <p class="news-preview">Selected to lead a new healthcare equity initiative focused on reducing disparities in maternal and child health outcomes across underserved communities in Wisconsin.</p>
            <div class="news-full">
                <p>The initiative brings together healthcare providers, community organizations, and public health agencies to address the root causes of maternal and child health disparities. This includes improving access to prenatal care, enhancing health literacy, and addressing social determinants like housing stability and food security.</p>
                <p>Wisconsin faces significant racial and geographic disparities in maternal mortality and infant health outcomes. This project takes a comprehensive approach, combining clinical interventions with community-based support systems and policy advocacy to create sustainable improvements.</p>
                <p>As project lead, I'm coordinating a multidisciplinary team and working to secure funding from state and federal sources. Early partnerships have been established with community health centers, birthing hospitals, and grassroots organizations serving high-risk populations.</p>
                <p>The work is challenging but essential. Every family deserves access to safe, high-quality maternal and child healthcare regardless of their zip code or demographic background.</p>
            </div>
            <button class="read-more-btn" onclick="toggleReadMore(this)">READ MORE</button>
        </div>
        <div class="news-image" style="background: linear-gradient(135deg, #9B59B6 0%, #8E44AD 100%); display: flex; align-items: center; justify-content: center;">
            <span style="color: white; font-size: 4em;">❤️</span>
        </div>
    </div>
</div>

</div>

<script>
function toggleReadMore(button) {
    const newsItem = button.closest('.news-item');
    const fullContent = newsItem.querySelector('.news-full');
    const preview = newsItem.querySelector('.news-preview');
    
    if (fullContent.classList.contains('visible')) {
        fullContent.classList.remove('visible');
        preview.style.display = 'block';
        button.textContent = 'READ MORE';
        newsItem.scrollIntoView({ behavior: 'smooth', block: 'start' });
    } else {
        fullContent.classList.add('visible');
        preview.style.display = 'none';
        button.textContent = 'READ LESS';
    }
}
</script>
```

---

## File Structure:
```
content/
└── news/
    ├── index.md           ← Create this first
    └── news-content.md    ← Then create this with all the HTML above
