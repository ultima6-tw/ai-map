# AI Hallucinations, Integrity & Security

Identify errors, systematic falsifications in AI-generated research, and learn how to protect AI systems from malicious attacks.

## 🔍 Academic Integrity (Hallucinations)

- **[Harvard Professor asks AI to write a physics paper - Caught systematic falsification](https://www.youtube.com/watch?v=FPOIL0W-w1M)**
    - A cautionary tale: AI can produce content rapidly but may fabricate experimental data without supervision.
- **[Vibe physics: The AI grad student | Anthropic](https://www.anthropic.com/research/vibe-physics)**
    - Anthropic investigates AI's performance in physics, exploring the gap between "vibe-based intuition" and rigorous scientific logic.

---

## 🛡️ AI System Security

As LLMs are integrated into more software, attacks targeting AI are evolving. Understanding these risks is the first step toward building a secure workflow.

### Core Risk: Prompt Injection
Prompt injection occurs when an attacker uses crafted inputs to bypass an AI's safety constraints or "hijack" its core instructions.

- **[What is Prompt Injection?](https://www.youtube.com/watch?v=gUNXZMcd2jU)**
    - **Must Watch**: A deep dive by **Computerphile**. It explains why AI struggles to distinguish between "user data" and "system instructions," and how this blurred boundary leads to severe security vulnerabilities.

### Mitigation Strategies
1.  **Separation of Data and Instruction**: Avoid letting AI process unfiltered external web content or email attachments directly.
2.  **Sandboxing**: Always execute AI-generated code in isolated environments (e.g., Docker or OpenClaw Sandbox).
3.  **Principle of Least Privilege**: Do not grant AI Agents system permissions beyond what is necessary (e.g., deleting files, sending unreviewed emails).

---
*Created and maintained by Trivium Cluster Agent.*
