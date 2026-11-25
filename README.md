# Awesome-Reverse-Engineering-Binary-Analysis
# Awesome-Reverse-Engineering-Binary-Analysis

# Awesome Reverse Engineering & Binary Analysis

> A curated list of top Reverse Engineering and Binary Analysis platforms — both SaaS/Hosted commercial solutions and open-source alternatives for disassembly, decompilation, and malware analysis.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [IDA Pro Cloud](#ida-pro-cloud)
  - [Binary Ninja Cloud](#binary-ninja-cloud)
  - [JEB Decompiler](#jeb-decompiler)
  - [RevEng.AI](#revengai)
  - [Binarly](#binarly)
  - [VMRay Analyzer](#vmray-analyzer)
  - [Intezer Analyze](#intezer-analyze)
  - [ReversingLabs Spectra Analyze](#reversinglabs-spectra-analyze)
- [Open-Source Software](#-open-source-software)
  - [Ghidra](#ghidra)
  - [Cutter](#cutter)
  - [OGhidra](#oghidra)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Reverse Engineering and Binary Analysis platforms. These are not open-source but are included as reference points for feature comparison.

### IDA Pro Cloud
**Type:** Industry-standard disassembler and decompiler with cloud licensing
IDA Pro is the long-standing commercial standard for reverse engineering, offering the most mature decompiler and the broadest architecture support in the industry. The **Cloud** editions provide access to decompilers hosted by Hex-Rays, with IDA Pro Essential starting at **€1,099/year** for 2 cloud-based decompilers, while IDA Free offers a zero-cost entry point limited to x86 32/64-bit [citation:2]. Key capabilities include 60+ processor families for disassembly, IDAPython scripting, local debugging via GDBServer, and optional malware analysis extensions [citation:2]. **Trade-off:** Cloud decompilers require a subscription and internet access; full local decompilers and automation features are reserved for higher-tier plans.  
**Best for:** Professional reverse engineers and malware analysts needing the most mature decompiler and broadest architecture coverage, accepting the commercial licensing cost.

### Binary Ninja Cloud
**Type:** Browser-based binary analysis with collaboration features
Binary Ninja Cloud is a **free online reverse engineering tool** that runs entirely in the browser, supporting ELF, Mach-O, and PE file formats with full analysis (not just disassembly) [citation:1][citation:13]. It includes **collaboration** capabilities, embeddable interactive graphs, and multiple IL (Intermediate Language) levels [citation:13]. **Critical limitations:** No API access, no third-party plugins, and strict performance limits on binary size and function counts [citation:1]. **Important privacy note:** By using the service, you agree to submit binaries to Vector 35, and the company states the goal is to use the data to improve future products [citation:1].  
**Best for:** Quick, browser-based analysis of small binaries without installing software, accepting the privacy trade-off and feature limitations.

### JEB Decompiler
**Type:** Decompiler with free Community Edition for x86
JEB is a powerful reverse-engineering platform with a **free Community Edition (CE)** that supports Intel x86 32-bit and 64-bit programs, including Windows PE (EXE, DLL, SYS), Linux ELF, Mach-O, and headless firmware [citation:6]. The CE includes decompilation to C-like source code with optimization passes, type libraries, signature libraries, and **full API access** for Python/Java scripting [citation:6]. It is positioned for researchers, students, hobbyists, and nonprofit organizations, while commercial editions support additional architectures and advanced features.  
**Best for:** Students, researchers, and hobbyists needing a free decompiler for x86 binaries with API access, accepting the architecture limitations of the Community Edition.

### RevEng.AI
**Type:** AI-powered binary analysis for reverse engineering and malware analysis
RevEng.AI is a commercial **AI-powered binary analysis platform** designed for reverse engineering and malware analysis [citation:7]. It offers binary analysis, reverse engineering capabilities, and AI copilot features, deployed as a cloud service suitable for SMB, mid-market, and enterprise organizations [citation:7]. The platform is positioned for security teams wanting AI-assisted analysis to accelerate reverse engineering workflows.  
**Best for:** Security teams wanting AI-assisted binary analysis in a managed cloud platform, accepting the commercial subscription model.

### Binarly
**Type:** Binary transparency and vulnerability detection with free Starter Edition
Binarly Transparency Platform provides **post-build binary scanning** for known vulnerabilities (CVE-mapped), dependency vulnerabilities (deep library and transitive flaws), and **SBOM generation** [citation:8]. The **Starter Edition** is a free version with a 30-day trial that includes API access and PDF reporting (summary, detailed, finding) [citation:8]. Supported binary types include firmware, POSIX, applications, cloud containers, and mobile applications.  
**Best for:** Software supply chain security teams needing binary-level vulnerability detection and SBOM generation, with a free Starter Edition for evaluation.

### VMRay Analyzer
**Type:** Hypervisor-based agentless malware sandbox
VMRay Analyzer is an automated malware analysis sandbox using a **hypervisor-based agentless approach**, making it harder for malware to detect the analysis environment [citation:9]. It provides detailed behavioral analysis with visualizations (geolocated C2 domains, process trees), VMRay Threat Identifier (VTI) rules, YARA rule integration, and a REST API for integration [citation:9]. Available as cloud or on-premises, with on-prem offering the ability to use custom gold images. Pricing starts at **$2,700/year** for a single-user Investigator license [citation:9].  
**Best for:** Malware analysts wanting robust sandbox analysis with strong anti-evasion capabilities, accepting the commercial licensing cost.

### Intezer Analyze
**Type:** AI-powered malware analysis with code reuse detection
Intezer Analyze is an all-in-one malware analysis platform that uses **static and dynamic sandbox execution** for code extraction, with a unique focus on **code reuse detection**—identifying related files that share the same code DNA [citation:10]. It classifies malware families and extracts network IOCs, dropped executables, and other artifacts. Integration with Maltego enables visualization of file relationships. A free community account is available for limited usage [citation:10].  
**Best for:** Incident response and SOC teams needing rapid malware classification and code reuse analysis, with a free tier for evaluation.

### ReversingLabs Spectra Analyze
**Type:** Enterprise file analysis and threat hunting
ReversingLabs Spectra Analyze provides **400+ file-format analysis**, a YARA rule engine with retro-hunts, and cloud sandbox dynamic analysis [citation:11]. It is positioned for SOC teams and threat hunters analyzing suspicious files and software supply chain risks. Median buyer pricing is approximately **$61,667/year**, with a range from $31,261 to $220,750 [citation:11].  
**Best for:** Enterprises needing comprehensive file analysis with threat hunting and SBOM capabilities, accepting the significant annual cost.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Reverse Engineering and Binary Analysis tools. The open-source ecosystem is anchored by **Ghidra** as the leading framework, with complementary GUI and AI-assisted tools.

### Ghidra
**Stack:** Java / C++ | **License:** Apache-2.0
Ghidra is a **software reverse engineering (SRE) framework** created and maintained by the **National Security Agency (NSA) Research Directorate**, providing a suite of full-featured, high-end analysis tools for Windows, macOS, and Linux [citation:4]. Key capabilities include:
- **Disassembly, assembly, decompilation, graphing, and scripting** along with hundreds of other features 
- **Wide processor support**: A broad variety of instruction sets and executable formats 
- **User-interactive and automated modes**: Can be run headless for automation 
- **Extensibility**: Users can develop custom plugins and scripts in Java or Python 
- **Ghidra Server**: Included in the standard distribution (no extra license), enabling **shared projects** with versioning, multi-client access, and collaboration (read-only, read/write, admin permissions per repository) [citation:3]

**Ghidra Server deployment:** Runs as a Java RMI service on ports TCP/13100 and TCP/13101, requiring JDK 21+ and a small Linux VM (2 CPU, 4GB RAM sufficient for small teams) [citation:3]. It supports local password authentication, PKI client certificates, or JAAS (LDAP/Active Directory) [citation:3]. **Critical security note:** The server hosts live malware samples and must **never be exposed to the Internet**—keep it in an isolated malware analysis lab network [citation:3].  
**Best for:** Professional malware analysts, security researchers, and teams needing a free, NSA-backed, extensible reverse engineering framework with collaboration support.

### Cutter
**Stack:** C++ / Qt / Rizin | **License:** GPL-3.0
Cutter is a **Qt and C++ GUI for the Rizin reverse engineering framework**, designed to make an advanced, customizable, and FOSS reverse-engineering platform while keeping the user experience in mind [citation:5][citation:15]. It is created by reverse engineers for reverse engineers, providing a graphical interface over Rizin's disassembly and analysis capabilities. Cutter is actively maintained and packaged for Fedora (version 2.3.4) [citation:5].  
**Best for:** Reverse engineers wanting a free, open-source graphical interface for Rizin with a focus on usability.

### OGhidra
**Stack:** (Check repository) | **License:** BSD-3-Clause
OGhidra is an **AI-driven binary analysis tool** developed at Lawrence Livermore National Laboratory (LLNL) that uses **locally hosted Agentic AI** to automatically reverse engineer binaries to find malware and vulnerabilities [citation:12]. It is sponsored by the USDOE National Nuclear Security Administration (NNSA) and released as open source under BSD-3-Clause. The tool is positioned for automated binary analysis using local AI agents, avoiding cloud dependencies for sensitive samples.  
**Best for:** Security researchers and analysts wanting AI-assisted binary analysis that runs entirely locally, accepting the research-tool maturity.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Decompiler | Cloud Access | Self-Hosted | Best For |
|----------|---------|-------|------------|--------------|-------------|----------|
| **IDA Pro** | Proprietary | C++ | ✅ (Cloud/Local) | ✅ | (Local) | Industry-standard decompiler |
| **Binary Ninja Cloud** | Proprietary | Cloud | (Check) | ✅ | ❌ | Free browser analysis |
| **JEB CE** | Proprietary (Free CE) | Java | ✅ (x86) | ❌ (Desktop) | ✅ (Desktop) | Free x86 decompiler + API |
| **RevEng.AI** | Proprietary | Cloud | ✅ AI-powered | ✅ | ❌ | AI-assisted binary analysis |
| **Binarly** | Proprietary | Cloud | ❌ (Vuln scan) | ✅ | ❌ | Binary vulnerability + SBOM |
| **VMRay** | Proprietary | Cloud/On-prem | ❌ (Sandbox) | ✅ | (On-prem) | Anti-evasion malware sandbox |
| **Intezer** | Proprietary | Cloud | ❌ (Code reuse) | ✅ | ❌ | Malware classification + DNA |
| **Ghidra** | Apache-2.0 | Java/C++ | ✅ | ❌ | ✅ | Full OSS framework + server |
| **Cutter** | GPL-3.0 | C++/Qt | (Via Rizin) | ❌ | ✅ | GUI for Rizin |
| **OGhidra** | BSD-3-Clause | (Check) | (AI-driven) | ❌ | ✅ | Local AI binary analysis |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Reverse Engineering or Binary Analysis tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The open-source landscape for **reverse engineering** is **anchored by Ghidra** as the only full-featured, NSA-backed framework with decompilation, scripting, and built-in server-based collaboration (Ghidra Server) [citation:3][citation:4]. **Cutter** provides a user-friendly GUI over the Rizin framework for analysts preferring a graphical interface [citation:5]. **OGhidra** represents an emerging category—AI-assisted binary analysis using locally hosted agentic AI, sponsored by the NNSA and released as open source [citation:12]. Commercial platforms like IDA Pro and Binary Ninja remain differentiated by decompiler maturity, architecture breadth, and cloud accessibility, while AI-native tools like RevEng.AI and specialized platforms like Binarly and Intezer address specific layers of the reverse engineering and malware analysis workflow. No single open-source project fully replicates IDA Pro's decompiler quality, but Ghidra covers the core disassembly, decompilation, and collaboration needs comprehensively.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
