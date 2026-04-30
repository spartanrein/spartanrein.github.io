<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Ops Page - Hyrox Shanghai</title>
    <style>
        :root {
            --bg-color: #000000;
            --text-color: #ffffff;
            --accent-color: #fceb00; /* Hyrox Yellow */
            --border-color: #333333;
            --font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            --content-font-size: 15px;
        }

        /* Fluid Reset */
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
            overflow-x: hidden;
            width: 100%;
        }

        /* Improved Container Spacing */
        .container {
            width: 100%;
            max-width: 900px;
            margin: 0 auto;
            padding: 40px clamp(15px, 5vw, 35px);
        }

        header {
            margin-bottom: 45px;
            border-bottom: 2px solid var(--accent-color);
            padding-bottom: 20px;
        }

        h1 {
            font-size: clamp(22px, 7vw, 36px);
            font-weight: 800;
            text-transform: uppercase;
            line-height: 1.1;
            margin-bottom: 10px;
        }

        .subtitle {
            font-size: 12px;
            color: #888;
            text-transform: uppercase;
            letter-spacing: 1.5px;
        }

        /* Section Spacing */
        h2 {
            font-size: 19px;
            font-weight: 600;
            margin: 55px 0 25px;
            color: var(--accent-color);
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        /* Accordion Spacing */
        .accordion {
            width: 100%;
            border-top: 1px solid var(--border-color);
        }

        .accordion-item {
            width: 100%;
            border-bottom: 1px solid var(--border-color);
        }

        .accordion-header {
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 26px 0;
            background: none;
            border: none;
            color: var(--text-color);
            cursor: pointer;
            text-align: left;
            font-family: inherit;
            font-size: 17px;
            font-weight: 600;
        }

        .title-wrapper {
            display: flex;
            align-items: center;
            padding-right: 15px;
            flex: 1;
            min-width: 0;
        }

        .icon {
            width: 20px;
            height: 20px;
            margin-right: 14px;
            flex-shrink: 0;
            stroke: currentColor;
            fill: none;
            stroke-width: 2;
        }

        .chevron {
            width: 18px;
            height: 18px;
            stroke: #666;
            transition: transform 0.3s ease;
            flex-shrink: 0;
        }

        .accordion-item.active .chevron {
            transform: rotate(180deg);
            stroke: var(--accent-color);
        }

        .accordion-item.active .accordion-header {
            color: var(--accent-color);
        }

        /* Content Breathing Room */
        .accordion-content {
            width: 100%;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.35s cubic-bezier(0.4, 0, 0.2, 1);
            font-size: var(--content-font-size);
            color: #ccc;
        }

        .accordion-item.active .accordion-content {
            max-height: 2000px;
            padding-bottom: 35px;
        }

        .content-inner {
            line-height: 1.6;
        }

        .content-block {
            margin-bottom: 24px;
        }

        .label {
            color: #777;
            font-size: 11px;
            text-transform: uppercase;
            display: block;
            margin-bottom: 6px;
        }

        .accent-text {
            color: var(--accent-color);
            text-decoration: none;
            font-weight: 600;
            word-break: break-all;
        }

        /* Table Styling */
        .table-wrapper {
            width: 100%;
            margin: 20px 0;
            border: 1px solid var(--border-color);
            background-color: #000;
        }

        .tech-table {
            width: 100%;
            border-collapse: collapse;
            font-family: "Courier New", monospace;
            background-color: #000000;
            table-layout: auto;
        }

        .tech-table th {
            background-color: #111;
            color: var(--accent-color);
            text-align: left;
            padding: 14px 10px;
            font-size: 12px;
            text-transform: uppercase;
            border-bottom: 2px solid var(--border-color);
        }

        .tech-table td {
            padding: 14px 10px;
            border-bottom: 1px solid var(--border-color);
            font-size: 14px;
            color: #ffffff;
            background-color: #000000;
            word-break: break-all;
        }

        .tech-table tbody tr:hover td {
            background-color: #111;
            color: var(--accent-color);
        }

        .config-tag {
            color: var(--accent-color);
            font-weight: 800;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }

        .config-tag::before {
            content: '';
            width: 4px;
            height: 16px;
            background: var(--accent-color);
            margin-right: 10px;
        }

        @media (min-width: 768px) {
            .container { padding: 60px 40px; }
            h2 { font-size: 20px; }
            .accordion-header { font-size: 18px; }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Hyrox</h1>
            <h1>OPS PAGE – SHANGHAI</h1>
            <p class="subtitle">16–17 MAY 2026 | INTERNAL USE ONLY</p>
        </header>

        <h2>Venue & Accommodation</h2>
        <div class="accordion">
            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M3 21h18"></path><path d="M3 7v1a3 3 0 0 0 6 0V7m0 1a3 3 0 0 0 6 0V7m0 1a3 3 0 0 0 6 0V7H3l2-4h14l2 4"></path><path d="M5 21V10.85"></path><path d="M19 21V10.85"></path><path d="M9 21v-4a2 2 0 0 1 4 0v4"></path></svg>
                        Venue Details
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <div class="content-inner">
                        <div class="content-block">
                            <span class="label">Name (EN)</span>
                            <p>SHANGHAI WORLD EXPO EXHIBITION & CONVENTION CENTER</p>
                        </div>
                        <div class="content-block">
                            <span class="label">Address (EN)</span>
                            <p>1099 Guo Zhan Road, Shanghai, China</p>
                        </div>
                        <div class="content-block" style="border-top: 1px solid #222; padding-top: 15px;">
                            <span class="label">名称 (ZH)</span>
                            <p>上海世博展览馆</p>
                        </div>
                        <div class="content-block">
                            <span class="label">地址 (ZH)</span>
                            <p>上海市浦东新区国展路1099号</p>
                        </div>
                    </div>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
                        Hotel Details
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <div class="content-inner">
                        <div class="content-block">
                            <span class="label">Hotel Name (EN)</span>
                            <p>SAVHE Hotel Shanghai World Expo</p>
                        </div>
                        <div class="content-block">
                            <span class="label">Address (EN)</span>
                            <p>No. 410 Xueye Road, Pudong New Area, Shanghai</p>
                        </div>
                        <div class="content-block" style="border-top: 1px solid #222; padding-top: 15px;">
                            <span class="label">酒店名称 (ZH)</span>
                            <p>上海世博萨和酒店</p>
                        </div>
                        <div class="content-block">
                            <span class="label">地址 (ZH)</span>
                            <p>上海市浦东新区雪野路 410 号</p>
                        </div>
                        <a href="tel:+862168818869" class="accent-text">CALL FRONT DESK →</a>
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
                    <div class="content-inner">
                        <p>The Floor Plan is available <a href="https://drive.google.com/file/d/1pqxaQhYyO0VfSDxzC1daZDAVlMFkqmO0/view?usp=sharing" target="_blank" class="accent-text">HERE</a>.</p>
                    </div>
                </div>
            </div>
        </div>

        <h2>Event Information</h2>
        <div class="accordion">
            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"></path></svg>
                        Start Waves
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <div class="content-inner">
                        <p>Check the Start Wave sheet <a href="https://docs.google.com/spreadsheets/d/1XYsb3mp7i4cLr715llGVElfHz_wbbpjpSXmVr6P8lNA/edit?gid=1391778420#gid=1391778420" target="_blank" class="accent-text">HERE</a>.</p>
                    </div>
                </div>
            </div>

            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><circle cx="12" cy="12" r="2"></circle><path d="M16.24 7.76a6 6 0 0 1 0 8.49m-8.48-.01a6 6 0 0 1 0-8.49m11.31-2.82a10 10 0 0 1 0 14.14m-14.14 0a10 10 0 0 1 0-14.14"></path></svg>
                        Loop Channel Assignment
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <div class="content-inner">
                        <p>The Loop Channel Assignment is <a href="https://docs.google.com/spreadsheets/d/1Z4xVx2gqcWqaX_h2xDgRBTwDiTzK9ypVRiJNqTCVAbs/edit?gid=324513968#gid=324513968" target="_blank" class="accent-text">HERE</a>.</p>
                    </div>
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
                    <div class="content-inner">
                        <p>Access the Inventory sheet <a href="https://docs.google.com/spreadsheets/d/1JMlkQguUmbiTYXNGrfLpVmxekoj6HC1PzkG6qDUAYCE/edit?gid=1810257584#gid=1810257584" target="_blank" class="accent-text">HERE</a>.</p>
                    </div>
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
                    <div class="content-inner">
                        <div class="config-tag">Config 2</div>
                        <div class="table-wrapper">
                            <table class="tech-table">
                                <thead>
                                    <tr>
                                        <th>Address</th>
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
                    <div class="content-inner">
                        <div class="config-tag">Config 2</div>
                        <div class="content-block">
                            <p>Lap Screen: <a href="https://hyrox-screens.r.mikatiming.com/?pid=tfd_screen_config_2&lang=EN_CAP" target="_blank" class="accent-text">View</a></p>
                            <p>Finish Screen: <a href="https://hyrox-screens.r.mikatiming.com/?pid=tfd_screen_finish_nat_config_2&lang=EN_CAP" target="_blank" class="accent-text">View</a></p>
                            <p>Recovery 1: <a href="https://hyrox-screens.r.mikatiming.com/?pid=selfietime_vertical_config_2&lang=EN_CAP" target="_blank" class="accent-text">View</a></p>
                            <p>Recovery 2: <a href="https://hyrox-screens.r.mikatiming.com/?pid=selfietime_vertical_config_2_2&lang=EN_CAP" target="_blank" class="accent-text">View</a></p>
                            <p>Ceremony: <a href="https://hyrox-screens.r.mikatiming.com/?pid=ceremony_screen_config_2&lang=EN_CAP" target="_blank" class="accent-text">View</a></p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        if ('scrollRestoration' in history) {
            history.scrollRestoration = 'manual';
        }
        window.scrollTo(0, 0);

        document.querySelectorAll('.accordion-header').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.parentElement;
                const isActive = item.classList.contains('active');

                document.querySelectorAll('.accordion-item').forEach(el => el.classList.remove('active'));
                if (!isActive) {
                    item.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
