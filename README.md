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
        }

        /* Essential Reset for Fluidity */
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
            overflow-x: hidden; /* Prevents accidental side-scrolling */
        }

        /* Fluid Container */
        .container {
            width: 100%;
            max-width: 900px;
            margin: 0 auto;
            padding: 20px 15px;
        }

        header {
            margin-bottom: 30px;
            border-bottom: 2px solid var(--accent-color);
            padding-bottom: 15px;
        }

        h1 {
            font-size: clamp(20px, 6vw, 32px); /* Responsive font size */
            font-weight: 800;
            text-transform: uppercase;
            line-height: 1.1;
            margin-bottom: 8px;
        }

        .subtitle {
            font-size: 11px;
            color: #888;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        h2 {
            font-size: 18px;
            font-weight: 600;
            margin: 35px 0 15px;
            color: var(--accent-color);
            text-transform: uppercase;
        }

        /* Accordion Structure - Full Width */
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
            justify-content: space-between; /* Pushes content to edges */
            align-items: center;
            padding: 20px 0;
            background: none;
            border: none;
            color: var(--text-color);
            cursor: pointer;
            text-align: left;
            font-family: inherit;
            font-size: 16px;
            font-weight: 600;
        }

        .title-wrapper {
            display: flex;
            align-items: center;
            padding-right: 10px;
        }

        .icon {
            width: 20px;
            height: 20px;
            margin-right: 12px;
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

        /* Fluid Content Area */
        .accordion-content {
            width: 100%;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.35s cubic-bezier(0.4, 0, 0.2, 1);
            font-size: 15px;
            color: #ccc;
        }

        .accordion-item.active .accordion-content {
            max-height: 2000px; /* Large enough for tables */
            padding-bottom: 25px;
        }

        .content-block {
            margin-bottom: 18px;
        }

        .label {
            color: #777;
            font-size: 11px;
            text-transform: uppercase;
            display: block;
            margin-bottom: 4px;
        }

        .accent-text {
            color: var(--accent-color);
            text-decoration: none;
            font-weight: 600;
            word-break: break-all;
        }

        /* Table Responsiveness Fix */
        .table-wrapper {
            width: 100%;
            overflow-x: auto;
            -webkit-overflow-scrolling: touch;
            margin: 15px 0;
            border: 1px solid var(--border-color);
        }

        .tech-table {
            width: 100%;
            min-width: 450px; /* Ensures table doesn't squash too much */
            border-collapse: collapse;
            font-family: "Courier New", monospace;
        }

        .tech-table th {
            background-color: #111;
            color: var(--accent-color);
            text-align: left;
            padding: 12px;
            font-size: 12px;
            text-transform: uppercase;
        }

        .tech-table td {
            padding: 12px;
            border-bottom: 1px solid #111;
            font-size: 14px;
            color: #fff;
        }

        .config-tag {
            color: var(--accent-color);
            font-weight: 800;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        .config-tag::before {
            content: '';
            width: 4px;
            height: 15px;
            background: var(--accent-color);
            margin-right: 8px;
        }

        /* Desktop Adjustments */
        @media (min-width: 768px) {
            .container { padding: 40px 20px; }
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
                        <svg class="icon" viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
                        Hotel Details
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <div class="content-block">
                        <span class="label">Hotel</span>
                        <p>上海世博萨和酒店 (SAVHE Hotel)</p>
                    </div>
                    <div class="content-block">
                        <span class="label">Address</span>
                        <p>上海市浦东新区雪野路 410 号</p>
                    </div>
                    <a href="tel:+862168818869" class="accent-text">CALL HOTEL →</a>
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
                    <p>The Floor Plan is available <a href="https://drive.google.com/file/d/1pqxaQhYyO0VfSDxzC1daZDAVlMFkqmO0/view?usp=sharing" target="_blank" class="accent-text">HERE</a>.</p>
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
                    <p>Check the Start Wave sheet <a href="https://docs.google.com/spreadsheets/d/1XYsb3mp7i4cLr715llGVElfHz_wbbpjpSXmVr6P8lNA/edit?gid=1391778420#gid=1391778420" target="_blank" class="accent-text">HERE</a>.</p>
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
                    <p>Access the Inventory sheet <a href="https://docs.google.com/spreadsheets/d/1JMlkQguUmbiTYXNGrfLpVmxekoj6HC1PzkG6qDUAYCE/edit?gid=1810257584#gid=1810257584" target="_blank" class="accent-text">HERE</a>.</p>
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
            
            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><rect x="2" y="3" width="20" height="15" rx="2"/><path d="M17 21l-5-4-5 4"/></svg>
                        Screen Links
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
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

    <script>
        document.querySelectorAll('.accordion-header').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.parentElement;
                const isActive = item.classList.contains('active');

                // Toggle logic
                document.querySelectorAll('.accordion-item').forEach(el => el.classList.remove('active'));
                if (!isActive) {
                    item.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
