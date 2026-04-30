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

        /* 100% Fluid Reset */
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
            overflow-x: hidden;
            width: 100%;
        }

        .container {
            width: 100%;
            max-width: 900px;
            margin: 0 auto;
            padding: 20px clamp(15px, 4vw, 30px);
        }

        header {
            margin-bottom: 30px;
            border-bottom: 2px solid var(--accent-color);
            padding-bottom: 15px;
            width: 100%;
        }

        h1 {
            font-size: clamp(24px, 8vw, 42px);
            font-weight: 900;
            text-transform: uppercase;
            line-height: 1;
            letter-spacing: -0.5px;
        }

        .subtitle {
            font-size: 11px;
            color: #888;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            margin-top: 5px;
        }

        h2 {
            font-size: clamp(16px, 5vw, 20px);
            font-weight: 700;
            margin: 40px 0 15px;
            color: var(--accent-color);
            text-transform: uppercase;
        }

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
            align-items: center;
            justify-content: space-between;
            padding: 20px 0;
            background: none;
            border: none;
            color: var(--text-color);
            cursor: pointer;
            text-align: left;
            font-family: inherit;
        }

        .title-wrapper {
            display: flex;
            align-items: center;
            flex: 1;
            min-width: 0;
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

        .accordion-header span {
            font-size: clamp(15px, 4vw, 18px);
            font-weight: 600;
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

        .accordion-content {
            width: 100%;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .accordion-item.active .accordion-content {
            max-height: 2000px;
            padding-bottom: 25px;
        }

        .content-inner {
            font-size: 15px;
            color: #ccc;
        }

        .accent-text {
            color: var(--accent-color);
            text-decoration: none;
            font-weight: 600;
        }

        /* --- TECH TABLE STYLING --- */
        .table-wrapper {
            width: 100%;
            overflow-x: auto;
            -webkit-overflow-scrolling: touch;
            margin: 15px 0;
            border: 1px solid var(--border-color);
            background-color: #000; /* Force black background */
        }

        .tech-table {
            width: 100%;
            min-width: 400px;
            border-collapse: collapse;
            font-family: "Courier New", monospace;
            background-color: #000;
            color: #fff;
        }

        .tech-table thead th {
            background-color: #111;
            color: var(--accent-color);
            text-align: left;
            padding: 12px;
            font-size: 11px;
            text-transform: uppercase;
            border-bottom: 2px solid var(--border-color);
        }

        /* Standardize tbody appearance */
        .tech-table tbody tr {
            background-color: #000;
            border-bottom: 1px solid #1a1a1a;
            transition: background-color 0.2s ease;
        }

        .tech-table tbody td {
            padding: 12px;
            font-size: 14px;
            color: #ffffff; /* Explicit white text */
            vertical-align: middle;
        }

        /* Column Alignment */
        .tech-table th:nth-child(2), 
        .tech-table td:nth-child(2) {
            text-align: center;
        }

        /* Standard Hover Styling */
        .tech-table tbody tr:hover {
            background-color: #111;
        }

        .tech-table tbody tr:hover td {
            color: var(--accent-color);
        }

        .tech-table tbody tr td:first-child {
            border-left: 3px solid transparent;
        }

        .tech-table tbody tr:hover td:first-child {
            border-left: 3px solid var(--accent-color);
        }

        .config-tag {
            color: var(--accent-color);
            font-weight: 800;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            font-size: 14px;
        }

        .config-tag::before {
            content: '';
            width: 3px;
            height: 14px;
            background: var(--accent-color);
            margin-right: 8px;
        }

        @media (min-width: 768px) {
            .container { padding: 40px 20px; }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <div class="main-title">
                <h1>Hyrox</h1>
                <h1>OPS Page – SH</h1>
            </div>
            <p class="subtitle">16–17 MAY 2026 | INTERNAL ONLY</p>
        </header>

        <h2>Venue & Accommodation</h2>
        <div class="accordion">
            <div class="accordion-item">
                <button class="accordion-header">
                    <div class="title-wrapper">
                        <svg class="icon" viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
                        <span>Hotel Details</span>
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <div class="content-inner">
                        <p>SAVHE Hotel Shanghai World Expo</p>
                        <a href="tel:+862168818869" class="accent-text">CALL HOTEL →</a>
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
                        <span>Inventory</span>
                    </div>
                    <svg class="icon chevron" viewBox="0 0 24 24"><polyline points="6 9 12 15 18 9"></polyline></svg>
                </button>
                <div class="accordion-content">
                    <div class="content-inner">
                        <p>Inventory sheet link <a href="https://docs.google.com/spreadsheets/d/1JMlkQguUmbiTYXNGrfLpVmxekoj6HC1PzkG6qDUAYCE/edit?gid=1810257584#gid=1810257584" target="_blank" class="accent-text">HERE</a>.</p>
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
                        <span>Webresults & RDP</span>
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
        </div>
    </div>

    <script>
        document.querySelectorAll('.accordion-header').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.parentElement;
                const isActive = item.classList.contains('active');
                document.querySelectorAll('.accordion-item').forEach(el => el.classList.remove('active'));
                if (!isActive) item.classList.add('active');
            });
        });
    </script>
</body>
</html>
