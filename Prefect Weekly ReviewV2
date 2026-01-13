<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>School Prefect Weekly Review Checklist</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #3498db 0%, #2c3e50 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            border-radius: 12px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.2);
            overflow: hidden;
        }

        .header {
            background: linear-gradient(135deg, #3498db 0%, #2c3e50 100%);
            color: white;
            padding: 30px;
            text-align: center;
        }

        .header h1 {
            font-size: 28px;
            margin-bottom: 10px;
        }

        .header-info {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-top: 20px;
        }

        .header-info input {
            padding: 10px 15px;
            border: none;
            border-radius: 6px;
            font-size: 15px;
            background: rgba(255,255,255,0.95);
        }

        .content {
            padding: 30px;
        }

        .section {
            margin-bottom: 30px;
            border: 2px solid #e0e0e0;
            border-radius: 10px;
            overflow: hidden;
        }

        .section-header {
            background: linear-gradient(135deg, #3498db 0%, #2c3e50 100%);
            color: white;
            padding: 15px 20px;
            font-size: 18px;
            font-weight: bold;
        }

        .section-body {
            padding: 20px;
        }

        .checklist-item {
            display: grid;
            grid-template-columns: 30px 1fr 80px;
            gap: 15px;
            align-items: start;
            padding: 15px;
            border-bottom: 1px solid #f0f0f0;
            transition: background 0.3s;
        }

        .checklist-item:hover {
            background: #f9f9f9;
        }

        .checklist-item:last-child {
            border-bottom: none;
        }

        .checklist-item input[type="checkbox"] {
            width: 20px;
            height: 20px;
            margin-top: 5px;
            cursor: pointer;
            accent-color: #3498db;
        }

        .checklist-item label {
            font-weight: 600;
            color: #333;
            cursor: pointer;
            line-height: 1.6;
        }

        .status-select {
            padding: 6px 10px;
            border: 2px solid #e0e0e0;
            border-radius: 6px;
            font-size: 13px;
            cursor: pointer;
            background: white;
        }

        .status-select:focus {
            outline: none;
            border-color: #3498db;
        }

        .comment-box {
            grid-column: 2 / 4;
            margin-top: 10px;
        }

        .comment-box textarea {
            width: 100%;
            padding: 10px;
            border: 2px solid #e0e0e0;
            border-radius: 6px;
            font-family: inherit;
            font-size: 14px;
            resize: vertical;
            min-height: 60px;
        }

        .comment-box textarea:focus {
            outline: none;
            border-color: #3498db;
        }

        .comment-label {
            font-size: 13px;
            color: #666;
            margin-bottom: 5px;
            display: block;
        }

        .signature-section {
            margin-top: 40px;
            padding: 30px;
            background: #f8f9fa;
            border-radius: 10px;
        }

        .signature-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-top: 20px;
        }

        .signature-box {
            border: 2px solid #3498db;
            border-radius: 8px;
            padding: 20px;
            background: white;
        }

        .signature-box h3 {
            color: #3498db;
            margin-bottom: 15px;
            font-size: 16px;
        }

        .signature-box input {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 6px;
            margin-bottom: 10px;
            font-size: 14px;
        }

        .signature-box input:focus {
            outline: none;
            border-color: #3498db;
        }

        .signature-line {
            border-top: 2px solid #333;
            margin-top: 30px;
            padding-top: 5px;
            text-align: center;
            font-size: 13px;
            color: #666;
        }

        .print-btn {
            background: #27ae60;
            color: white;
            border: none;
            padding: 15px 30px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 16px;
            margin: 20px auto;
            display: block;
            transition: transform 0.2s;
            font-weight: bold;
        }

        .print-btn:hover {
            transform: scale(1.05);
            background: #229954;
        }

        @media print {
            body {
                background: white;
                padding: 0;
            }
            .container {
                box-shadow: none;
                max-width: 100%;
            }
            .print-btn {
                display: none;
            }
        }

        @media (max-width: 768px) {
            .header-info,
            .signature-grid {
                grid-template-columns: 1fr;
            }

            .checklist-item {
                grid-template-columns: 25px 1fr;
            }

            .status-select {
                grid-column: 2;
                margin-top: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>🏫 School Prefect Weekly Review Checklist</h1>
            <div class="header-info">
                <input type="text" id="prefectName" placeholder="Prefect Name">
                <input type="text" id="weekOf" placeholder="Week of (e.g., Jan 13-17, 2026)">
            </div>
        </div>

        <div class="content">
            <!-- Daily Responsibilities Section -->
            <div class="section">
                <div class="section-header">📋 Daily Responsibilities</div>
                <div class="section-body">
                    <div class="checklist-item">
                        <input type="checkbox" id="attendance">
                        <label for="attendance">Attendance & Punctuality Records Maintained</label>
                        <select class="status-select">
                            <option value="">Status</option>
                            <option value="excellent">Excellent</option>
                            <option value="good">Good</option>
                            <option value="needs-improvement">Needs Work</option>
                        </select>
                        <div class="comment-box">
                            <span class="comment-label">Prefect's Comments:</span>
                            <textarea placeholder="Add your comments here..."></textarea>
                        </div>
                    </div>

                    <div class="checklist-item">
                        <input type="checkbox" id="discipline">
                        <label for="discipline">Discipline Maintenance (breaks, lunch, class)</label>
                        <select class="status-select">
                            <option value="">Status</option>
                            <option value="excellent">Excellent</option>
                            <option value="good">Good</option>
                            <option value="needs-improvement">Needs Work</option>
                        </select>
                        <div class="comment-box">
                            <span class="comment-label">Prefect's Comments:</span>
                            <textarea placeholder="Add your comments here..."></textarea>
                        </div>
                    </div>

                    <div class="checklist-item">
                        <input type="checkbox" id="timekeeping">
                        <label for="timekeeping">Timekeeping for Breaks & Lunch</label>
                        <select class="status-select">
                            <option value="">Status</option>
                            <option value="excellent">Excellent</option>
                            <option value="good">Good</option>
                            <option value="needs-improvement">Needs Work</option>
                        </select>
                        <div class="comment-box">
                            <span class="comment-label">Prefect's Comments:</span>
                            <textarea placeholder="Add your comments here..."></textarea>
                        </div>
                    </div>

                    <div class="checklist-item">
                        <input type="checkbox" id="pe-support">
                        <label for="pe-support">PE Time Support & Student Discipline</label>
                        <select class="status-select">
                            <option value="">Status</option>
                            <option value="excellent">Excellent</option>
                            <option value="good">Good</option>
                            <option value="needs-improvement">Needs Work</option>
                        </select>
                        <div class="comment-box">
                            <span class="comment-label">Prefect's Comments:</span>
                            <textarea placeholder="Add your comments here..."></textarea>
                        </div>
                    </div>

                    <div class="checklist-item">
                        <input type="checkbox" id="environment">
                        <label for="environment">Environment Care (classroom tidiness, lobby safety, clean-up duties)</label>
                        <select class="status-select">
                            <option value="">Status</option>
                            <option value="excellent">Excellent</option>
                            <option value="good">Good</option>
                            <option value="needs-improvement">Needs Work</option>
                        </select>
                        <div class="comment-box">
                            <span class="comment-label">Prefect's Comments:</span>
                            <textarea placeholder="Add your comments here..."></textarea>
                        </div>
                    </div>

                    <div class="checklist-item">
                        <input type="checkbox" id="language">
                        <label for="language">Language Monitoring (gentle reminders given)</label>
                        <select class="status-select">
                            <option value="">Status</option>
                            <option value="excellent">Excellent</option>
                            <option value="good">Good</option>
                            <option value="needs-improvement">Needs Work</option>
                        </select>
                        <div class="comment-box">
                            <span class="comment-label">Prefect's Comments:</span>
                            <textarea placeholder="Add your comments here..."></textarea>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Weekly Responsibilities Section -->
            <div class="section">
                <div class="section-header">📅 Weekly Responsibilities</div>
                <div class="section-body">
                    <div class="checklist-item">
                        <input type="checkbox" id="assembly">
                        <label for="assembly">Weekly Assembly Coordination & MC Duties</label>
                        <select class="status-select">
                            <option value="">Status</option>
                            <option value="excellent">Excellent</option>
                            <option value="good">Good</option>
                            <option value="needs-improvement">Needs Work</option>
                        </select>
                        <div class="comment-box">
                            <span class="comment-label">Prefect's Comments:</span>
                            <textarea placeholder="Add your comments here..."></textarea>
                        </div>
                    </div>

                    <div class="checklist-item">
                        <input type="checkbox" id="activities">
                        <label for="activities">Activity Coordination (Fun Friday, monthly activities)</label>
                        <select class="status-select">
                            <option value="">Status</option>
                            <option value="excellent">Excellent</option>
                            <option value="good">Good</option>
                            <option value="needs-improvement">Needs Work</option>
                        </select>
                        <div class="comment-box">
                            <span class="comment-label">Prefect's Comments:</span>
                            <textarea placeholder="Add your comments here..."></textarea>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Teacher's Evaluation Section -->
            <div class="section">
                <div class="section-header">👨‍🏫 Teacher's Evaluation</div>
                <div class="section-body">
                    <div class="comment-box" style="grid-column: 1;">
                        <span class="comment-label"><strong>Academic Performance Feedback:</strong></span>
                        <textarea placeholder="Teacher's feedback on attendance records, progress, and areas of improvement..."></textarea>
                    </div>

                    <div class="comment-box" style="grid-column: 1; margin-top: 20px;">
                        <span class="comment-label"><strong>Behavioural Evaluation:</strong></span>
                        <textarea placeholder="Evaluate discipline, cooperation, recurring issues, and positive contributions (teamwork, leadership)..."></textarea>
                    </div>

                    <div class="comment-box" style="grid-column: 1; margin-top: 20px;">
                        <span class="comment-label"><strong>Areas for Improvement:</strong></span>
                        <textarea placeholder="Specific areas where the prefect can improve..."></textarea>
                    </div>

                    <div class="comment-box" style="grid-column: 1; margin-top: 20px;">
                        <span class="comment-label"><strong>Positive Recognition:</strong></span>
                        <textarea placeholder="Acknowledge positive contributions, leadership qualities, and teamwork..."></textarea>
                    </div>
                </div>
            </div>

            <!-- Signature Section -->
            <div class="signature-section">
                <h2 style="text-align: center; color: #2c3e50; margin-bottom: 20px;">✍️ Signatures</h2>
                <div class="signature-grid">
                    <div class="signature-box">
                        <h3>Prefect</h3>
                        <input type="text" placeholder="Prefect's Full Name" id="prefectSigName">
                        <input type="date" id="prefectDate">
                        <div class="signature-line">Prefect's Signature</div>
                    </div>

                    <div class="signature-box">
                        <h3>Teacher</h3>
                        <input type="text" placeholder="Teacher's Full Name" id="teacherSigName">
                        <input type="date" id="teacherDate">
                        <div class="signature-line">Teacher's Signature</div>
                    </div>
                </div>
            </div>

            <button class="print-btn" onclick="window.print()">🖨️ Print Checklist</button>
        </div>
    </div>

    <script>
        // Auto-fill today's date for signature fields
        const today = new Date().toISOString().split('T')[0];
        document.getElementById('prefectDate').value = today;
        document.getElementById('teacherDate').value = today;

        // Auto-populate prefect name in signature if filled in header
        document.getElementById('prefectName').addEventListener('input', function() {
            document.getElementById('prefectSigName').value = this.value;
        });
    </script>
</body>
</html>
