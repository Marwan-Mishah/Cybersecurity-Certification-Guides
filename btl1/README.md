# Blue Team Level 1 (BTL1)

> **Last verified:** September 2026  
> **Exam taken:** July 2026  
> **Score:** 95%  
> **Provider:** Centri (formerly Security Blue Team)  
> **Level:** Junior  
> **Focus:** Blue Team / Security Operations / Incident Response  
> **Result:** Passed on first attempt

## Key Takeaways

- Moved from understanding individual security concepts to following structured investigation workflows.
- Practiced SIEM analysis, phishing investigation, threat intelligence, digital forensics, and incident response.
- Strengthened evidence correlation across users, hosts, processes, network activity, and timestamps.
- Built the practical Blue Team foundation that later supported eCIR, eCTHP, and eCDFP.

---

## Overview

Blue Team Level 1, commonly known as BTL1, is a practical defensive cybersecurity certification focused on the skills used by junior security analysts and SOC professionals.

The certification covers six main areas:

- Security Fundamentals
- Phishing Analysis
- Threat Intelligence
- Digital Forensics
- Security Information and Event Management (SIEM)
- Incident Response

What made BTL1 particularly valuable to me was its practical focus.

The training combines theory with browser-based labs, security tools, log analysis, forensic artifacts, network traffic, phishing investigations, threat intelligence, and incident-response scenarios.

The final assessment is also practical rather than a traditional multiple-choice exam.

I completed BTL1 in July 2026 and passed on my first attempt with a score of **95%**.

More importantly, BTL1 changed the way I approached security investigations.

Before it, much of my cybersecurity knowledge could be described as:

```text
Concept
   ↓
Definition
   ↓
Example
```

After BTL1 and my early SOC experience, I increasingly started thinking in terms of:

```text
Alert
   ↓
Evidence
   ↓
Context
   ↓
Correlation
   ↓
Timeline
   ↓
Conclusion
```

That transition was the most valuable outcome of the certification for me.

---

## My Background Before BTL1

I did not start BTL1 completely new to cybersecurity.

Before taking it, I had already completed:

- CompTIA Security+
- Approximately one month of hands-on SOC internship experience at Cyberstone

I started my internship on **June 28, 2026**.

During that early SOC experience, I had already been exposed to:

- SIEM monitoring
- Security alerts
- Log analysis
- Alert triage
- True-positive and false-positive classification
- Investigating suspicious activity
- Following related activity across multiple events
- Working with different types of security logs

However, my practical experience was still limited.

I understood many security concepts individually, but I was still developing the ability to connect multiple pieces of evidence and investigate an incident as a complete sequence of events.

This is where BTL1 became particularly useful.

Security+ had already taught me much of the theory.

My internship was exposing me to real security operations.

BTL1 provided a structured environment where I could practice the investigation skills connecting the two.

---

## Who Is BTL1 For?

BTL1 is primarily aimed at people entering defensive cybersecurity or still early in their careers.

It can be particularly relevant for:

- Cybersecurity students
- Recent graduates
- Junior SOC analysts
- Security analysts
- IT professionals moving into cybersecurity
- Incident response beginners
- Digital forensics beginners
- Threat intelligence beginners

You do not need previous professional SOC experience to start BTL1.

However, knowledge of networking, operating systems, and general security concepts will make the training easier.

For me, Security+ significantly reduced the amount of fundamental theory I needed to learn during BTL1.

---

## Current Exam Information

At the time of writing:

| Item | Details |
|---|---|
| Certification | Blue Team Level 1 |
| Abbreviation | BTL1 |
| Provider | Centri |
| Previous provider name | Security Blue Team |
| Level | Junior |
| Exam type | Practical |
| Delivery | Online |
| Exam environment | Live browser-based lab |
| Maximum exam window | 24 hours |
| Traditional multiple-choice exam | No |
| Included exam attempts | 2 |
| Training access | 4 months / 124 days |
| Included lab time | 100 hours |
| Exam access | 12 months |
| Certification validity | Lifetime digital certificate |

Exam policies and access conditions can change, so I recommend checking Centri's current documentation before purchasing or scheduling the exam.

---

## Security Blue Team Became Centri

Older BTL1 resources may refer to **Security Blue Team**.

The company changed its trading name to **Centri** on June 1, 2026.

The underlying platform, existing certifications, learning progress, and certification records remained valid through the transition.

Because BTL1 has existed for years under the Security Blue Team name, both names still appear in older:

