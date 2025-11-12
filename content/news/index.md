<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gugobloxx News</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .header {
            text-align: center;
            color: white;
            margin-bottom: 40px;
            padding: 20px;
        }

        .header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .header p {
            font-size: 1.2em;
            opacity: 0.9;
        }

        .news-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }

        .news-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .news-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.4);
        }

        .news-image {
            width: 100%;
            height: 200px;
            object-fit: cover;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3em;
        }

        .news-content {
            padding: 25px;
        }

        .news-category {
            display: inline-block;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.85em;
            margin-bottom: 15px;
            font-weight: 600;
        }

        .news-title {
            font-size: 1.5em;
            margin-bottom: 15px;
            color: #333;
            line-height: 1.3;
        }

        .news-date {
            color: #888;
            font-size: 0.9em;
            margin-bottom: 15px;
        }

        .news-preview {
            color: #555;
            line-height: 1.6;
            margin-bottom: 15px;
        }

        .news-full {
            color: #555;
            line-height: 1.6;
            margin-bottom: 15px;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.5s ease;
        }

        .news-full.expanded {
            max-height: 1000px;
        }

        .read-more-btn {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border: none;
            padding: 12px 30px;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1em;
            font-weight: 600;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            display: inline-block;
        }

        .read-more-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .read-more-btn:active {
            transform: scale(0.98);
        }

        @media (max-width: 768px) {
            .news-grid {
                grid-template-columns: 1fr;
            }

            .header h1 {
                font-size: 2em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>📰 Gugobloxx News</h1>
            <p>Stay updated with the latest stories</p>
        </div>

        <div class="news-grid">
            <!-- News Card 1 -->
            <div class="news-card">
                <div class="news-image">🚀</div>
                <div class="news-content">
                    <span class="news-category">Technology</span>
                    <h2 class="news-title">Revolutionary AI Breakthrough Announced</h2>
                    <p class="news-date">November 11, 2025</p>
                    <p class="news-preview">
                        Scientists at Gugobloxx Labs have unveiled a groundbreaking artificial intelligence system that promises to revolutionize the tech industry...
                    </p>
                    <div class="news-full">
                        <p>
                            The new AI system, dubbed "NexGen-AI," demonstrates unprecedented capabilities in natural language processing and problem-solving. According to lead researcher Dr. Sarah Chen, "This technology represents a quantum leap forward in machine learning."
                        </p>
                        <p>
                            The system has already been tested in various real-world applications, showing remarkable results in healthcare diagnostics, climate modeling, and educational assistance. Industry experts believe this could be the most significant AI advancement in decades.
                        </p>
                        <p>
                            Gugobloxx Labs plans to make the technology available for beta testing next quarter, with a full commercial release expected by mid-2026.
                        </p>
                    </div>
                    <button class="read-more-btn" onclick="toggleReadMore(this)">Read More</button>
                </div>
            </div>

            <!-- News Card 2 -->
            <div class="news-card">
                <div class="news-image">🌍</div>
                <div class="news-content">
                    <span class="news-category">Environment</span>
                    <h2 class="news-title">Global Climate Summit Reaches Historic Agreement</h2>
                    <p class="news-date">November 10, 2025</p>
                    <p class="news-preview">
                        World leaders have signed a comprehensive climate accord that sets ambitious targets for carbon reduction over the next decade...
                    </p>
                    <div class="news-full">
                        <p>
                            The agreement, signed by 195 countries, includes binding commitments to reduce greenhouse gas emissions by 50% by 2035. This represents the most aggressive climate action plan in history.
                        </p>
                        <p>
                            Key provisions include massive investments in renewable energy infrastructure, protection of critical ecosystems, and financial support for developing nations transitioning to green economies.
                        </p>
                        <p>
                            Environmental groups have praised the accord as a "turning point" in the fight against climate change, though some critics argue the targets don't go far enough.
                        </p>
                    </div>
                    <button class="read-more-btn" onclick="toggleReadMore(this)">Read More</button>
                </div>
            </div>

            <!-- News Card 3 -->
            <div class="news-card">
                <div class="news-image">🏆</div>
                <div class="news-content">
                    <span class="news-category">Sports</span>
                    <h2 class="news-title">Underdog Team Wins Championship in Stunning Upset</h2>
                    <p class="news-date">November 9, 2025</p>
                    <p class="news-preview">
                        In one of the greatest upsets in sports history, the Gugobloxx Titans defeated the heavily favored champions in a thrilling final match...
                    </p>
                    <div class="news-full">
                        <p>
                            The Titans, who entered the playoffs as the eighth seed, completed their Cinderella run with a dramatic 98-95 victory. Star player Marcus Johnson scored 42 points, including the game-winning three-pointer with just 2.3 seconds remaining.
                        </p>
                        <p>
                            "This is what dreams are made of," said coach Jennifer Martinez after the game. "Our team never stopped believing, and tonight we made history."
                        </p>
                        <p>
                            The victory marks the franchise's first championship in 30 years and has sent fans into a frenzy of celebration across the city.
                        </p>
                    </div>
                    <button class="read-more-btn" onclick="toggleReadMore(this)">Read More</button>
                </div>
            </div>

            <!-- News Card 4 -->
            <div class="news-card">
                <div class="news-image">💼</div>
                <div class="news-content">
                    <span class="news-category">Business</span>
                    <h2 class="news-title">Tech Giant Announces Major Acquisition</h2>
                    <p class="news-date">November 8, 2025</p>
                    <p class="news-preview">
                        Gugobloxx Corporation has acquired innovative startup CloudSync in a deal valued at $5.2 billion, marking the company's largest acquisition to date...
                    </p>
                    <div class="news-full">
                        <p>
                            The acquisition brings CloudSync's cutting-edge cloud computing platform and 2,000+ employees into the Gugobloxx ecosystem. CEO Michael Torres stated, "This strategic move positions us at the forefront of cloud innovation."
                        </p>
                        <p>
                            CloudSync's proprietary technology enables seamless data synchronization across multiple platforms with military-grade security. The startup had been valued at over $3 billion before acquisition talks began.
                        </p>
                        <p>
                            Analysts predict the deal will significantly boost Gugobloxx's enterprise offerings and create new revenue streams in the cloud services sector.
                        </p>
                    </div>
                    <button class="read-more-btn" onclick="toggleReadMore(this)">Read More</button>
                </div>
            </div>

            <!-- News Card 5 -->
            <div class="news-card">
                <div class="news-image">🎬</div>
                <div class="news-content">
                    <span class="news-category">Entertainment</span>
                    <h2 class="news-title">Blockbuster Film Breaks Opening Weekend Records</h2>
                    <p class="news-date">November 7, 2025</p>
                    <p class="news-preview">
                        "Galaxy Warriors: The Final Chapter" has shattered box office records with a stunning $312 million opening weekend worldwide...
                    </p>
                    <div class="news-full">
                        <p>
                            The highly anticipated conclusion to the beloved sci-fi franchise exceeded all expectations, becoming the biggest opening weekend in cinema history. Fans lined up for hours to catch the first screenings.
                        </p>
                        <p>
                            Director Ava Rodriguez delivered an epic finale that critics are calling "a masterpiece of storytelling and visual effects." The film currently holds a 96% rating on review aggregator sites.
                        </p>
                        <p>
                            Industry insiders predict the film could surpass $2 billion globally, potentially becoming one of the highest-grossing films of all time.
                        </p>
                    </div>
                    <button class="read-more-btn" onclick="toggleReadMore(this)">Read More</button>
                </div>
            </div>

            <!-- News Card 6 -->
            <div class="news-card">
                <div class="news-image">🔬</div>
                <div class="news-content">
                    <span class="news-category">Science</span>
                    <h2 class="news-title">Medical Breakthrough Offers Hope for Rare Disease</h2>
                    <p class="news-date">November 6, 2025</p>
                    <p class="news-preview">
                        Researchers at Gugobloxx Medical Institute have developed a promising new treatment for a rare genetic disorder that affects thousands worldwide...
                    </p>
                    <div class="news-full">
                        <p>
                            The gene therapy treatment showed remarkable success in clinical trials, with 87% of participants experiencing significant improvement. The breakthrough could offer new hope to families affected by this devastating condition.
                        </p>
                        <p>
                            Dr. James Peterson, lead researcher, explained: "We've essentially developed a way to correct the genetic mutation at its source. This represents a paradigm shift in how we approach genetic diseases."
                        </p>
                        <p>
                            The treatment is expected to undergo final FDA review within the next six months, with approval anticipated for early 2026.
                        </p>
                    </div>
                    <button class="read-more-btn" onclick="toggleReadMore(this)">Read More</button>
                </div>
            </div>
        </div>
    </div>

    <script>
        function toggleReadMore(button) {
            const newsCard = button.closest('.news-card');
            const fullContent = newsCard.querySelector('.news-full');
            const preview = newsCard.querySelector('.news-preview');
            
            if (fullContent.classList.contains('expanded')) {
                // Collapse
                fullContent.classList.remove('expanded');
                preview.style.display = 'block';
                button.textContent = 'Read More';
                
                // Smooth scroll back to card top
                newsCard.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
            } else {
                // Expand
                fullContent.classList.add('expanded');
                preview.style.display = 'none';
                button.textContent = 'Read Less';
            }
        }
    </script>
</body>
</html>
