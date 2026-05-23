# Agentic-SOC-Analyst

An intelligent threat hunting assistant that combines natural language processing (OpenAI GPT) with real-time log analysis from Microsoft Defender for Endpoint and Azure AD — rebuilt from scratch to deepen understanding of AI-driven security operations.

This project was built as a hands-on learning exercise: taking a working AI SOC analyst bot and constructing it to understand the integration of LLMs, Azure Log Analytics, function calling, and threat intelligence workflows.

***

_**Why I built This Bot**_

-Understand how LLMs interpret natural language hunting queries <br>
-Master OpenAI function calling for structured query planning
-Learn secure integration with Azure Log Analytics using KQL
-Implement MITRE ATT&CK mapping and IOC extraction
-Build professional-grade prompt engineering for threat detection
-Practice secure development (secrets management, input validation, guardrails)

***

_**How it Works**_

-User Input (Natural Language)
-GPT decides: Table + Fields + Filters (via Function Calling)
-Query Azure Log Analytics Workspace (Real MDE & Azure AD logs)
-Returned logs → GPT Threat Analysis Engine
-Structured Findings: Title, MITRE Mapping, Confidence, IOCs, Recommendations
-Color-coded display + Saved to _threats.jsonl

***

_**Key Features**_

-Natural language threat hunting "Check for brute force on Emp000555"
-Intelligent table selection with OpeAI function calling
-Real-time querying of Defender for Endpoint and Logs
-Automated MITRE ATT&CK technique mapping 
-Confidence scoring and acctionable reccomendations
-Secure design: API keys never committed.

***

_**Project Build Journey**_

This system was built in phases to confirm that each component worked independently to ensure that Agentic SOC Analyst was able to compile complete threat hunts

Phase	Goal	Key Learnings
1	Setup & Auth	Azure DefaultAzureCredential, secure key management
2	Query Planning	OpenAI function calling, structured outputs
3	Log Retrieval	KQL construction, pandas for data handling
4	Threat Analysis	Prompt engineering, JSON schema enforcement
5	Output & Logging	Colorama formatting, JSONL append mode
6	Guardrails & Polish	Validation, model selection, error handling, token estimation, rate limit awareness




