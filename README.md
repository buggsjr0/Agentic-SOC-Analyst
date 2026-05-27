# AI Powered SOC Analyst for Microsoft Defender & Azure

An intelligent threat hunting assistant that combines natural language processing (OpenAI GPT) with real-time log analysis from Microsoft Defender for Endpoint and Azure AD. Built from scratch to deepen understanding of AI-driven security operations.

This project was built as a hands-on learning exercise: taking a working AI SOC analyst bot and constructing it to understand the integration of LLMs, Azure Log Analytics, function calling, and threat intelligence workflows.

***

_**📌 Why I built This Bot**_

- Understand how LLMs interpret natural language hunting queries <br>
- Master OpenAI function calling for structured query planning <br>
- Learn secure integration with Azure Log Analytics using KQL <br>
- Implement MITRE ATT&CK mapping and IOC extraction <br>
- Build professional-grade prompt engineering for threat detection <br>
- Practice secure development (secrets management, input validation, guardrails) <br>

***

_**📌 How it Works**_

- User Input (Natural Language) <br>
- GPT decides: Table + Fields + Filters (via Function Calling) <br>
- Query Azure Log Analytics Workspace (Real MDE & Azure AD logs) <br>
- Returned logs → GPT Threat Analysis Engine <br>
- Structured Findings: Title, MITRE Mapping, Confidence, IOCs, Recommendations <br>
- Color-coded display + Saved to _threats.jsonl <br>

***

_**📌 Key Features**_

- Natural language threat hunting "Check for brute force on Emp000555" <br>
- Intelligent table selection with OpeAI function calling <br>
- Real-time querying of Defender for Endpoint and Logs <br>
- Automated MITRE ATT&CK technique mapping <br>
- Confidence scoring and acctionable reccomendations <br>
- Secure design: API keys never committed. <br>

***

_**Project Build Journey**_

This system was built in phases to confirm that each component worked independently to ensure that Agentic SOC Analyst was able to compile complete threat hunts

| Phase | Goal | Key Learnings | 
| ----- | ----- | ----- |
| 1 | Setup & Auth | Azure DefaultAzureCredential & secure key management |
| 2 | Query Planning | OpenAI function calling, structured outputs
| 3 | Log Retrieval	 | KQL construction, pandas for data handling
| 4 | Threat Analysis | Prompt engineering, JSON schema enforcement
| 5 | Output & Logging	 | Colorama formatting, JSONL append mode 
| 6 | Guardrails & Polish | Validation, model selection, error handling, token estimation, rate limit awareness



__**Demo Example**__

***User prompts AI agent:***
> "Any supicous login attempts againt admin accounts in the ladt 48hrs?

Bot responds with
- Detected brute-force attempts from multiple IPs
- Mapped to MITRE
- IOCs extracted (IP addresses, usernames)
- Recommendations based on user input: block IPs, implement lockout policies. 


