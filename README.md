AI-Powered Insurance Claims Processing Agent
--------------------------------------------
Hi! This project is a prototype of an automated insurance claims processing system built using Python and Streamlit.
The goal of this project is to simulate how insurance companies can use AI to read claim documents, validate information, detect risks, and automatically decide how the claim should be handled.
Instead of manually reviewing every claim, this system acts like a mini digital claims officer.

The idea is to simulate how insurance companies handle First Notice of Loss (FNOL) documents and reduce the need for manual effort during the initial claim review stage. Instead of a human reading every document line by line, this system acts like a digital claims assistant that can read the document, understand key information, check for missing details, and decide how the claim should be handled.

Information Extracted
---------------------
The system attempts to identify:
Policy Number
Insured Name
Date of Loss
Location of Incident
Accident Description
Estimated Damage Amount
Claim Type (Vehicle / Injury / etc.)

| Condition                      | Decision         |
| ------------------------------ | ---------------- |
| Mandatory fields missing       | Manual Review    |
| Fraud-related words detected   | Investigation    |
| Injury-related claim           | Specialist Queue |
| Low damage estimate (< 25,000) | Fast-track       |
| Otherwise                      | Manual Review    |

Additional Smart Features
-------------------------
🔴 Fraud keyword highlighting
🧠 Claim type detection using text analysis
📈 Confidence score based on data completeness
📄 Downloadable AI-generated claim report
🌐 Interactive web interface

🛠 Technologies Used
--------------------
Python
Streamlit (Web App Interface)
pdfplumber (PDF text extraction)
Regex (Field detection)
Rule-based AI logic

How to Run This Project
-----------------------
1. Install dependencies
pip install streamlit pdfplumber

2. Run the app
streamlit run app.py

3. Open in browser
Upload an FNOL PDF and view the AI processing results.

Author
------
Maryala Sanjana
B.Tech – Information Technology
