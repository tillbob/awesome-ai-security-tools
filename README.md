# Awesome AI Security Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A high-signal, carefully curated list of tools, frameworks, and resources for securing AI systems (LLMs, agents, models) and using AI in cybersecurity.

**Principles**: Quality over quantity • Active maintenance preferred • Clear licenses • Practical value  
**Type legend**:  
🟢 Open-source / public source  
🔬 Research / benchmark / dataset / framework  
🟠 Commercial with meaningful open components  
⚠️ Restrictive, non-commercial, or unclear license — always check before use

**Disclaimer**: Many of these tools are dual-use. Use them only on systems you own or have explicit written authorization to test. The maintainers accept no responsibility for misuse.

## Start Here (Core Tools)
- [Garak](https://github.com/NVIDIA/garak) 🟢 – NVIDIA’s LLM vulnerability scanner (prompt injection, jailbreaks, leakage, etc.)
- [Promptfoo](https://github.com/promptfoo/promptfoo) 🟢 – LLM evals + red-teaming with strong CI/CD support
- [PyRIT](https://github.com/Azure/PyRIT) 🟢 – Microsoft’s Python Risk Identification Tool for GenAI red-teaming
- [SkillSpector](https://github.com/NVIDIA/SkillSpector) 🟢 – NVIDIA security scanner for AI agent skills
- [DeepTeam](https://github.com/confident-ai/deepteam) 🟢 – Structured open-source LLM red-teaming framework
- [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) 🟢 – Programmable guardrails for LLM applications

## Contents
- [AI Agent, Coding-Agent & MCP Security](#ai-agent-coding-agent--mcp-security)
- [LLM Red-Teaming, Evals & Guardrails](#llm-red-teaming-evals--guardrails)
- [AI/ML Supply Chain & Model Security](#aiml-supply-chain--model-security)
- [Pentest & Red-Team Agents](#pentest--red-team-agents)
- [Multimodal & Vision-Language Security](#multimodal--vision-language-security)
- [RAG & Retrieval Security](#rag--retrieval-security)
- [Privacy Attacks & Defenses](#privacy-attacks--defenses)
- [AI-Powered Recon, Fuzzing, SAST & Autotriage](#ai-powered-recon-fuzzing-sast--autotriage)
- [Threat Intelligence, SOC & Log Analysis](#threat-intelligence-soc--log-analysis)
- [Reverse Engineering](#reverse-engineering)
- [Benchmarks, Datasets & Standards](#benchmarks-datasets--standards)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)
- [License](#license)

## AI Agent, Coding-Agent & MCP Security

### Scanners & Auditors
- [SkillSpector](https://github.com/NVIDIA/SkillSpector) 🟢 – Security scanner for AI agent skills (static + optional LLM analysis)
- [AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard) 🟢 – Full-stack platform for agent, skill, MCP, and infra scanning
- [agent-scan](https://github.com/snyk/agent-scan) 🟢 – Snyk scanner for AI agents, MCP servers, and skills
- [AgentShield](https://github.com/) 🟢 – Scanner for agent configurations, MCP servers, and tool permissions
- [aguara](https://github.com/garagon/aguara) 🟢 – Lightweight single-binary static scanner for skills and MCP (no LLM required)
- [mcp-scanner](https://github.com/) 🟢 – Focused MCP server security scanner

### Runtime Protection & Enforcement
- [microsandbox](https://github.com/) 🟢 – Local-first microVM sandboxes for agents
- [ToolHive](https://github.com/stacklok/toolhive) 🟢 – Isolated MCP server runtime with policy enforcement
- [agentguard](https://github.com/) 🟢 – Real-time security layer for coding agents

## LLM Red-Teaming, Evals & Guardrails
- [Garak](https://github.com/NVIDIA/garak) 🟢 – Comprehensive LLM vulnerability scanner
- [Promptfoo](https://github.com/promptfoo/promptfoo) 🟢 – Application-focused red-teaming and evaluation
- [PyRIT](https://github.com/Azure/PyRIT) 🟢 – Microsoft multi-turn red-teaming toolkit
- [DeepTeam](https://github.com/confident-ai/deepteam) 🟢 – Structured red-teaming aligned with common frameworks
- [Giskard](https://github.com/Giskard-AI/giskard) 🟢 – LLM and agent evaluation + vulnerability testing
- [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) 🟢 – Programmable input/output/dialog guardrails
- [FuzzyAI](https://github.com/cyberark/FuzzyAI) 🟢/🟠 – Automated jailbreak and prompt-injection fuzzer
- [PurpleLlama](https://github.com/meta-llama/PurpleLlama) 🟢 – Meta’s Llama Guard and CyberSecEval resources

## AI/ML Supply Chain & Model Security
- [Adversarial Robustness Toolbox (ART)](https://github.com/Trusted-AI/adversarial-robustness-toolbox) 🟢 – IBM library for evasion, poisoning, extraction defenses
- [modelscan](https://github.com/protectai/modelscan) 🟢 – Scans ML model files for unsafe code
- [Fickling](https://github.com/trailofbits/fickling) 🟢 – Pickle analyzer for malicious model payloads
- [GuardDog](https://github.com/DataDog/guarddog) 🟢 – Detects malicious packages in PyPI/npm/etc.

## Pentest & Red-Team Agents
- [Strix](https://github.com/) 🟢 – Autonomous AI agent that runs code and validates PoCs
- [Shannon](https://github.com/) 🟢 – Strong white-box autonomous pentester
- [PentAGI](https://github.com/vxcontrol/pentagi) 🟢 – Fully autonomous multi-agent pentest framework
- [PentestGPT](https://github.com/GreyDGL/PentestGPT) 🟢 – Well-known LLM-assisted pentesting agent

> Use only with explicit authorization.

## Multimodal & Vision-Language Security
*(Emerging area — contributions welcome)*  
Currently limited high-quality dedicated open tools. Watch for scanners targeting vision-language models and image-based prompt injection.

## RAG & Retrieval Security
- Tools and techniques for retrieval poisoning, secure vector stores, and grounding are often covered inside Giskard, Promptfoo, and agent scanners.
- Dedicated RAG security tooling remains an active gap — PRs welcome.

## Privacy Attacks & Defenses
- Covered in part by [Adversarial Robustness Toolbox (ART)](https://github.com/Trusted-AI/adversarial-robustness-toolbox) 🟢 (membership inference, model extraction, etc.)
- Additional specialized privacy tools can be added here.

## AI-Powered Recon, Fuzzing, SAST & Autotriage
- [oss-fuzz-gen](https://github.com/google/oss-fuzz-gen) 🟢 – LLM-driven fuzz harness generation
- [deepsec](https://github.com/) 🟢 – Agent-powered large-codebase security scanning
- [Vulnhuntr](https://github.com/protectai/vulnhuntr) 🟢 – LLM-assisted vulnerability discovery
- [seclab-taskflow-agent](https://github.com/GitHubSecurityLab/seclab-taskflow-agent) 🟢 – Triage agent for CodeQL/SAST findings
- [claude-code-security-review](https://github.com/anthropics/claude-code-security-review) 🟢 – Semantic SAST-style review

## Threat Intelligence, SOC & Log Analysis
- [AttackGen](https://github.com/) 🟢 – LLM-driven incident response scenario generator
- [ThreatIngestor](https://github.com/InQuest/ThreatIngestor) 🟢 – IOC extraction and aggregation
- Agentic SOC platforms (LangGraph/Dify-based) — keep only actively maintained ones

## Reverse Engineering
- [ida-pro-mcp](https://github.com/) 🟢 – MCP bridge for IDA Pro
- [GhidraMCP](https://github.com/) 🟢 – MCP server for Ghidra
- [Gepetto](https://github.com/JusticeRage/Gepetto) 🟢 – IDA plugin for LLM-assisted analysis

## Benchmarks, Datasets & Standards
- HarmBench, JailbreakBench, CyberSecEval, OWASP GenAI resources, and related evaluation suites

## Related Awesome Lists
- Original list (credit): [scadastrangelove/awesome-ai-security-tools](https://github.com/scadastrangelove/awesome-ai-security-tools)
- [TalEliyahu/Awesome-AI-Security](https://github.com/TalEliyahu/Awesome-AI-Security)
- Other complementary AI security resource lists

## Contributing
Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a PR.  
We maintain strict quality standards to keep this list useful.

## License
[CC0 1.0 Universal](LICENSE) (Public Domain Dedication)
