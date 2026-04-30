# Sentinel's Journal - Critical Learnings Only

## 2025-05-14 - [Prompt Injection Mitigation in LLM-powered Notebooks]
**Learning:** User-provided text that is directly interpolated into an LLM prompt can be used for prompt injection, potentially overriding instructions or leaking information.
**Action:** Sanitize user inputs by escaping special characters (like quotes) and stripping control characters (like curly braces or brackets) before including them in LLM prompts.