- Guides
- Reviews
- Screenshots
- Community discussions
- Training references

---

## What I Learned

### 1. Security Fundamentals

The Security Fundamentals section establishes the baseline knowledge needed for the more practical parts of BTL1.

It includes areas such as:

- Networking
- Security concepts
- Network devices
- Security controls
- Endpoint security
- Network security
- Email security
- Risk
- Policies and procedures
- Compliance
- Active Directory
- Blue Team roles
- Professional skills

Because I had already completed Security+, much of this material was familiar.

For me, this section mainly reinforced the foundation before moving into hands-on investigations.

The biggest difference between Security+ and BTL1 was not necessarily the concepts themselves.

It was what happened next.

Security+ often helped me understand:

> **What is this technology or security concept?**

BTL1 increasingly required me to ask:

> **How can I use it during an investigation?**

---

### 2. Phishing Analysis

The phishing section taught me a more structured way to investigate suspicious emails.

Instead of simply looking at an email and deciding whether it "looks malicious," I learned to break it into individual artifacts.

These can include:

- Email headers
- Sender information
- Reply-To information
- URLs
- Domains
- IP addresses
- Attachments
- File hashes
- Email artifacts
- Threat-intelligence indicators

#### What I Learned From Phishing Analysis

The main skill I developed was following a repeatable investigation process.

For example:

```text
Suspicious Email
      ↓
Inspect Headers
      ↓
Extract URLs / Domains / IPs
      ↓
Analyze Attachments
      ↓
Check Hashes
      ↓
Enrich Indicators
      ↓
Determine Context
      ↓
Document Findings
```

This taught me not to base a conclusion on a single suspicious characteristic.

Instead, I should collect evidence and determine whether the different artifacts support the same conclusion.

---

### 3. Threat Intelligence

Before BTL1, I understood the general idea of Indicators of Compromise.

BTL1 helped me understand how threat intelligence can support an active investigation.

The training introduced concepts such as:

- Indicators of Compromise
- Threat actors
- Tactical intelligence
- Operational intelligence
- Strategic intelligence
- MITRE ATT&CK
- Cyber Kill Chain
- MISP
- OpenCTI
- Indicator enrichment

#### What I Learned From Threat Intelligence

If an investigation produces an indicator such as:

- IP address
- Domain
- URL
- File hash
- Email address

the indicator by itself may not provide enough context.

Threat intelligence can help answer questions such as:

- Has this IP been associated with malicious activity?
- Has this file hash been observed before?
- Is the domain suspicious or newly registered?
- Is the infrastructure connected to known malicious activity?
- Does the observed behavior map to known attacker techniques?

This helped me understand that threat intelligence is not necessarily a completely separate activity from investigation.

It can be one of the evidence-enrichment stages inside the investigation itself.

---

### 4. Digital Forensics

The Digital Forensics section was especially useful because it introduced investigation techniques beyond normal SIEM monitoring.

BTL1 covers areas related to:

- Disk forensics
- Memory forensics
- Windows artifacts
- Linux artifacts
- Evidence acquisition
- File systems
- File metadata
- Deleted files
- Hashing
- Evidence integrity
- Timeline analysis

#### What I Learned From Digital Forensics

One of the most important things I learned was that **not every investigation can be solved using SIEM logs alone**.

Sometimes the investigation needs to move from centralized telemetry to evidence collected directly from the affected endpoint.

For example:

```text
SIEM Alert
    ↓
Suspicious Endpoint Activity
    ↓
Collect Relevant Evidence
    ↓
Analyze Disk / Memory / Artifacts
    ↓
Reconstruct Activity
```

Forensic artifacts can help answer questions such as:

- What executable was launched?
- When did it run?
- What files were created?
- What programs had previously executed?
- What activity occurred before the alert?
- Was evidence deleted?
- What processes existed in memory?
- How does the endpoint evidence fit into the wider timeline?

This gave me a better understanding of the relationship between SOC investigation and DFIR.

It also became useful later when I moved into the more specialized **eCDFP** certification.

---

### 5. SIEM and Log Analysis

The SIEM section was directly relevant to my SOC internship.

Splunk is one of the main technologies used in BTL1, and the training involves areas such as:

- Log searching
- Filtering
- Event analysis
- Windows Event Logs
- Security monitoring
- Network activity
- Alert investigation
- Event correlation
- Detection
- Timeline reconstruction

#### What I Learned From SIEM Investigation

