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
            --content-font-size: 15px;
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

        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 20px 15px; /* Reduced for mobile */
        }

        header {
            margin-bottom: 30px;
            border-bottom: 2px solid var(--accent-color);
            padding-bottom: 15px;
        }

        h1 {
            font-size: 22px; /* Scaled down for mobile */
            font-weight: 800;
            letter-spacing: 1px;
            margin-bottom: 8px;
            text-transform: uppercase;
            line-height: 1.2;
        }

        .subtitle {
            font-size: 12px;
            color: #888;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        h2 {
            font-size: 18px;
            font-weight: 600;
            margin: 30px 0 15px;
            color: var(--accent-color);
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .icon {
            display: inline-block;
            width: 18px;
            height: 18px;
            margin-right: 10px;
            vertical-align: middle;
            fill: none;
            stroke: currentColor;
            stroke-width: 2;
            stroke-linecap: round;
            stroke-linejoin: round;
            flex-shrink: 0; /* Prevents icon squashing */
        }

        .chevron {
            width: 16px;
            height: 16px;
            transition: transform 0.3s ease;
            stroke: #666;
        }

        .accordion {
            border-top: 1px solid var(--border-color);
            margin-bottom: 20px;
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
            padding: 18px 0; /* Tighter for mobile */
            font-size: 16px;
            font-weight: 600;
            font-family: inherit;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .accordion-header:hover { color: var(--accent-color); }
        .accordion-item.active .accordion-header { color: var(--accent-color); }
        .accordion-item.active .chevron { transform: rotate(180deg); stroke: var(--accent-color); }

        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
            color: #e0e0e0;
            font-size: var(--content-font-size);
        }

        .accordion-item.active .accordion-content {
            max-height: 2000px; /* High enough to accommodate content */
            padding-bottom: 20px;
        }

        .content-block { margin-bottom: 15px; }

        .label {
            color: #888;
            font-size: 11px;
            text-transform: uppercase;
            display: block;
            margin-bottom: 2px;
            letter-spacing: 0.5px;
        }

        .accent-text {
            color: var(--accent-color);
            text-decoration: none;
            font-weight: 600;
            transition: color 0.2s ease;
            word-break: break-word;
        }

        .accent-text:hover { color: #ffffff; }

        /* Tech Table Mobile Fixes */
        .table-scroll-container {
            width: 100%;
            overflow-x: auto; /* Allows horizontal scroll on tiny screens */
            -webkit-overflow-scrolling: touch;
            margin-top: 15px;
        }

        .tech-table {
            width: 100%;
            min-width: 300px; /* Prevents columns from becoming too thin */
            border-collapse: collapse;
            background-color: #000000;
            border: none;
        }

        .tech-table th {
            text-align: left;
            padding: 12px 10px;
            background-color: #111111;
            color: var(--accent-color);
            font-size: 11px;
            text-transform: uppercase;
            letter-spacing: 1px;
            border-bottom: 1px solid var(--border-color);
        }

        .tech-table td {
            padding: 10px 10px;
            color: #ffffff;
            font-family: "Courier New", Courier, monospace;
            font-size: 13px; /* Slightly smaller for table data */
            word-break: break-all; /* Prevents long RDP strings from breaking layout */
            vertical-align: top;
        }

        .tech-table th:nth-child(2), .tech-table td:nth-child(2) {
            text-align: center;
        }

        .config-title {
            color: var(--accent-color);
            font-weight: 800;
            margin: 20px 0 10px 0;
            font-size: 16px;
            display: flex;
            align-items: center;
        }

        .config-title::before {
            content: "";
            display: inline-block;
            width: 4px;
            height: 16px;
            background: var(--accent-color);
            margin-right: 10px;
        }

        /* Responsive Breakpoints */
        @media (min-width: 768px) {
            .container { padding: 40px 20px; }
            h1 { font-size: 36px; }
            h2 { font-size: 20px; }
            .accordion-header { padding: 24px 0; font-size: 18px; }
            .tech-table th, .tech-table td { font-size: 14px; padding: 12px; }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>OPS PAGE – HYROX SHANGHAI</h1>
            <p class="subtitle">16–17 MAY 2026 | INTERNAL USE ONLY</p>
        </header>

        <h2>Venue and Accommodation</h2>
        <div class="accordion">
            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
                        Hotel Accommodation
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
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
                    <div class="content-block" style="border-top: 1px solid #222; padding-top: 10px;">
                        <span class="label">Contact</span>
                        <p>Tel: <a href="tel:+862168818869" style="color:white; text-decoration:none;">+86 21 6881 8869</a></p>
                    </div>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M3 21h18"></path><path d="M3 7v1a3 3 0 0 0 6 0V7m0 1a3 3 0 0 0 6 0V7m0 1a3 3 0 0 0 6 0V7H3l2-4h14l2 4"></path><path d="M5 21V10.85"></path><path d="M19 21V10.85"></path><path d="M9 21v-4a2 2 0 0 1 4 0v4"></path></svg>
                        Event Venue
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
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
                    </div>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"></path><polyline points="9 22 9 12 15 12 15 22"></polyline></svg>
                        Floor Plan
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <p>The Floor Plan can be found <a href="https://drive.google.com/file/d/1pqxaQhYyO0VfSDxzC1daZDAVlMFkqmO0/view?usp=sharing" target="_blank" class="accent-text">HERE</a>.</p>
                </div>
            </div>
        </div>

        <h2>Event Information</h2>
        <div class="accordion">
            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"></path></svg>
                        Start Wave
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <p>The link to the start wave is <a href="https://docs.google.com/spreadsheets/d/1XYsb3mp7i4cLr715llGVElfHz_wbbpjpSXmVr6P8lNA/edit?gid=1391778420#gid=1391778420" target="_blank" class="accent-text">HERE</a>.</p>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M5 3v4M19 3v4M5 21v-4M19 21v-4M2 12h3m14 0h3M7 12c0-2.8 2.2-5 5-5s5 2.2 5 5-2.2 5-5 5-5-2.2-5-5z"></path><path d="M9 12c0-1.7 1.3-3 3-3s3 1.3 3 3-1.3 3-3 3-3-1.3-3-3z"></path></svg>
                        Loop Channel Assignment
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <p>Loop Channel Assignment is <a href="https://docs.google.com/spreadsheets/d/1Z4xVx2gqcWqaX_h2xDgRBTwDiTzK9ypVRiJNqTCVAbs/edit?gid=324513968#gid=324513968" target="_blank" class="accent-text">HERE</a>.</p>
                </div>
            </div>
        </div>

        <h2>Logistics</h2>
        <div class="accordion">
            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg>
                        Inventory
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <p>The Inventory sheet is <a href="https://docs.google.com/spreadsheets/d/1JMlkQguUmbiTYXNGrfLpVmxekoj6HC1PzkG6qDUAYCE/edit?gid=1810257584#gid=1810257584" target="_blank" class="accent-text">HERE</a>.</p>
                </div>
            </div>
        </div>

        <h2>Tech</h2>
        <div class="accordion">
            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><rect x="2" y="3" width="20" height="14" rx="2" ry="2"></rect><line x1="8" y1="21" x2="16" y2="21"></line><line x1="12" y1="17" x2="12" y2="21"></line></svg>
                        Webresults & RDP
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <p>Webresults sheet is <a href="https://docs.google.com/spreadsheets/d/1FWcLjGaQb46gH75hjLZFEiSf4DSFWtBRrUxOduGFez4/edit?gid=682272386#gid=682272386" target="_blank" class="accent-text">HERE</a></p>
                    <div class="config-title">Config: 2</div>
                    <div class="table-scroll-container">
                        <table class="tech-table">
                            <thead>
                                <tr>
                                    <th>RDP / Address</th>
                                    <th>Assignment</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr><td>.21/rdp4hyrox13</td><td>TFCC DB</td></tr>
                                <tr><td>.21/rdp4hyrox14</td><td>PVG Ben</td></tr>
                                <tr><td>.21/rdp4hyrox15</td><td>PVG Rein</td></tr>
                                <tr><td>.21/rdp4hyrox16</td><td>PVG Mitch</td></tr>
                                <tr><td>.21/rdp4hyrox17</td><td>PVG Darko</td></tr>
                                <tr><td>.21/rdp4hyrox18</td><td>PVG Burq</td></tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><rect x="2" y="3" width="20" height="15" rx="2"/><path d="M17 21l-5-4-5 4"/></svg>
                        Screen Links
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <div class="config-title">Config 2</div>
                    <p style="margin-bottom: 5px;">Lap: <a href="https://hyrox-screens.r.mikatiming.com/?pid=tfd_screen_config_2&lang=EN_CAP" target="_blank" class="accent-text">Link</a></p>
                    <p style="margin-bottom: 5px;">Finish: <a href="https://hyrox-screens.r.mikatiming.com/?pid=tfd_screen_finish_nat_config_2&lang=EN_CAP" target="_blank" class="accent-text">Link</a></p>
                    <p style="margin-bottom: 5px;">Recovery 1: <a href="https://hyrox-screens.r.mikatiming.com/?pid=selfietime_vertical_config_2&lang=EN_CAP" target="_blank" class="accent-text">Link</a></p>
                    <p style="margin-bottom: 5px;">Recovery 2: <a href="https://hyrox-screens.r.mikatiming.com/?pid=selfietime_vertical_config_2_2&lang=EN_CAP" target="_blank" class="accent-text">Link</a></p>
                    <p>Ceremony: <a href="https://hyrox-screens.r.mikatiming.com/?pid=ceremony_screen_config_2&lang=EN_CAP" target="_blank" class="accent-text">Link</a></p>
                </div>
            </div>
        </div>
    </div>

    <script>
        document.querySelectorAll('.accordion-header').forEach(header => {
            header.addEventListener('click', () => {
                const item = header.parentElement;
                const isActive = item.classList.contains('active');
                
                // Close others
                document.querySelectorAll('.accordion-item').forEach(i => i.classList.remove('active'));
                
                if (!isActive) item.classList.add('active');
            });
        });
    </script>
</body>
</html>
