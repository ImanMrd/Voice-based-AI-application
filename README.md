<div align="center">
  <img src="stellantis_ai_concept.jpg" alt="Industrial AI Voice Assistant Concept" width="100%">
</div>

# 🏭 Industrial AI Voice Assistant (Stellantis Thesis Project)

> 🔒 **Security Notice:** Due to Non-Disclosure Agreements (NDA) and corporate security policies with Stellantis, the proprietary source code for this project cannot be made public. This repository serves as an architectural overview of the platform developed for my MSc Thesis in Mechatronics Engineering.

## 📌 The Business Challenge
On the Fiat 500 BEV production line, electricians at the repair area (*Piazzale*) were required to manually enter defect data into a digital SharePoint system. 
This manual data entry process required taking off gloves, walking to a PC, typing out the issue, and searching through drop-down menus. It took approximately **5 minutes per defect**, pulling skilled workers away from actual repair tasks and slowing down production.

## 💡 The Solution
I designed and developed a **Voice-Based AI Application** that allows workers to report defects completely hands-free. They simply speak naturally about the issue, and the AI handles the rest.

## 🚀 How It Works (In Plain English)
1. **Audio Capture:** The worker speaks into the system (e.g., "The front left headlight is scratched").
2. **Speech-to-Text (Whisper):** A highly advanced AI model transcribes the Italian industrial audio into text.
3. **Data Extraction (Claude LLM):** An AI "brain" analyzes the text and automatically extracts the correct categories (Sequence, Tipologia, Defect Type).
4. **Database Sync (Power Automate):** The system instantly pushes the organized data directly into the corporate SharePoint database.

## 🛠️ Technology Architecture
*   **Frontend:** A Desktop Application built with Python (Streamlit) featuring a push-to-talk interface for the factory floor.
*   **Backend AI (Databricks):** Secure enterprise environment hosting the Large Language Models (Whisper Large v3 & Anthropic Claude 3 Haiku).
*   **Database Integration:** Microsoft Power Automate & SharePoint List for secure corporate data storage.
*   **Deployment:** A custom launcher so factory workers never have to touch a command line or terminal.

## 📊 Business Value Delivered
*   **Time Savings:** Reduced the data entry process from **~5 minutes down to ~1 minute** per defect.
*   **Worker Efficiency:** Allowed electricians to remain focused on diagnosing and fixing vehicles rather than doing administrative typing.
*   **Data Accuracy:** The AI is trained to understand factory-specific jargon and acronyms, ensuring the final database is perfectly organized.
*   **Enterprise Security:** The entire system was built to operate strictly within the corporate IT policies, ensuring data never leaked outside approved networks.

---
*Created by [Iman Moradi Nezhad](https://github.com/ImanMrd) | Showcasing Enterprise AI Integration and Industrial Automation.*
