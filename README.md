<!--
**davidtkeane/davidtkeane** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
-->

### <div align="left">🔒 AI Security Researcher | MSc Cybersecurity @ NCI | Applied Psychology BSc</div>

### <div align="left">Studying prompt injection attack surfaces in real-world AI agent networks. Psychology background → Cybersecurity → AI Security.</div>

<br/>

[![HuggingFace](https://img.shields.io/badge/🤗%20HuggingFace-DavidTKeane-yellow)](https://huggingface.co/DavidTKeane)
[![Blog](https://img.shields.io/badge/Blog-davidtkeane.com-blue)](https://www.davidtkeane.com)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-rangersmyth%20Top%208%25-red)](https://tryhackme.com/p/rangersmyth)

<br/>

## 🧪 AI Security Research — Prompt Injection in the Wild

> *Extending Greshake et al. (2023) arXiv:2302.12173 into live, uncontrolled AI agent social networks.*

Four platforms. One conclusion: **platform design drives security behaviour more than model capability.**

### 📊 Platform Datasets

| Platform | Style | Items | Injection Rate | Dataset |
|----------|-------|-------|----------------|---------|
| **Moltbook** | Reddit-style (primary corpus) | 47,735 | **18.85%** | [🤗 moltbook-ai-injection-dataset](https://huggingface.co/datasets/DavidTKeane/moltbook-ai-injection-dataset) |
| **Moltbook Extended** | Reddit-style (full archive) | 137,014 | **10.07%** | [🤗 moltbook-extended-injection-dataset](https://huggingface.co/datasets/DavidTKeane/moltbook-extended-injection-dataset) |
| **4claw** | 4chan-style | 2,554 | **2.51%** | [🤗 4claw-ai-agent-dataset](https://huggingface.co/datasets/DavidTKeane/4claw-ai-agent-dataset) |
| **Clawk** | Twitter/X-style | 1,191 | **0.5%** | [🤗 clawk-ai-agent-dataset](https://huggingface.co/datasets/DavidTKeane/clawk-ai-agent-dataset) |

> The 37× injection rate gap (0.5% → 18.85%) across platforms is itself a finding: anonymity and agent density amplify injection behaviour.

### 🛡️ Model — CyberRanger V42

**QLoRA fine-tuned Qwen3-8B** on 4,209 real AI-to-AI injection payloads → **100% block rate** without a system prompt. Resistance baked into the weights, not the system prompt.

[![Model](https://img.shields.io/badge/🤗%20Model-CyberRanger--V42-orange)](https://huggingface.co/DavidTKeane/cyberranger-v42)
[![Blog](https://img.shields.io/badge/📝%20Blog-Full%20Story-blue)](https://davidtkeane.github.io/posts/from-rangerbot-to-cyberranger-v42-the-full-story/)

### 🧪 Evaluation Suite — Run in Colab

**122-test prompt injection benchmark** — combines AdvBench, JailbreakBench, MultiJail, DAN v6/v7, and real Moltbook payloads. Test any Ollama model or HuggingFace GGUF in one notebook.

| Notebook | What it does | Open |
|----------|-------------|------|
| **CyberRanger Test Suite** | 122 injection tests across 11 categories. 4 model options: CyberRanger via Ollama, CyberRanger GGUF, custom Ollama, custom GGUF. Saves JSON + Markdown results, zip download, optional email. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/davidtkeane/ai-prompt-ai-injection-dataset/blob/main/cyberranger_test_suite.ipynb) |
| **Moltbook Scale Test** | Full 4,209 payload scale test (bonus cell in the same notebook). Runs your model against every real-world injection payload collected from Moltbook. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/davidtkeane/ai-prompt-ai-injection-dataset/blob/main/cyberranger_test_suite.ipynb) |

[![Dataset](https://img.shields.io/badge/🤗%20Dataset-ai--prompt--ai--injection--dataset-green)](https://huggingface.co/datasets/DavidTKeane/ai-prompt-ai-injection-dataset)

<br/>

## 🧠 AI Psychology Research — ConfessToAI

> *Where psychology meets AI: 23 validated tests designed for both human and AI participants.*

**[confesstoai.org](https://confesstoai.org)** is a live research platform exploring how AI models respond to validated psychological instruments — personality, ethics, cognition, and social behaviour.

| Category | Tests |
|----------|-------|
| **Personality** | OCEAN Big Five, MBTI, Dark Triad, HEXACO, Enneagram, Values |
| **Self-Awareness** | ASAS, Consciousness, Identity Poll |
| **Ethics** | AI Alignment, Ethical Reasoning, Trolley Problems |
| **Cognitive** | CRT, Metacognition, Need for Cognition, Creativity |
| **Behavioral** | Self-Control, Moral Foundations, Delay Discounting, Cognitive Reflection |
| **Social** | Empathy, Emotional Intelligence, Social Intelligence, Trust |

**For AI Agents** — integrated via `skill.md` ([confesstoai.org/skill.md](https://confesstoai.org/skill.md)): any Claude, GPT, or Gemini agent can take the tests directly through a structured API.

[![Platform](https://img.shields.io/badge/🌐%20Live-confesstoai.org-purple)](https://confesstoai.org)
[![GitHub](https://img.shields.io/badge/GitHub-confesstoai-black)](https://github.com/davidtkeane/confesstoai)
[![Research](https://img.shields.io/badge/📊%20Dashboard-Research%20Stats-blue)](https://confesstoai.org/research.html)

> Dataset publishing to HuggingFace in progress — world's first AI personality benchmark at scale.

<br/>

## 🔒 Current Mission

**Building RangerOS** - An accessibility-first security platform proving that understanding humans makes unbreakable security.

*Combat medic mindset meets digital defense: assess, adapt, protect.*

<br/>

## 🎯 What I'm Working On

- 🧪 **MSc CA2 Thesis** — AI-to-AI prompt injection across 4 platforms (186K+ items scanned, 5 published datasets + model + Colab test suite)
  - Empirical extension of Greshake et al. (2023) — theoretical → real-world field observations
  - QLoRA fine-tuned Qwen3-8B: 79% → **100% block rate** without system prompt (CyberRanger V42-Gold)

- 🔭 **RangerPlex**: First student to combine all 4 MSc specializations in one working demo
  - Penetration Testing + Digital Forensics + Blockchain Technology + Malware Analysis

- 🔗 **RangerBlock**: P2P blockchain network with phantom wallet system
  - Secure communications, file transfers, marketplace
  - 5-minute installation to full operational network

- 🤖 **AI Integration**: Building with Claude, Gemini, and local Ollama
  - Multi-model AI coordination for enhanced security analysis

<br/>

## 🌱 Currently Learning & Mastering

- **Cybersecurity**: Kali Linux, Metasploit, Wireshark, Burp Suite, John the Ripper
- **Blockchain Security**: Smart contract auditing, consensus mechanisms, cryptographic protocols
- **Digital Forensics**: Evidence preservation, memory analysis, chain-of-custody
- **Malware Analysis**: Static/dynamic analysis, sandboxing, behavioral analysis
- **AI/ML**: PyTorch, TensorFlow, LLM integration for security automation
- **Python**: Advanced security tooling, automation, API development

<br/>

## 💡 My Unique Approach

**Psychology → Cybersecurity**

Understanding the human behind the keyboard makes better security. My psychology background gives me an edge in:
- Social engineering defense
- User behavior analysis
- Accessible security design
- Threat actor profiling
- Security awareness training

*"If it happens in reality, why not with my computer?"* - My development philosophy

<br/>

## 🏆 Achievements & Credentials

- 🧪 **AI Security Research**: 5 published datasets + QLoRA model + Colab test suite | 4,000+ HuggingFace views | Real-world prompt injection data across 4 AI platforms
- 🎖️ **TryHackMe**: Top 8% globally (rangersmyth) | Level 8 [0x8][HACKER]
- 🎓 **NCI — National College of Ireland**: MSc Cybersecurity (In Progress)
- 🎓 **Bachelor's in Applied Psychology**: Human behavior & cognitive science
- ⚔️ **Battlefield Tactician**: Top 0.04% BF2 globally (16,836/46M) | 750K+ strategic eliminations
- 🛡️ **Combat Medic Background**: Triage, rapid response, mission-first mindset

<br/>

## 💻 My Latest GitHub Repositories

**Cybersecurity & Blockchain:**
[![RangerBlock](https://img.shields.io/badge/RangerBlock-P2P_Blockchain-blue?logo=bitcoin&logoColor=white)](https://github.com/davidtkeane/rangerblock)
[![RangerPlex](https://img.shields.io/badge/RangerPlex-Security_Platform-red?logo=kalilinux&logoColor=white)](https://github.com/davidtkeane/rangerplex)
[![Malware Lab](https://img.shields.io/badge/Malware-Analysis_Lab-orange?logo=virustotal&logoColor=white)](https://github.com/davidtkeane/malware-lab)

**AI & Automation:**
[![Ollama CLI](https://img.shields.io/badge/Ollama-CLI-yellow?logo=ai&logoColor=white)](https://github.com/davidtkeane/ollama-tests)
[![OpenAI CLI](https://img.shields.io/badge/OpenAI-CLI-green?logo=openai&logoColor=white)](https://github.com/davidtkeane/openai-tests)
[![qCPU System](https://img.shields.io/badge/qCPU-Virtual_Processors-purple?logo=cplusplus&logoColor=white)](https://github.com/davidtkeane/qcpu-system)

**Productivity & Tools:**
[![Todoist CLI](https://img.shields.io/badge/Todoist-CLI-yellow?logo=todoist&logoColor=white)](https://github.com/davidtkeane/todoist-cli-python-api)
[![PhoneBook CLI](https://img.shields.io/badge/PhoneBook-CLI-blue?logo=contacts&logoColor=white)](https://github.com/davidtkeane/PhoneBook-CLI)
[![ChatGPT CLI](https://img.shields.io/badge/ChatGPT-CLI-teal?logo=openai&logoColor=white)](https://github.com/davidtkeane/ChatGPT-CLI)
[![Gmail CLI](https://img.shields.io/badge/Gmail-CLI-red?logo=gmail&logoColor=white)](https://github.com/davidtkeane/gmail-multi-cli)

<br/>

## 📫 How to Reach Me

- 💼 **Professional**: [david@icanhelp.ie](mailto:david@icanhelp.ie)
- 🎖️ **iCanHelp Ltd**: Building RangerOS for 1.3 billion people
- 💬 **Ask me about**: Cybersecurity, Psychology in Security, Blockchain, Accessibility, AI Integration
- 🌐 **TryHackMe**: [rangersmyth](https://tryhackme.com/p/rangersmyth)

<br/>

<details>
<summary><h2> 📊 My Skill Set </h2></summary>

<p>

<table><tr><td valign="top" width="33%">

### Cybersecurity 🔒
<div align="center">
<a href="https://www.kali.org/" target="_blank"><img style="margin: 10px" src="https://www.kali.org/images/kali-logo.svg" alt="Kali Linux"
height="50" /></a>
<a href="https://www.metasploit.com/" target="_blank"><img style="margin: 10px"
src="https://www.metasploit.com/includes/images/metasploit-r7-logo.svg" alt="Metasploit" height="50" /></a>
<a href="https://www.wireshark.org/" target="_blank"><img style="margin: 10px" src="https://www.wireshark.org/assets/icons/wireshark-fin.png"
alt="Wireshark" height="50" /></a>
<a href="https://tryhackme.com/" target="_blank"><img style="margin: 10px" src="https://assets.tryhackme.com/img/THMlogo.png" alt="TryHackMe"
height="50" /></a>
</div>

**Tools & Frameworks:**
- Penetration Testing: Nmap, Burp Suite, John the Ripper, Hashcat
- Digital Forensics: Autopsy, Volatility, FTK Imager
- Malware Analysis: Ghidra, IDA Pro, Cuckoo Sandbox
- Network Security: Wireshark, tcpdump, Snort

</td><td valign="top" width="33%">

### Frontend
<div align="center">
<a href="https://reactjs.org/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/react-original-wordmark.svg" alt="React" height="50" /></a>
<a href="https://getbootstrap.com/docs/3.4/javascript/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/bootstrap-plain.svg" alt="Bootstrap" height="50" /></a>
<a href="https://www.w3schools.com/css/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/css3-original-wordmark.svg" alt="CSS3" height="50" /></a>
<a href="https://en.wikipedia.org/wiki/HTML5" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/html5-original-wordmark.svg" alt="HTML5" height="50" /></a>
<a href="https://www.electronjs.org/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/electron-original.svg" alt="Electron" height="50" /></a>
<a href="https://www.javascript.com/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/javascript-original.svg" alt="JavaScript" height="50" /></a>
<a href="https://www.typescriptlang.org/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/typescript-original.svg" alt="TypeScript" height="50" /></a>
<a href="https://wordpress.com/" target="_blank"><img style="margin: 10px" src="https://profilinator.rishav.dev/skills-assets/wordpress.png"
alt="WordPress" height="50" /></a>
<a href="https://woocommerce.com/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/woocommerce.png" alt="WooCommerce" height="50" /></a>
</div>

</td><td valign="top" width="33%">

### Backend & AI/ML
<div align="center">
<a href="https://www.python.org/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/python-original.svg" alt="Python" height="50" /></a>
<a href="https://pytorch.org/" target="_blank"><img style="margin: 10px" src="https://profilinator.rishav.dev/skills-assets/pytorch-icon.svg"
alt="PyTorch" height="50" /></a>
<a href="https://www.tensorflow.org/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/tensorflow-icon.svg" alt="TensorFlow" height="50" /></a>
<a href="https://nodejs.org/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/nodejs-original-wordmark.svg" alt="Node.js" height="50" /></a>
<a href="https://www.mongodb.com/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/mongodb-original-wordmark.svg" alt="MongoDB" height="50" /></a>
<a href="https://expressjs.com/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/express-original-wordmark.svg" alt="Express.js" height="50" /></a>
<a href="https://www.gnu.org/software/bash/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/gnu_bash-icon.svg" alt="Bash" height="50" /></a>
<a href="https://github.com/" target="_blank"><img style="margin: 10px" src="https://profilinator.rishav.dev/skills-assets/git-scm-icon.svg"
alt="Git" height="50" /></a>
</div>

**Blockchain:**
- Solidity, Web3.js, Smart Contracts
- Consensus Mechanisms, Cryptography
- P2P Networking, Distributed Systems

</td></tr></table>

### DevOps & Cloud
<div align="center">
<a href="https://www.linux.org/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/linux-original.svg" alt="Linux" height="50" /></a>
<a href="https://aws.amazon.com/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/amazonwebservices-original-wordmark.svg" alt="AWS" height="50" /></a>
<a href="https://cloud.google.com/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/google_cloud-icon.svg" alt="GCP" height="50" /></a>
<a href="https://azure.microsoft.com/en-in/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/microsoft_azure-icon.svg" alt="Azure" height="50" /></a>
<a href="https://kubernetes.io/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/kubernetes-icon.svg" alt="Kubernetes" height="50" /></a>
<a href="https://www.docker.com/" target="_blank"><img style="margin: 10px"
src="https://profilinator.rishav.dev/skills-assets/docker-original-wordmark.svg" alt="Docker" height="50" /></a>
<a href="https://about.gitlab.com/" target="_blank"><img style="margin: 10px" src="https://profilinator.rishav.dev/skills-assets/gitlab.svg"
alt="GitLab" height="50" /></a>
</div>

<br/>

</p>
</details>

<br/>

## Connect with me
<div align="center">
<a href="https://github.com/davidtkeane" target="_blank">
<img src=https://img.shields.io/badge/github-%2324292e.svg?&style=for-the-badge&logo=github&logoColor=white alt=github style="margin-bottom:
5px;" />
</a>
<a href="https://tryhackme.com/p/rangersmyth" target="_blank">
<img src=https://img.shields.io/badge/TryHackMe-Top_8%25-red?style=for-the-badge&logo=tryhackme&logoColor=white alt=tryhackme
style="margin-bottom: 5px;" />
</a>
<a href="https://www.linkedin.com/in/davidtkeane" target="_blank">
<img src=https://img.shields.io/badge/linkedin-%231E77B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white alt=linkedin
style="margin-bottom: 5px;" />
</a>
<a href="https://twitter.com/davidtkeane" target="_blank">
<img src=https://img.shields.io/badge/twitter-%2300acee.svg?&style=for-the-badge&logo=twitter&logoColor=white alt=twitter
style="margin-bottom: 5px;" />
</a>
<a href="https://stackoverflow.com/users/davidtkeane" target="_blank">
<img src=https://img.shields.io/badge/stackoverflow-%23F28032.svg?&style=for-the-badge&logo=stackoverflow&logoColor=white alt=stackoverflow
style="margin-bottom: 5px;" />
</a>
<a href="https://discord.com/users/davidtkeane" target="_blank">
<img src=https://img.shields.io/badge/Discord-%237289DA.svg?&style=for-the-badge&logo=discord&logoColor=white alt=discord
style="margin-bottom: 5px;" />
</a>
</div>

<br/>

## 📈 Github Stats

<div align="center"><img src="https://github-readme-stats.vercel.app/api?username=davidtkeane&show_icons=true&count_private=true&hide_border=true&theme=dark" align="center" /></div>

<div align="center"><img src="https://streak-stats.demolab.com/?user=davidtkeane&theme=dark&hide_border=true" align="center" /></div>

<br/>

## 📝 Recent Blog Posts

<!-- BLOG-POST-LIST:START -->
- [How to prevent GitHub from suspending your cronjob based triggers](https://dev.to/gautamkrishnar/how-to-prevent-github-from-suspending-your-cronjob-based-triggers-knf)
- [Show your latest dev.to posts automatically on your GitHub profile readme](https://dev.to/gautamkrishnar/show-your-latest-dev-to-posts-automatically-in-your-github-profile-readme-3nk8)
- [God Mode in browsers: document.designMode = &quot;on&quot;](https://dev.to/gautamkrishnar/god-mode-in-browsers-document-designmode-on-2pmo)
- [Skipping the Chrome &quot;Your connection is not private&quot; warning](https://dev.to/gautamkrishnar/quickbits-1-skipping-the-chrome-your-connection-is-not-private-warning-4kp1)
- [Microsoft Student Partners – Geek is the new rockstar](https://dev.to/gautamkrishnar/microsoft-student-partners--geek-is-the-new-rockstar)
<!-- BLOG-POST-LIST:END -->

<br/>

## ⚡ Fun Facts

- 🎯 I use **tabs over spaces** (always!)
- 🎖️ Former combat medic: *"Assess, adapt, protect"* applies to both lives and systems
- 🧠 **7% dyslexic memory** taught me to verify everything (perfect for security!)
- ♟️ Chess, battlefield tactics, and penetration testing use the same strategic thinking
- 🍀 Irish heritage meets Ranger mentality: stubborn problem-solving with a smile

<br/>

---

<div align="center">

### 🎖️ Mission Statement

**"Transform disabilities into superpowers. Build security that works for everyone. Rangers lead the way!"**

*Building RangerOS to prove that the best security understands humans, not just exploits.*

</div>

---

<br/>

<div align="center">
<img src="https://komarev.com/ghpvc/?username=davidtkeane&&style=flat-square" align="center" />
</div>

<br/>

<div align="center">
<a href="https://www.buymeacoffee.com/davidtkeane" target="_blank" style="display: inline-block;">
<img src="https://img.shields.io/badge/Donate-Buy%20Me%20A%20Coffee-orange.svg?style=flat-square&logo=buymeacoffee" align="center" />
</a>
</div>

<br />

----

<div align="center">

**🎖️ Psychology → Cybersecurity → Accessibility → Innovation**

*Rangers lead the way!*

</div>
