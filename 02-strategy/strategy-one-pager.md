# AI Strategy One-Pager - Juno Automated Prioritization

## 1. Problem & Workflow

Our team often prioritizes functionality and speed over conversation quality. JUNO reviews test conversations to ensure NURI understands parents before answering and encourages continued engagement. It identifies issues, prioritizes improvements, and decides whether the product is ready for user testing.

## 2. Target Metrics

The most important KPI for our product is Conversation Continuation Rate. The percentage of conversations where a parent gives a substantive follow-up after NURI responds.

Supporting KPIs include conversation depth, return rate, and proactive-message response rate.

## 3. Autonomy Level

I would not choose **Assist** because the team’s current challenge is that quality principles are often forgotten under time and budget pressure. If JUNO still requires manual activation, it will not truly solve the problem.

## 4. Data & Model Approach

We will not take the shortcut of using a generic LLM with prompts alone, because we have already seen it overlook and inconsistently apply NURI’s standards. We currently rely on a generic LLM, but its response quality is not sufficient to differentiate NURI. We have added extensive manual adjustments to improve quality, and our next step is to build our own RAG system to consistently apply NURI’s standards and reduce reliance on manual intervention.

## 5. Risks & Mitigations

The one-way-door risk is releasing generic LLM responses that feel impersonal or inconsistent, causing parents to lose trust in NURI before we can differentiate the product. The guardrail is a mandatory JUNO release gate: no external testing until RAG-grounded responses pass NURI’s conversation-quality evaluation and receive human approval.

## 6. V1 Scope

IN: JUNO reviews test conversations, evaluates them against NURI’s quality standards, identifies recurring issues, prioritizes improvements, and recommends release readiness.

OUT:

JUNO will not independently release, deploy, or make the final product decision; human approval is always required.
JUNO will not treat functional correctness or the absence of bugs as proof of conversation quality; readiness must be supported by user-behavior and quality evidence.