Because I already had early SOC exposure, the concept of investigating alerts inside a SIEM was not completely new to me.

However, BTL1 strengthened the investigation methodology behind the alert.

One of the most important lessons was:

> **An alert is usually the beginning of an investigation, not the conclusion.**

An alert may lead to questions such as:

- Who generated the activity?
- Which host was involved?
- Which account was involved?
- What happened immediately before the alert?
- What happened afterward?
- Did similar activity appear elsewhere?
- Was there related network communication?
- Were additional accounts or endpoints involved?
- Does another data source support the same finding?

This naturally leads to **correlation**.

Instead of seeing:

```text
Event A

Event B

Event C

Event D
```

I learned to look for:

```text
Event A
   ↓
Event B
   ↓
Event C
   ↓
Event D

= Incident Timeline
```

That way of thinking became particularly important when working with real SOC alerts during my internship.

---

### 6. Incident Response

Incident Response ties many of the previous domains together.

BTL1 introduces areas such as:

- Preparation
- Detection
- Analysis
- Case management
- Containment
- Eradication
- Recovery
- Lessons learned
- Incident documentation
- MITRE ATT&CK mapping

#### What I Learned From Incident Response

BTL1 helped me understand that discovering malicious activity is only one part of incident response.

A simplified lifecycle can look like:

```text
Preparation
    ↓
Detection
    ↓
Analysis
    ↓
Containment
    ↓
Eradication
    ↓
Recovery
    ↓
Lessons Learned
```

The investigation needs to support broader questions such as:

- Which systems are affected?
- How far did the attacker progress?
- Is the attacker still active?
- What needs to be contained?
- What needs to be removed?
- How can normal operations be restored?
- What evidence should be preserved?
- How can similar activity be detected earlier in the future?

This helped connect technical investigation with the wider incident-response process.

---

## Tools and Technologies

BTL1 exposed me to a broad set of defensive-security tools.

Examples include:

#### SIEM and Log Analysis

- Splunk
- Windows Event Viewer
- DeepBlueCLI
- PowerShell

#### Network Analysis

- Wireshark

#### Digital Forensics

- Autopsy
- FTK Imager
- KAPE
- Volatility
- ProcDump
- JumpList Explorer
- PECmd
- Windows forensic utilities
- Scalpel

#### Threat Intelligence

- VirusTotal
- MISP
- OpenCTI
- Domain intelligence services
- MITRE ATT&CK

#### Phishing Analysis

- PhishTool
- URL-analysis tools
- Browser-history tools
- CyberChef

#### Incident Response and Detection

- TheHive
- Sigma

The main value was **not memorizing every tool**.

It was understanding what kind of evidence each category of tool could help me investigate.

For example:

```text
Need centralized logs?
→ SIEM

Need packet-level evidence?
→ Wireshark

Need disk artifacts?
→ Forensic tools

Need memory evidence?
→ Memory-analysis tools

Need context for an IoC?
→ Threat intelligence

Need investigation organization?
→ Case-management tools
```

That distinction became more important to me than simply knowing a long list of tool names.

---

## Training and Labs

The training is self-paced and includes browser-based labs.

At the time of writing, the official package includes:

- 4 months / 124 days of training access
- 100 lab hours
- Two exam attempts
- 12 months of exam access

Because the labs are browser-based, you do not need to build a complete SOC home lab before starting BTL1.

However, I strongly recommend actually using the labs rather than approaching the course as reading material.

The practical sections were considerably more valuable to me than simply reading the theory.

Many concepts became much clearer after I had to:

- Search logs
- Examine artifacts
- Use investigation tools
- Correlate evidence
- Follow timestamps
- Build a timeline
- Reach an evidence-based conclusion

---

## How BTL1 and My SOC Internship Reinforced Each Other

I was completing BTL1 while also gaining early exposure to real SOC operations during my Cyberstone internship.

During the internship, I was seeing:

- Real security alerts
- Real logs
- SIEM dashboards
- Alert classification
- Investigation workflows
- Different log sources
- True-positive and false-positive decisions

BTL1 gave me a structured environment to understand and practice many of the investigation techniques behind those activities.

The two experiences therefore helped me in different ways.

#### My SOC internship gave me:

- Exposure to real operational environments
- Real-world log sources
- Real alerts
- SIEM workflows
- Analyst decision-making
- Operational context

#### BTL1 gave me:

- Structured investigation practice
- Exposure to multiple analysis disciplines
- A repeatable evidence-driven methodology
- More experience correlating different data sources
- A better understanding of timelines
- A clearer connection between SOC analysis and DFIR

