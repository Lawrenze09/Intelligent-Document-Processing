 AI-Invoice-Automation-Pipeline
AI-driven financial pipeline that automates bulk extraction of 100+ invoice records from multi-page PDFs into Notion using Google Gemini and Make.com.

AI-Driven Financial Pipeline: 100+ Records in 30 Seconds
The Mission: Productivity Over Manual Labor
I built this project to solve a common business headache: manually typing data from hundreds of invoices into a database. This automated Intelligent Document Processing (IDP) pipeline extracts data from a 7-page "messy" PDF and migrates it directly into a structured Notion Database in seconds.

The Tech Stack (Zero-Cost Architecture)
Orchestration: Make.com (Free Tier).

OCR & Extraction: PDF.co.

Intelligence: Google Gemini AI (Generative AI).

Database: Notion API.

Note on Scale: This project was intentionally capped at 100 records to operate within the no-cost / free tier limits of the APIs used. However, the logic is fully scalable to handle thousands of rows with a professional subscription.

Engineering Challenges (The "Real" Story)
No automation is perfect on the first try. During development, I encountered a Function 'parseJSON' not found error because the AI output included "conversational noise" (extra text) that broke standard JSON parsing.

My Solution: Instead of forcing a fragile JSON parse, I refactored the architecture. I mapped the Array Output directly from Google Gemini into a Make.com Iterator. This pivot made the workflow more stable, cost-efficient, and capable of handling bulk data without crashing.

Visual Proof of Success
1. The "100 Operations" Milestone
![Make Workflow Success](Workflow.png)

This screenshot confirms the workflow successfully processed 100 records in a single execution within free-tier constraints. All modules show "Green" for 100% data throughput.

3. The Final Notion Database
![Notion Result 1](Fixed%20data%20in%20notion%202.png) ![Notion Result 2](Fixed%20data%20in%20notion.png)

From unstructured, multi-page PDFs to a clean, searchable, and organized Notion database.

Key Takeaways
Cost-Efficient Engineering: Maximized the utility of free-tier AI tools to deliver professional results with zero overhead.

Bulk Data Management: Engineered a system to handle high-volume data (100+ rows) efficiently.

Technical Problem Solving: Demonstrated the ability to debug and refactor workflows when standard automation modules fail.
