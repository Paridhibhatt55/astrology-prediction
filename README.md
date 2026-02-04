This project is an Astrology Prediction Website that collects basic user details through a frontend form and generates AI-assisted, guidance-based astrology insights, which are then emailed to the user.
The goal of this project is not to provide deterministic predictions, but to demonstrate:
Responsible use of Large Language Models (LLMs)
Clear prompt design
Human oversight and judgment
End-to-end automation using n8n
Real-world frontend development and deployment

🧩 Project Architecture Overview
Frontend (GitHub Pages)
→ n8n Webhook
→ LLM (Astrologer Prompt)
→ Email Delivery (Gmail OAuth)
User → HTML Form → n8n Webhook → OpenAI Node → Gmail Node → User Email

🖥️ Frontend Details

Technologies Used

HTML

CSS

Vanilla JavaScript

Features

User-friendly astrology form

Input validation (required fields checked on client side)

Clear disclaimer for guidance-only predictions

Fetch API used to send data to n8n securely

Hosted using GitHub Pages

Collected Inputs

Full Name

Email Address

Date of Birth

Time of Birth (optional)

Place of Birth

Area of Focus (Career / Relationships / Health)🖥️ Frontend Details

Technologies Used
HTML
CSS
Vanilla JavaScript

Features

User-friendly astrology form
Input validation (required fields checked on client side)
Clear disclaimer for guidance-only predictions
Fetch API used to send data to n8n securely
Hosted using GitHub Pages
Collected Inputs
Full Name
Email Address
Date of Birth
Time of Birth (optional)
Place of Birth
Area of Focus (Career / Relationships / Health)

🔄 Automation Workflow (n8n)
Workflow Steps
Webhook Node
Receives JSON data from the frontend form
OpenAI (Message a Model) Node
Uses a carefully designed prompt
AI acts as an ethical astrologer
Generates structured, readable guidance

Gmail Node
Sends the generated guidance to the user’s email
Uses Gmail OAuth for secure authentication
Workflow Proof
n8n workflow screenshots / exported JSON are included as part of submission

🤖 Responsible AI Usage Explanation
This project follows responsible AI principles:
AI is used as a decision-support tool, not an authority
Predictions are framed as possibilities and tendencies
No extreme, harmful, or absolute claims are generated
A mandatory disclaimer is included in every output
Prompt design is explicit and constraine

Human judgment is applied in:
Selecting inputs
Designing prompts
Validating outputs
Deciding what is sent to users

The AI does not:
Predict death, disease, or guaranteed outcomes
Replace human interpretation
Operate without constraints