I do not consider one a replacement for the other.

The internship showed me how security operations work in a real environment.

BTL1 helped me build the skills behind those operations in a controlled training environment.

---

## My Exam Experience

I completed the BTL1 exam in July 2026.

At that point, I had:

- CompTIA Security+
- Approximately one month of hands-on SOC experience
- Completed the BTL1 training and labs

I passed the exam on my first attempt with a score of **95%**.

The practical nature of the exam was one of the things I liked most about the certification.

Instead of only being asked whether I knew what a security concept meant, I had to investigate activity and work through evidence.

I had to pay attention to areas such as:

- Timestamps
- Indicators of compromise
- Relationships between events
- Different evidence sources
- Sequence of attacker activity
- Context surrounding suspicious behavior

One of the strongest lessons reinforced by the exam was that a single artifact normally does not explain an entire incident.

For example:

```text
Process Execution
       +
Network Connection
       +
User Activity
       +
File Artifact
       +
Threat Intelligence
       +
Timeline
       ↓
Better Understanding of the Incident
```

That investigation mindset is one of the main things I carried forward from BTL1.

---

## What BTL1 Changed in the Way I Investigate

Before this stage of my learning, much of my thinking was:

```text
Concept
→ Definition
→ Example
```

After gaining SOC exposure and completing BTL1, I increasingly approached investigations as:

```text
Alert
   ↓
Evidence
   ↓
Context
   ↓
Correlation
   ↓
Timeline
   ↓
Conclusion
```

Instead of stopping at:

> "This event is suspicious."

I became more interested in asking:

- Why is it suspicious?
- What happened before it?
- What happened afterward?
- Which user generated it?
- Which host was involved?
- Is there related network activity?
- Are there relevant endpoint artifacts?
- Can another data source validate the finding?
- What does the complete timeline suggest?

That transition was one of the most useful outcomes of BTL1 for me.

---

## What I Actually Gained From BTL1

The biggest value of BTL1 was not any individual tool.

It was learning how multiple Blue Team disciplines can connect during the same investigation.

For example:

```text
Phishing Analysis
        ↓
Extract IoCs
        ↓
Threat Intelligence
        ↓
Search SIEM
        ↓
Identify Endpoint Activity
        ↓
Digital Forensics
        ↓
Reconstruct Timeline
        ↓
Incident Response
```

Before BTL1, these topics could appear to be completely separate cybersecurity specialties.

BTL1 helped me understand how they can become different stages or evidence sources within the same investigation.

---

## Skills I Developed

After completing BTL1, I was more comfortable with:

- Approaching alerts as starting points rather than final conclusions
- Investigating activity across multiple evidence sources
- Correlating events by timestamp, user, host, process, and network activity
- Extracting and enriching Indicators of Compromise
- Investigating suspicious emails systematically
- Searching and interpreting security logs
- Building timelines from related events
- Recognizing when SIEM telemetry alone is insufficient
- Using forensic artifacts to support an investigation
- Relating technical findings to the incident-response process
- Mapping suspicious behavior to attacker techniques
- Documenting findings based on evidence rather than assumptions

I would not describe BTL1 alone as making me an expert in SIEM, DFIR, threat intelligence, or incident response.

Its main value was giving me a **practical foundation across all of them** and teaching me how they connect.

---

## How BTL1 Helped With Later Certifications

BTL1 became a major foundation for the three Blue Team certifications I completed later through INE:

- eCIR — Incident Response
- eCTHP — Threat Hunting
- eCDFP — Digital Forensics

BTL1 had already introduced me to the general workflow connecting:

```text
Detection
    ↓
Investigation
    ↓
Evidence
    ↓
Correlation
    ↓
Forensics
    ↓
Response
```

Because of that, when I moved into the more specialized INE certifications, I was not encountering these disciplines for the first time.

Instead, I could focus on going deeper into each area.

For me, the progression looked approximately like:

```text
Security+
Broad Cybersecurity Foundation
        ↓
BTL1
Practical Blue Team Foundation
        ↓
SOC Internship Experience
        ↓
eCIR
Incident Response
        ↓
eCTHP
Threat Hunting
        ↓
eCDFP
Digital Forensics
```

BTL1 was therefore one of the most important foundations in my early Blue Team learning path.

---

## Important Things to Know Before Starting

### BTL1 Is Broader Than SIEM

