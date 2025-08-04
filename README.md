# TRAVEL_PLANNER_AGENT

# 🧳 AI Travel Planner Agent – IBM Watsonx Agentic AI

This project is an interactive **AI-powered travel planning assistant**, built using **IBM Watsonx's Agentic AI platform**. The agent helps users plan personalized travel itineraries by collecting key trip details and generating optimized travel plans automatically.

---

## 🚀 Features

- Interactive and friendly travel assistant chatbot
- Accepts input via:
  - Predefined quick-start questions (button clicks)
  - Natural chat text input
- Gathers key details:
  1. Source and destination cities
  2. Trip duration
  3. Travel mode & food preferences
  4. Number of travelers
  5. Budget
- Automatically suggests the best travel mode if not provided
- Generates a full travel plan including:
  - Transportation options
  - Accommodation recommendations
  - Daily itinerary
  - Food suggestions
  - Estimated total cost
- Deployable as a web chat, embeddable widget, or API

---

## 💡 Technologies Used

- [IBM Watsonx Agentic AI (Granite Model)](https://www.ibm.com/products/watsonx)
- Natural Language Processing (NLP)
- Web chat / embed integration
- IAM Token (for API access)

---

## 🧠 Agent Instruction Logic

The agent follows this behavior model:

- Accept user input via button clicks or free chat
- Parse and store all available trip details
- Identify any missing fields and prompt only for those
- Once all data is collected, generate a complete, structured travel plan
- Auto-suggest travel mode based on distance if user does not specify

---

## 🔧 Setup and Deployment

1. Create a new Agent in [IBM Watsonx Agentic AI](https://dataplatform.cloud.ibm.com/)
2. Bind the Granite model (`granite-3-3-8b-instruct`)
3. Paste the complete **agent instructions** into the model prompt:
   > (See `agent-instructions.txt` in this repo or copy from below)
4. Add 4 Quick Start buttons:
   - Enter source and destination cities
   - Enter number of days
   - Mention travel mode and food preference
   - Enter number of people and budget
5. Deploy the agent
6. Share via:
   - Web chat URL
   - HTML embed `<iframe>`
   - REST API using IAM token and endpoint

---

## 📂 Repository Structure
├── README.md # This file

├── agent-instructions.txt # Full instruction logic used in Granite model

├── images/ # Screenshots of deployment (optional)

└── embed-code.html # Sample embed file (optional)

