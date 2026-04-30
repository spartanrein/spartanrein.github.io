<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ops Page - Hyrox Shanghai</title>
    <style>
        /* Base Reset & Variables */
        :root {
            --bg-color: #000000;
            --text-color: #ffffff;
            --accent-color: #fceb00; /* Hyrox Yellow */
            --border-color: #333333;
            --font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            font-family: var(--font-family);
            line-height: 1.6;
            -webkit-font-smoothing: antialiased;
        }

        /* Layout */
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* Header */
        header {
            margin-bottom: 50px;
            border-bottom: 2px solid var(--accent-color);
            padding-bottom: 20px;
        }

        h1 {
            font-size: 28px;
            font-weight: 800;
            letter-spacing: 1px;
            margin-bottom: 10px;
            text-transform: uppercase;
        }

        .subtitle {
            font-size: 14px;
            color: #888;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        h2 {
            font-size: 20px;
            font-weight: 600;
            margin: 40px 0 20px;
            color: var(--accent-color);
            text-transform: uppercase;
        }

        /* SVG Icons */
        .icon {
            display: inline-block;
            width: 18px;
            height: 18px;
            margin-right: 12px;
            vertical-align: middle;
            fill: none;
            stroke: currentColor;
            stroke-width: 2;
            stroke-linecap: round;
            stroke-linejoin: round;
        }

        .chevron {
            width: 16px;
            height: 16px;
            transition: transform 0.3s ease;
            stroke: #666;
        }

        /* Accordion Styles */
        .accordion {
            border-top: 1px solid var(--border-color);
        }

        .accordion-item {
            border-bottom: 1px solid var(--border-color);
        }

        .accordion-header {
            width: 100%;
            background: none;
            border: none;
            color: var(--text-color);
            text-align: left;
            padding: 24px 0;
            font-size: 16px;
            font-weight: 600;
            font-family: inherit;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .accordion-header:hover {
            color: var(--accent-color);
        }

        .accordion-header .title-wrapper {
            display: flex;
            align-items: center;
        }

        /* Active State logic */
        .accordion-item.active .accordion-header {
            color: var(--accent-color);
        }

        .accordion-item.active .chevron {
            transform: rotate(180deg);
            stroke: var(--accent-color);
        }

        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-in-out, padding 0.3s ease;
            color: #e0e0e0;
            font-size: 15px;
        }

        .accordion-item.active .accordion-content {
            max-height: 800px; 
            padding-bottom: 30px;
        }

        /* Content Specific Styles */
        .content-block {
            margin-bottom: 15px;
        }

        .label {
            color: #888;
            font-size: 12px;
            text-transform: uppercase;
            display: block;
            margin-bottom: 4px;
        }

        .accent-text {
            color: var(--accent-color);
            text-decoration: none;
            font-weight: 600;
            border-bottom: 1px solid transparent;
            transition: border-color 0.2s;
        }

        .accent-text:hover {
            border-bottom-color: var(--accent-color);
        }

        .phone-link {
            color: var(--text-color);
            text-decoration: none;
            font-size: 16px;
        }

        /* Responsive */
        @media (min-width: 768px) {
            h1 { font-size: 36px; }
            .accordion-header { font-size: 18px; }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>OPS PAGE – HYROX SHANGHAI</h1>
            <p class="subtitle">16–17 MAY 2026 | INTERNAL USE ONLY</p>
        </header>

        <h2>Event Logistics</h2>

        <div class="accordion">
            
            <div class="accordion-item">
                <button class="accordion-header" aria-expanded="false">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24">
                            <path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path>
                            <circle cx="12" cy="10" r="3"></circle>
                        </svg>
                        Hotel Accommodation
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <div class="content-block">
                        <span class="label">Hotel Name</span>
                        <p>上海世博萨和酒店</p>
                        <p style="color: #888;">SAVHE Hotel Shanghai World Expo</p>
                    </div>

                    <div class="content-block">
                        <span class="label">Address</span>
                        <p>上海市浦东新区雪野路 410 号</p>
                        <p style="color: #888;">No. 410 Xueye Road, Pudong New Area, Shanghai</p>
                    </div>

                    <div class="content-block" style="margin-top: 20px; border-top: 1px solid #222; padding-top: 15px;">
                        <span class="label">Contact Numbers</span>
                        <p>Tel: <a href="tel:+862168818869" class="phone-link">+86 21 6881 8869</a></p>
                        <p>Service: <a href="tel:+8619370733609" class="phone-link">+86 193 7073 3609</a></p>
                    </div>

                    <div style="margin-top: 20px;">
                        <a href="https://maps.google.com/?q=SAVHE+Hotel+Shanghai+World+Expo" target="_blank" class="accent-text">
                            OPEN IN MAPS →
                        </a>
                    </div>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header" aria-expanded="false">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24">
                            <path d="M3 21h18"></path>
                            <path d="M3 7v1a3 3 0 0 0 6 0V7m0 1a3 3 0 0 0 6 0V7m0 1a3 3 0 0 0 6 0V7H3l2-4h14l2 4"></path>
                            <path d="M5 21V10.85"></path>
                            <path d="M19 21V10.85"></path>
                            <path d="M9 21v-4a2 2 0 0 1 4 0v4"></path>
                        </svg>
                        Event Venue
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <div class="content-block">
                        <span class="label">Venue Name</span>
                        <p>上海世博展览馆</p>
                        <p style="color: #888;">SHANGHAI WORLD EXPO EXHIBITION & CONVENTION CENTER</p>
                    </div>

                    <div class="content-block">
                        <span class="label">Address</span>
                        <p>上海市浦东新区国展路1099号</p>
                        <p style="color: #888;">1099 Guo Zhan Road, Pudong New Area, Shanghai</p>
                    </div>

                    <div style="margin-top: 20px;">
                        <a href="https://maps.google.com/?q=Shanghai+World+Expo+Exhibition+and+Convention+Center" target="_blank" class="accent-text">
                            OPEN IN MAPS →
                        </a>
                    </div>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header" aria-expanded="false">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24">
                            <path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"></path>
                        </svg>
                        Start Wave
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <p>The link to the start wave is <a href="https://docs.google.com/spreadsheets/d/1XYsb3mp7i4cLr715llGVElfHz_wbbpjpSXmVr6P8lNA/edit?gid=1391778420#gid=1391778420" target="_blank" class="accent-text">HERE</a>.</p>
                </div>
            </div>

        </div>
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const accordionHeaders = document.querySelectorAll('.accordion-header');

            accordionHeaders.forEach(header => {
                header.addEventListener('click', () => {
                    const currentItem = header.parentElement;
                    const isActive = currentItem.classList.contains('active');

                    // Close all accordion items
                    document.querySelectorAll('.accordion-item').forEach(item => {
                        item.classList.remove('active');
                        item.querySelector('.accordion-header').setAttribute('aria-expanded', 'false');
                    });

                    // If the clicked item wasn't active, open it
                    if (!isActive) {
                        currentItem.classList.add('active');
                        header.setAttribute('aria-expanded', 'true');
                    }
                });
            });
        });
    </script>
</body>
</html>