SIEM investigation is important, but the certification also covers:

- Phishing
- Threat intelligence
- Network traffic
- Endpoint evidence
- Disk artifacts
- Memory artifacts
- Incident response
- Case management

---

### The Labs Matter

Reading the course alone does not provide the same experience as actually completing investigations.

The labs are where many of the concepts begin connecting.

---

### You Do Not Need Years of Experience

I personally had only around one month of SOC internship experience when I completed BTL1.

That experience helped because alerts, logs, and SIEM workflows were already familiar to me, but I was still very early in my Blue Team development.

---

### Knowing Tools Is Not the Same as Knowing How to Investigate

Knowing a Splunk command or Wireshark filter is useful.

But an investigation requires knowing **why** you are using it.

I found these questions more important:

```text
What am I trying to determine?

What evidence would support it?

What happened before this event?

What happened afterward?

Can I validate this using another source?

Does the evidence support my conclusion?
```

That investigation process is more transferable than memorizing individual tool commands.

---

## Frequently Asked Questions

#### Is BTL1 a beginner certification?

Yes.

It is designed for people early in their defensive-security careers.

#### Is BTL1 theoretical or practical?

Both, but it has a strong practical focus.

The course includes theory, while the labs and final assessment require hands-on investigation.

#### Is the exam multiple choice?

No.

The current BTL1 final assessment is a practical live-lab exam rather than a traditional multiple-choice test.

#### Can it be taken remotely?

Yes.

The training and exam are online.

#### How long is the exam?

The current maximum exam window is **24 hours**.

That is the available completion window, not a requirement to work continuously for 24 hours.

#### How many attempts are included?

The current package includes **two exam attempts**.

#### How much training access is included?

The current training-access period is **4 months / 124 days**.

#### How many lab hours are included?

The current package includes **100 lab hours**.

#### How long is exam access?

The current exam-access period is **12 months**.

#### Does BTL1 expire?

The provider currently issues BTL1 as a **lifetime digital certification**.

#### Did I have professional SOC experience before BTL1?

I had approximately one month of hands-on SOC internship experience.

I was still very early in my practical Blue Team development.

#### Did I pass on my first attempt?

Yes.

I passed on my first attempt with a score of **95%**.

---

## Exam Confidentiality

The BTL1 assessment is protected by exam-security and confidentiality requirements.

This guide therefore does **not** contain:

- Real exam questions
- Exam answers
- Flags
- Exact investigation scenarios
- Exam screenshots
- Confidential artifacts
- Information that reveals the solution to the assessment

The purpose of this guide is to document the certification, what I learned, and how it contributed to my development without compromising the integrity of the exam.

---

## Final Thoughts

BTL1 was important in my progression from **understanding cybersecurity concepts** to **performing structured security investigations**.

Security+ gave me a broad cybersecurity foundation.

My early SOC internship at Cyberstone exposed me to real security operations.

BTL1 helped connect those two experiences into a more structured investigation methodology.

The most valuable change for me was moving from thinking about isolated alerts to thinking about incidents as connected timelines of evidence.

Instead of stopping at:

> **"This event is suspicious."**

I became more interested in asking:

> **Why did it happen?**  
> **What happened before it?**  
> **What happened afterward?**  
> **Which systems and users were involved?**  
> **What other evidence supports the finding?**  
> **How does everything fit together?**

That investigation mindset was the main skill I took away from BTL1.

The certification also gave me the practical foundation that later helped me move deeper into incident response, threat hunting, and digital forensics through eCIR, eCTHP, and eCDFP.

---

## Official Sources

For current information, verify details directly through:

- [Centri — Blue Team Level 1](https://www.centri.org/certifications/blue-team-level-1)
- [Centri — Certification and Exam Access](https://support.centri.org/hc/en-gb/articles/11520624967836-Certification-and-Exam-Access)
- [Centri — Is BTL1 Right for Me?](https://support.centri.org/hc/en-gb/articles/11316228055836-Is-BTL1-Right-For-Me)
- [Centri — BTL1 Exam NDA](https://www.centri.org/btl1-exam-nda)

Certification pricing, access periods, exam policies, course content, and platform features may change after this guide is published.

---

## Disclaimer

This guide combines my personal experience completing BTL1 with publicly available information from the certification provider.

My score, background, preparation, and exam experience should not be interpreted as a guarantee of another candidate's experience.

This repository does not contain confidential exam material, brain dumps, memorized tasks, or exact exam scenarios.
