# Multi-Agent-Early-Warning-Risk-System

Multi-Agent Early Warning Risk System [LangGraph Agentic Framework] 
Business Context - The bank wants a simple Early Warning Risk Monitoring System. 
You can create a synthetic data - a CSV file containing: 
• Customer ID 
• Loan Amount 
• Days Past Due (DPD) 
• Industry 
• Credit Score 
• Last 3-month transaction trend (Increase / Stable / Decrease) 
• External news sentiment (Positive / Neutral / Negative) 
Goal: Build a Parallel Multi-Agent Risk Assessment System using LangGraph. 
Required Workflow Design - Use Parallel Multi-Agent Architecture. All agents must be 
executed independently and simultaneously. 
Workflow: 
User Input (Customer Data) 
→ Trigger Parallel Agents 
→ Combine Outputs 
→ Final Risk Decision 
Agents Required (Parallel) 
1. Financial Risk Agent 
• Evaluate DPD 
• Evaluate Loan Amount 
• Assign Risk: Low / Medium / High 
• Explain reasoning 
 
2. Behavioral Risk Agent 
• Analyze transaction trend 
• Flag deterioration 
• Assign risk level 
 
3. External Risk Agent 
• Evaluate sentiment 
• Flag negative signals 
• Assign risk level 
 
4. Creditworthiness Agent 
• Evaluate credit score 
• Categorize: 
750 → Low 
650–750 → Medium 
<650 → High 
Final Aggregation Step - After all agents complete: 
• A final combining node must: 
• Collect all outputs 
• Apply rule-based logic 
• Determine Overall Risk: 
o If ≥2 High → High 
o If 1 High + others Medium → Moderate 
o Else → Low 
