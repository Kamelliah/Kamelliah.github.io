---
widget: blank
headless: true
weight: 10

title: Career Timeline
subtitle: "Healthcare Policy & Public Service Journey"

design:
  columns: "1"
  spacing:
    padding: ["60px", "0", "60px", "0"]
---

<style>
.timeline-wrapper {
    background: #f8f9fa;
    padding: 80px 40px;
    border-radius: 20px;
    overflow-x: auto;
}

.timeline-container {
    position: relative;
    max-width: 1400px;
    margin: 0 auto;
    min-height: 500px;
    padding: 100px 0;
}

/* Main horizontal line */
.timeline-line {
    position: absolute;
    top: 50%;
    left: 5%;
    right: 5%;
    height: 8px;
    background: linear-gradient(to right, #FDB702, #FF6B35, #C5050C, #9B4F96, #667eea);
    border-radius: 10px;
    transform: translateY(-50%);
    z-index: 1;
}

/* Progress line that fills based on current position */
.timeline-progress {
    position: absolute;
    top: 50%;
    left: 5%;
    height: 8px;
    background: linear-gradient(to right, #FDB702, #FF6B35);
    border-radius: 10px;
    transform: translateY(-50%);
    width: 25%;
    z-index: 2;
    transition: width 1s ease;
}

.milestones {
    position: relative;
    display: flex;
    justify-content: space-between;
    padding: 0 5%;
    z-index: 3;
}

.milestone {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
    cursor: pointer;
    transition: transform 0.3s ease;
}

.milestone:hover {
    transform: scale(1.05);
}

/* Alternating positions */
.milestone:nth-child(odd) {
    padding-bottom: 250px;
}

.milestone:nth-child(even) {
    padding-top: 250px;
}

/* Circle year badge */
.milestone-circle {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    border: 6px solid;
    background: white;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5em;
    font-weight: 700;
    box-shadow: 0 8px 25px rgba(0,0,0,0.2);
    position: relative;
    z-index: 4;
    transition: all 0.3s ease;
}

.milestone:nth-child(1) .milestone-circle {
    border-color: #FDB702;
    color: #FDB702;
}

.milestone:nth-child(2) .milestone-circle {
    border-color: #FF6B35;
    color: #FF6B35;
}

.milestone:nth-child(3) .milestone-circle {
    border-color: #C5050C;
    color: #C5050C;
}

.milestone:nth-child(4) .milestone-circle {
    border-color: #667eea;
    color: #667eea;
}

/* Active/Current milestone */
.milestone.active .milestone-circle {
    animation: pulse 2s infinite;
    box-shadow: 0 0 0 0 rgba(253, 183, 2, 0.7);
}

@keyframes pulse {
    0% {
        box-shadow: 0 0 0 0 rgba(253, 183, 2, 0.7);
    }
    70% {
        box-shadow: 0 0 0 20px rgba(253, 183, 2, 0);
    }
    100% {
        box-shadow: 0 0 0 0 rgba(253, 183, 2, 0);
    }
}

/* Connector line from circle to timeline */
.milestone-connector {
    width: 3px;
    background: currentColor;
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    z-index: 2;
}

.milestone:nth-child(odd) .milestone-connector {
    top: 120px;
    height: 130px;
}

.milestone:nth-child(even) .milestone-connector {
    bottom: 120px;
    height: 130px;
}

.milestone:nth-child(1) .milestone-connector { color: #FDB702; }
.milestone:nth-child(2) .milestone-connector { color: #FF6B35; }
.milestone:nth-child(3) .milestone-connector { color: #C5050C; }
.milestone:nth-child(4) .milestone-connector { color: #667eea; }

/* Diamond marker on timeline */
.milestone-marker {
    position: absolute;
    width: 24px;
    height: 24px;
    background: currentColor;
    transform: rotate(45deg);
    z-index: 3;
    box-shadow: 0 4px 10px rgba(0,0,0,0.2);
}

.milestone:nth-child(odd) .milestone-marker {
    bottom: -4px;
    left: 50%;
    margin-left: -12px;
}

.milestone:nth-child(even) .milestone-marker {
    top: -4px;
    left: 50%;
    margin-left: -12px;
}

/* Content box */
.milestone-content {
    text-align: center;
    max-width: 250px;
    margin-top: 20px;
}

.milestone:nth-child(even) .milestone-content {
    margin-top: 0;
    margin-bottom: 20px;
}

.milestone-title {
    font-size: 1.1em;
    font-weight: 700;
    color: #1a1a1a;
    margin-bottom: 8px;
    text-transform: uppercase;
    letter-spacing: 0.5px;
}

.milestone-description {
    font-size: 0.9em;
    color: #666;
    line-height: 1.5;
}

/* Current badge */
.current-badge {
    position: absolute;
    top: -25px;
    background: #FDB702;
    color: white;
    padding: 6px 16px;
    border-radius: 20px;
    font-size: 0.7em;
    font-weight: 700;
    text-transform: uppercase;
    box-shadow: 0 4px 12px rgba(253, 183, 2, 0.4);
    animation: bounce 2s infinite;
}

@keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
}

/* Completed milestone styling */
.milestone.completed .milestone-circle {
    background: linear-gradient(135deg, #4ade80, #22c55e);
    color: white;
    border-color: #22c55e;
}

.milestone.completed .milestone-circle::after {
    content: '✓';
    position: absolute;
    font-size: 2em;
}

@media (max-width: 1200px) {
    .timeline-container {
        min-height: 800px;
    }
    
    .milestones {
        flex-direction: column;
        align-items: flex-start;
    }
    
    .milestone {
        width: 100%;
        padding: 30px 0 !important;
        flex-direction: row;
        justify-content: flex-start;
    }
    
    .milestone-connector {
        display: none;
    }
    
    .timeline-line {
        left: 60px;
        right: auto;
        width: 8px;
        height: 90%;
        top: 5%;
        transform: none;
    }
    
    .timeline-progress {
        left: 60px;
        width: 8px !important;
        height: 30%;
        top: 5%;
        transform: none;
    }
    
    .milestone-marker {
        display: none;
    }
    
    .milestone-content {
        text-align: left;
        margin: 0 0 0 30px;
    }
}
</style>

<div class="timeline-wrapper">
    <div class="timeline-container">
        <div class="timeline-line"></div>
        <div class="timeline-progress" id="timelineProgress"></div>
        
        <div class="milestones">
            
            <!-- Milestone 1: 2025 -->
            <div class="milestone active" data-progress="25">
                <div class="milestone-connector"></div>
                <div class="milestone-circle">
                    <div class="current-badge">NOW</div>
                    2025
                </div>
                <div class="milestone-marker"></div>
                <div class="milestone-content">
                    <div class="milestone-title">Begin Interim Role</div>
                    <div class="milestone-description">
                        Launch career in public health or healthcare policy
                    </div>
                </div>
            </div>

            <!-- Milestone 2: 2025-2027 -->
            <div class="milestone" data-progress="50">
                <div class="milestone-connector"></div>
                <div class="milestone-circle">
                    2025–27
                </div>
                <div class="milestone-marker"></div>
                <div class="milestone-content">
                    <div class="milestone-title">Complete MPH Degree</div>
                    <div class="milestone-description">
                        Master of Public Health at UW-Madison
                    </div>
                </div>
            </div>

            <!-- Milestone 3: 2025-2028 -->
            <div class="milestone" data-progress="75">
                <div class="milestone-connector"></div>
                <div class="milestone-circle">
                    2025–28
                </div>
                <div class="milestone-marker"></div>
                <div class="milestone-content">
                    <div class="milestone-title">Leadership via USPHS</div>
                    <div class="milestone-description">
                        U.S. Public Health Service leadership
                    </div>
                </div>
            </div>

            <!-- Milestone 4: Long Term -->
            <div class="milestone" data-progress="100">
                <div class="milestone-connector"></div>
                <div class="milestone-circle">
                    Future
                </div>
                <div class="milestone-marker"></div>
                <div class="milestone-content">
                    <div class="milestone-title">Shape National Policy</div>
                    <div class="milestone-description">
                        Drive systemic healthcare change nationwide
                    </div>
                </div>
            </div>

        </div>
    </div>
</div>

<script>
// Make timeline interactive
document.addEventListener('DOMContentLoaded', function() {
    const milestones = document.querySelectorAll('.milestone');
    const progressBar = document.getElementById('timelineProgress');
    
    milestones.forEach(milestone => {
        milestone.addEventListener('click', function() {
            // Remove active class from all
            milestones.forEach(m => m.classList.remove('active'));
            
            // Add active to clicked
            this.classList.add('active');
            
            // Update progress bar
            const progress = this.getAttribute('data-progress');
            progressBar.style.width = progress + '%';
            
            // Update gradient based on progress
            if (progress <= 25) {
                progressBar.style.background = 'linear-gradient(to right, #FDB702, #FDB702)';
            } else if (progress <= 50) {
                progressBar.style.background = 'linear-gradient(to right, #FDB702, #FF6B35)';
            } else if (progress <= 75) {
                progressBar.style.background = 'linear-gradient(to right, #FDB702, #FF6B35, #C5050C)';
            } else {
                progressBar.style.background = 'linear-gradient(to right, #FDB702, #FF6B35, #C5050C, #9B4F96)';
            }
        });
    });
});
</script>
