<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ops Page - Hong Kong</title>
    <style>
        /* Base Reset & Variables */
        :root {
            --bg-color: #000000;
            --text-color: #ffffff;
            --accent-color: #fceb00;
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
            line-height: 1.5;
            -webkit-font-smoothing: antialiased;
        }

        /* Layout */
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        /* Typography */
        h1 {
            font-size: 28px;
            font-weight: 500;
            letter-spacing: 0.5px;
            margin-bottom: 20px;
        }

        .subtitle {
            font-size: 15px;
            color: #e0e0e0;
            margin-bottom: 50px;
        }

        h2 {
            font-size: 22px;
            font-weight: 600;
            margin-bottom: 30px;
        }

        /* SVG Icons */
        .icon {
            display: inline-block;
            width: 16px;
            height: 16px;
            margin-right: 8px;
            vertical-align: middle;
            fill: none;
            stroke: currentColor;
            stroke-width: 2;
            stroke-linecap: round;
            stroke-linejoin: round;
        }

        .chevron {
            width: 14px;
            height: 14px;
            transition: transform 0.3s ease;
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
            padding: 20px 0;
            font-size: 15px;
            font-weight: 500;
            font-family: inherit;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: color 0.2s ease;
        }

        .accordion-header:hover {
            color: #cccccc;
        }

        .accordion-header .title-wrapper {
            display: flex;
            align-items: center;
        }

        /* Active State */
        .accordion-item.active .accordion-header {
            color: var(--accent-color);
        }

        .accordion-item.active .chevron {
            transform: rotate(180deg);
        }

        /* Accordion Content */
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out, padding 0.3s ease;
            background-color: var(--bg-color);
            color: var(--text-color);
            font-size: 15px;
        }

        .accordion-item.active .accordion-content {
            padding-bottom: 20px;
            max-height: 200px; /* Arbitrary high value to allow expansion */
        }

        .accent-text {
            color: var(--accent-color);
        }

        /* Responsive */
        @media (min-width: 768px) {
            h1 { font-size: 36px; }
            h2 { font-size: 24px; }
            .subtitle { font-size: 16px; }
            .accordion-header { font-size: 16px; }
            .accordion-content { font-size: 16px; }
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>OPS PAGE – HONG KONG (8-10 MAY 2026)</h1>
        <p class="subtitle">Welcome to the Event Ops Page – this is intended for internal use only and is commercial in confidence.</p>

        <h2>Event Overview</h2>

        <div class="accordion">
            
            <div class="accordion-item active">
                <button class="accordion-header" aria-expanded="true">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24">
                            <path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path>
                            <path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path>
                        </svg>
                        to Race Week Syntax
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <p>The <svg class="icon" viewBox="0 0 24 24" style="margin: 0 4px; width: 14px; height:14px;"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg> to the Race Week Syntax is <span class="accent-text">HERE</span></p>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header" aria-expanded="false">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24">
                            <path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path>
                            <path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path>
                        </svg>
                        to Wave Start Spreadsheet
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <p>Link to the Wave Start Spreadsheet is located here.</p>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header" aria-expanded="false">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24">
                            <path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path>
                            <path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path>
                        </svg>
                        to Staff Accommodation Spreadsheet
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <p>Details regarding staff accommodation can be found here.</p>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header" aria-expanded="false">
                    <div class="title-wrapper">
                        Start Wave Schedule & Ceremony Times
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <p>Schedule details goes here.</p>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header" aria-expanded="false">
                    <div class="title-wrapper">
                        Staff Shifts
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <p>Staff shift information goes here.</p>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header" aria-expanded="false">
                    <div class="title-wrapper">
                        Important Event Updates
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                <div class="accordion-content">
                    <p>Any important updates will be posted here.</p>
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
