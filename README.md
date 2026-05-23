# Agentic-SOC-Analyst

An intelligent threat hunting assistant that combines natural language processing (OpenAI GPT) with real-time log analysis from Microsoft Defender for Endpoint and Azure AD — rebuilt from scratch to deepen understanding of AI-driven security operations.

This project was built as a hands-on learning exercise: taking a working AI SOC analyst bot and constructing it to understand the integration of LLMs, Azure Log Analytics, function calling, and threat intelligence workflows.

_**Why I built This Bot**_

-Understand how LLMs interpret natural language hunting queries

-Master OpenAI function calling for structured query planning

-Learn secure integration with Azure Log Analytics using KQL

-Implement MITRE ATT&CK mapping and IOC extraction

-Build professional-grade prompt engineering for threat detection

-Practice secure development (secrets management, input validation, guardrails)


_**How it Works**_

-User Input (Natural Language)
       
-GPT decides: Table + Fields + Filters (via Function Calling)
       
-Query Azure Log Analytics Workspace (Real MDE & Azure AD logs)
       
-Returned logs → GPT Threat Analysis Engine
       
-Structured Findings: Title, MITRE Mapping, Confidence, IOCs, Recommendations
       
-Color-coded display + Saved to _threats.jsonl






