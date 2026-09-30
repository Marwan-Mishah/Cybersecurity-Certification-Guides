# Blue Team Level 1 (BTL1)

> Last verified: September 2026  
> Exam taken: July 2026  
> Score: 95%  
> Provider: Centri (formerly Security Blue Team)  
> Level: Junior  
> Focus: Blue Team / Security Operations / Incident Response

## Overview

Blue Team Level 1, commonly known as BTL1, is a practical defensive cybersecurity certification focused on the skills used by junior security analysts and SOC professionals.

The certification covers six main areas:

- Security Fundamentals
- Phishing Analysis
- Threat Intelligence
- Digital Forensics
- Security Information and Event Management (SIEM)
- Incident Response

What makes BTL1 different from many entry-level cybersecurity certifications is its strong practical focus.

The training includes browser-based labs, investigations, security tools, log analysis, forensic artifacts, network traffic, phishing emails, and incident-response scenarios.

The final assessment is also practical rather than a traditional multiple-choice exam.

I completed BTL1 in July 2026 and passed on my first attempt with a score of **95%**.

---

# My Background Before BTL1

I did not start BTL1 completely new to cybersecurity.

Before taking the certification, I had already completed CompTIA Security+ and had approximately one month of hands-on SOC experience from my summer internship at Cyberstone.

During that SOC experience, I had already been exposed to the general workflow of security monitoring and investigation.

This gave me some familiarity with concepts such as:

- SIEM monitoring
- Security alerts
- Log analysis
- Alert triage
- Investigating suspicious activity
- Distinguishing between true positives and false positives
- Following activity across multiple events

However, my practical experience was still limited.

I understood many cybersecurity concepts individually, but I was still developing the ability to connect evidence together and investigate an incident as a complete sequence of events.

This is where BTL1 became particularly useful for me.

---

# Who Is BTL1 For?

BTL1 is designed primarily for people who are entering defensive cybersecurity or are still early in their careers.

It can be particularly relevant for:

- Cybersecurity students
- Recent graduates
- Junior SOC analysts
- Security analysts
- IT professionals moving into cybersecurity
- Incident response beginners
- Digital forensics beginners
- Threat intelligence beginners
- Career changers entering defensive security

The provider currently recommends approximately **0–2 years of experience**.

That means BTL1 does not assume that the candidate is already an experienced analyst.

At the same time, having some knowledge of networking, operating systems, and general security concepts will make the training easier to understand.

---

# Prerequisite Knowledge

There are no strict professional-experience requirements for BTL1.

The training introduces many of the fundamentals needed for the certification.

However, I would consider the following knowledge useful before starting:

- Basic networking
- TCP/IP
- IP addresses and ports
- Common network protocols
- Windows fundamentals
- Basic Linux usage
- Cybersecurity terminology
- Common types of attacks
- Basic log concepts
- Basic incident response concepts

Someone who has already studied a foundational certification such as Security+ will recognize many of the concepts in the Security Fundamentals section.

The main difference is that BTL1 starts moving those concepts into practical investigations.

---

# Current Exam Information

| Item | Details |
|---|---|
| Certification | Blue Team Level 1 |
| Abbreviation | BTL1 |
| Provider | Centri |
| Previous provider name | Security Blue Team |
| Level | Junior |
| Recommended experience | 0–2 years |
| Exam type | Practical |
| Delivery | Online |
| Exam environment | Live browser-based lab |
| Maximum exam duration | 24 hours |
| Traditional multiple-choice exam | No |
| Included exam attempts | 2 |
| Training access | 4 months / 124 days |
| Included lab time | 100 hours |
| Exam access | 12 months |
| Current listed price | £399 GBP |
| Certificate validity | Lifetime |

The current BTL1 package includes the training, labs, and certification exam.

Candidates receive two exam attempts.

If the first attempt is unsuccessful, Centri currently requires a 10-day cooldown before the second attempt.

A third attempt may be available for purchase subject to Centri's current policy.

---

# Security Blue Team Became Centri

When people search for BTL1, they may still find many older resources referring to **Security Blue Team**.

Security Blue Team changed its trading name to **Centri** on 1 June 2026.

It is the same company and the BTL1 certification itself did not change because of the rebrand.

Older certificates issued under Security Blue Team remain valid.

Since I took BTL1 after the transition period began, both names may still appear in older guides, screenshots, community discussions, and training material.

---

# Course Structure

BTL1 currently covers six core technical domains.

## 1. Security Fundamentals

This section establishes the foundation needed for the rest of the course.

Topics include areas such as:

- Security concepts
- Networking
- OSI model
- Network devices
- Security controls
- Endpoint security
- Network security
- Email security
- Risk
- Policies and procedures
- Compliance
- Active Directory
- Blue-team roles
- Professional skills

For someone who already has a general certification such as Security+, much of this section may feel familiar.

For me, this part acted mainly as a foundation before moving into the practical investigation domains.

---

# 2. Phishing Analysis

The phishing section teaches a structured way to investigate suspicious emails.

This goes beyond simply looking at an email and deciding whether it "looks suspicious."

You learn to inspect evidence associated with the message.

Important areas include:

- Email headers
- Sender information
- Reply-to information
- URLs
- Domains
- IP addresses
- Attachments
- File hashes
- Email artifacts
- Threat intelligence
- Reporting
- Defensive actions

## What I Learned From Phishing Analysis

One of the main things I gained was a more systematic investigation process.

Instead of immediately deciding whether an email is malicious, I learned to break it down into artifacts and analyze each one.

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

This is much closer to how phishing investigations should be handled in a SOC environment.

---

# 3. Threat Intelligence

Threat Intelligence teaches how external and internal intelligence can provide additional context during investigations.

The training introduces areas such as:

- Threat actors
- Indicators of Compromise
- Tactical intelligence
- Operational intelligence
- Strategic intelligence
- MITRE ATT&CK
- Cyber Kill Chain
- MISP
- OpenCTI
- Indicator enrichment

## What I Learned From Threat Intelligence

Before BTL1, I understood the general idea of an Indicator of Compromise.

BTL1 helped me understand how IoCs can actually be used during an investigation.

For example, if an investigation reveals:

```text
Suspicious IP
Domain
URL
File Hash
Email Address
```

those indicators can be enriched using threat intelligence sources.

This can help answer questions such as:

```text
Has this IP been associated with malicious activity?

Has this file hash been seen before?

Is this domain recently registered?

Is this infrastructure associated with a known threat actor?

Does this behavior map to known attacker techniques?
```

Threat intelligence is therefore not necessarily a separate activity from investigation.

It can be part of the investigation process itself.

---

# 4. Digital Forensics

The Digital Forensics section was particularly useful because it introduced investigation techniques that go beyond normal SIEM monitoring.

BTL1 covers areas such as:

- Disk forensics
- Memory forensics
# Blue Team Level 1 (BTL1)

> Last verified: September 2026  
> Exam taken: July 2026  
> Score: 95%  
> Provider: Centri (formerly Security Blue Team)  
> Level: Junior  
> Focus: Blue Team / Security Operations / Incident Response

## Overview

Blue Team Level 1, commonly known as BTL1, is a practical defensive cybersecurity certification focused on the skills used by junior security analysts and SOC professionals.

The certification covers six main areas:

- Security Fundamentals
- Phishing Analysis
- Threat Intelligence
- Digital Forensics
- Security Information and Event Management (SIEM)
- Incident Response

What makes BTL1 different from many entry-level cybersecurity certifications is its strong practical focus.

The training includes browser-based labs, investigations, security tools, log analysis, forensic artifacts, network traffic, phishing emails, and incident-response scenarios.

The final assessment is also practical rather than a traditional multiple-choice exam.

I completed BTL1 in July 2026 and passed on my first attempt with a score of **95%**.

---

# My Background Before BTL1

I did not start BTL1 completely new to cybersecurity.

Before taking the certification, I had already completed CompTIA Security+ and had approximately one month of hands-on SOC experience from my summer internship at Cyberstone.

During that SOC experience, I had already been exposed to the general workflow of security monitoring and investigation.

This gave me some familiarity with concepts such as:

- SIEM monitoring
- Security alerts
- Log analysis
- Alert triage
- Investigating suspicious activity
- Distinguishing between true positives and false positives
- Following activity across multiple events

However, my practical experience was still limited.

I understood many cybersecurity concepts individually, but I was still developing the ability to connect evidence together and investigate an incident as a complete sequence of events.

This is where BTL1 became particularly useful for me.

---

# Who Is BTL1 For?

BTL1 is designed primarily for people who are entering defensive cybersecurity or are still early in their careers.

It can be particularly relevant for:

- Cybersecurity students
- Recent graduates
- Junior SOC analysts
- Security analysts
- IT professionals moving into cybersecurity
- Incident response beginners
- Digital forensics beginners
- Threat intelligence beginners
- Career changers entering defensive security

The provider currently recommends approximately **0–2 years of experience**.

That means BTL1 does not assume that the candidate is already an experienced analyst.

At the same time, having some knowledge of networking, operating systems, and general security concepts will make the training easier to understand.

---

# Prerequisite Knowledge

There are no strict professional-experience requirements for BTL1.

The training introduces many of the fundamentals needed for the certification.

However, I would consider the following knowledge useful before starting:

- Basic networking
- TCP/IP
- IP addresses and ports
- Common network protocols
- Windows fundamentals
- Basic Linux usage
- Cybersecurity terminology
- Common types of attacks
- Basic log concepts
- Basic incident response concepts

Someone who has already studied a foundational certification such as Security+ will recognize many of the concepts in the Security Fundamentals section.

The main difference is that BTL1 starts moving those concepts into practical investigations.

---

# Current Exam Information

| Item | Details |
|---|---|
| Certification | Blue Team Level 1 |
| Abbreviation | BTL1 |
| Provider | Centri |
| Previous provider name | Security Blue Team |
| Level | Junior |
| Recommended experience | 0–2 years |
| Exam type | Practical |
| Delivery | Online |
| Exam environment | Live browser-based lab |
| Maximum exam duration | 24 hours |
| Traditional multiple-choice exam | No |
| Included exam attempts | 2 |
| Training access | 4 months / 124 days |
| Included lab time | 100 hours |
| Exam access | 12 months |
| Current listed price | £399 GBP |
| Certificate validity | Lifetime |

The current BTL1 package includes the training, labs, and certification exam.

Candidates receive two exam attempts.

If the first attempt is unsuccessful, Centri currently requires a 10-day cooldown before the second attempt.

A third attempt may be available for purchase subject to Centri's current policy.

---

# Security Blue Team Became Centri

When people search for BTL1, they may still find many older resources referring to **Security Blue Team**.

Security Blue Team changed its trading name to **Centri** on 1 June 2026.

It is the same company and the BTL1 certification itself did not change because of the rebrand.

Older certificates issued under Security Blue Team remain valid.

Since I took BTL1 after the transition period began, both names may still appear in older guides, screenshots, community discussions, and training material.

---

# Course Structure

BTL1 currently covers six core technical domains.

## 1. Security Fundamentals

This section establishes the foundation needed for the rest of the course.

Topics include areas such as:

- Security concepts
- Networking
- OSI model
- Network devices
- Security controls
- Endpoint security
- Network security
- Email security
- Risk
- Policies and procedures
- Compliance
- Active Directory
- Blue-team roles
- Professional skills

For someone who already has a general certification such as Security+, much of this section may feel familiar.

For me, this part acted mainly as a foundation before moving into the practical investigation domains.

---

# 2. Phishing Analysis

The phishing section teaches a structured way to investigate suspicious emails.

This goes beyond simply looking at an email and deciding whether it "looks suspicious."

You learn to inspect evidence associated with the message.

Important areas include:

- Email headers
- Sender information
- Reply-to information
- URLs
- Domains
- IP addresses
- Attachments
- File hashes
- Email artifacts
- Threat intelligence
- Reporting
- Defensive actions

## What I Learned From Phishing Analysis

One of the main things I gained was a more systematic investigation process.

Instead of immediately deciding whether an email is malicious, I learned to break it down into artifacts and analyze each one.

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

This is much closer to how phishing investigations should be handled in a SOC environment.

---

# 3. Threat Intelligence

Threat Intelligence teaches how external and internal intelligence can provide additional context during investigations.

The training introduces areas such as:

- Threat actors
- Indicators of Compromise
- Tactical intelligence
- Operational intelligence
- Strategic intelligence
- MITRE ATT&CK
- Cyber Kill Chain
- MISP
- OpenCTI
- Indicator enrichment

## What I Learned From Threat Intelligence

Before BTL1, I understood the general idea of an Indicator of Compromise.

BTL1 helped me understand how IoCs can actually be used during an investigation.

For example, if an investigation reveals:

```text
Suspicious IP
Domain
URL
File Hash
Email Address
```

those indicators can be enriched using threat intelligence sources.

This can help answer questions such as:

```text
Has this IP been associated with malicious activity?

Has this file hash been seen before?

Is this domain recently registered?

Is this infrastructure associated with a known threat actor?

Does this behavior map to known attacker techniques?
```

Threat intelligence is therefore not necessarily a separate activity from investigation.

It can be part of the investigation process itself.

---

# 4. Digital Forensics

The Digital Forensics section was particularly useful because it introduced investigation techniques that go beyond normal SIEM monitoring.

BTL1 covers areas such as:

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

The course introduces several forensic tools used to examine these artifacts.

## What I Learned From Digital Forensics

This section helped me understand that not every security investigation can be solved using SIEM logs alone.

Sometimes you need to examine evidence directly from the affected system.

For example:

```text
SIEM Alert
    ↓
Suspicious Endpoint Activity
    ↓
Collect Evidence
    ↓
Analyze Disk / Memory / Artifacts
    ↓
Reconstruct Activity
```

I learned how forensic artifacts can help answer questions such as:

- What executable was launched?
- When did it run?
- What files were created?
- What programs were previously executed?
- What activity occurred before the alert?
- Was evidence deleted?
- What processes existed in memory?

This gave me a better understanding of the relationship between SOC investigation and DFIR.

---

# 5. Security Information and Event Management (SIEM)

The SIEM section focuses on using centralized logs to investigate suspicious activity.

Splunk is one of the main technologies used in the BTL1 training.

The section involves areas such as:

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

## What I Learned From SIEM Investigation

Because I already had approximately one month of SOC experience before taking BTL1, the idea of investigating alerts inside a SIEM was not completely new to me.

However, BTL1 helped strengthen the investigation process behind the alert.

One important lesson was:

> An alert is usually the beginning of an investigation, not the conclusion.

An analyst may start with one suspicious event and then investigate:

```text
Who generated the activity?

Which host was involved?

What happened immediately before it?

What happened after it?

Did the same activity appear elsewhere?

Was there network communication?

Did another account or endpoint become involved?
```

This naturally leads to correlation.

Instead of analyzing isolated events:

```text
Event A
Event B
Event C
Event D
```

you try to understand:

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

That way of thinking became especially important to me later when working with real SOC alerts.

---

# 6. Incident Response

Incident Response ties many of the previous domains together.

The course covers areas such as:

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

TheHive is one of the case-management technologies introduced in BTL1.

## What I Learned From Incident Response

BTL1 helped me understand that investigating an alert is only one part of responding to an incident.

A simplified response lifecycle can look like:

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

The analyst needs to understand not only **what happened**, but also:

- What systems are affected?
- How far did the attacker get?
- Is the attacker still active?
- What needs to be contained?
- What needs to be removed?
- How can normal operations be restored?
- How can similar incidents be detected earlier in the future?

This helped connect technical investigation with the larger incident-response process.

---

# Tools and Technologies

BTL1 exposes students to a broad set of defensive-security tools.

Some of the tools currently associated with the curriculum include:

### SIEM and Log Analysis

- Splunk
- Event Viewer
- DeepBlueCLI
- PowerShell

### Network Analysis

- Wireshark

### Digital Forensics

- Autopsy
- FTK Imager
- KAPE
- Volatility
- ProcDump
- JumpList Explorer
- PECmd
- Windows File Analyzer
- Scalpel

### Threat Intelligence

- VirusTotal
- MISP
- OpenCTI
- DomainTools
- MITRE ATT&CK

### Phishing Analysis

- PhishTool
- URL2PNG
- Browser History Viewer
- Browser History Capturer
- CyberChef

### Incident Response and Detection

- TheHive
- Sigma

The important part of BTL1, in my opinion, was not memorizing each individual tool.

It was understanding **why and when a certain category of tool is useful during an investigation**.

For example:

```text
Need centralized logs?
→ SIEM

Need packet-level evidence?
→ Wireshark

Need disk artifacts?
→ Forensic tools

Need memory evidence?
→ Volatility

Need context for an IoC?
→ Threat intelligence

Need case organization?
→ TheHive
```

---

# Training and Labs

The training is self-paced and includes browser-based labs.

At the time of writing, the official package includes:

- 4 months of course access
- 100 hours of lab access
- Two exam attempts
- 12 months of exam access

Because the labs are browser-based, you do not need to build a complete SOC environment on your own to complete the certification.

This makes BTL1 relatively accessible for students who do not yet have their own security home lab.

The labs are important because BTL1 is not intended to be completed purely through reading.

Many of the concepts become much clearer when you actually investigate the artifacts and use the tools.

---

# My Experience With the Training

I found the practical parts considerably more valuable than simply reading the theoretical material.

At the time, I was already gaining exposure to real SOC workflows during my Cyberstone summer internship.

That created an interesting relationship between the internship and the certification.

During the internship, I was seeing:

```text
Real alerts
Real logs
SIEM dashboards
Alert classification
SOC workflows
```

BTL1 gave me a structured environment to understand the investigation techniques behind those activities.

So instead of seeing BTL1 as completely separate from my SOC experience, the two reinforced each other.

---

# The BTL1 Exam

The BTL1 exam is not a traditional certification test based primarily on multiple-choice questions.

It is a practical security investigation performed inside a live lab environment.

Candidates currently receive up to **24 hours** after starting the exam.

The purpose is to investigate realistic security incidents and demonstrate the ability to work with evidence rather than simply recall definitions.

The provider includes two exam attempts.

---

# My Exam Experience

I completed the BTL1 exam in **July 2026**.

At that point, I had:

- CompTIA Security+
- Approximately one month of hands-on SOC experience
- BTL1 training and labs

I passed the exam on my **first attempt with a score of 95%**.

The practical nature of the exam was one of the things I liked most about the certification.

Instead of being asked only whether I knew what a certain security concept meant, I had to actually investigate activity and work through evidence.

I had to pay close attention to areas such as:

- Timestamps
- Indicators of compromise
- Relationships between events
- Different evidence sources
- Sequence of attacker activity
- Context surrounding suspicious behavior

One of the strongest lessons reinforced by the exam was that a single artifact does not normally explain an entire incident.

For example:

```text
Suspicious Process
```

by itself may not tell you enough.

You may need:

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
      =
Better Understanding of the Incident
```

That mindset is one of the main things I carried forward from BTL1.

---

# What BTL1 Added to My SOC Experience

My internship and BTL1 helped me in different ways.

The SOC internship gave me exposure to real operational environments.

BTL1 gave me a structured environment for developing the skills behind those operations.

Before this period, much of my cybersecurity knowledge could be described as:

```text
Concept
→ Definition
→ Example
```

After gaining SOC exposure and completing BTL1, I started thinking more like:

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

That transition was one of the most useful outcomes for me.

---

# What I Actually Gained From BTL1

The biggest value was not any single tool.

It was learning how the different blue-team disciplines connect.

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
Reconstruct Incident
        ↓
Incident Response
```

Before BTL1, these topics can look like completely separate cybersecurity specialties.

The certification helped me understand how they can become different stages of the same investigation.

---

# Exam-Day Workflow

The exact interface and policies may change, but the general process is:

```text
Access Certification Platform
        ↓
Start Exam
        ↓
Access Practical Lab
        ↓
Investigate Scenario
        ↓
Analyze Evidence
        ↓
Answer Required Tasks
        ↓
Submit Exam
        ↓
Receive Result
```

Because the exam clock begins once the assessment is started, it is important to begin when you have enough uninterrupted time available.

The current maximum exam period is 24 hours.

This does not mean you are expected to actively work for 24 continuous hours.

It is the maximum window available to complete and submit the assessment.

---

# Exam Attempts and Retakes

The current BTL1 package includes:

```text
Attempt 1
   ↓
If unsuccessful
   ↓
10-day cooldown
   ↓
Attempt 2
```

Both included attempts must fit within the 12-month exam-access period.

Under the current policy, a third and final attempt may be purchased for an additional fee and can be subject to approval.

Because these policies may change, candidates should always check the current Centri exam-access policy before scheduling.

---

# Certification Validity

BTL1 currently provides a lifetime certification.

It does not currently use the recurring renewal model seen with some other certification providers.

Certified candidates also receive digital certification credentials.

The provider currently lists digital rewards including a certificate and Credly badge.

---

# Important Things to Know Before Starting

## BTL1 Is Not Just a SIEM Certification

Although SIEM investigation is a major component, BTL1 covers a much broader defensive-security workflow.

You will encounter:

- Email investigations
- Threat intelligence
- Network traffic
- Endpoint artifacts
- Disk evidence
- Memory evidence
- Incident response
- Case management

---

## The Labs Matter

Reading the course alone does not provide the same experience as actually completing investigations.

The practical labs are where many of the concepts start connecting together.

---

## You Do Not Need Years of SOC Experience

BTL1 is intentionally aimed at junior learners.

I personally had only around one month of SOC experience when I completed it.

That experience helped because I was already familiar with alerts and SIEM workflows, but I was still early in my blue-team learning.

---

## Knowing a Tool Is Not the Same as Knowing How to Investigate

It is possible to learn individual Splunk commands or Wireshark filters without understanding how to conduct an investigation.

BTL1 is more useful when you focus on questions such as:

```text
What am I trying to prove?

What evidence do I need?

What happened before this?

What happened afterward?

Can I validate this finding using another data source?
```

---

# Frequently Asked Questions

## Is BTL1 a beginner certification?

Yes.

The certification is positioned at the junior level and currently recommends approximately 0–2 years of experience.

---

## Is BTL1 theoretical or practical?

Both the training and final assessment have a strong practical focus.

The certification includes theoretical lessons, but the labs and exam require hands-on investigation.

---

## Is the BTL1 exam multiple choice?

The current final exam is a practical assessment rather than a traditional multiple-choice exam.

---

## Can I take BTL1 from home?

Yes.

The training and exam are delivered online.

The practical environment is accessed remotely.

---

## How long is the exam?

The current maximum exam window is 24 hours.

---

## Do I really need 24 hours?

Not necessarily.

Twenty-four hours is the available exam window, not a required completion time.

---

## How many attempts do I get?

The current BTL1 package includes two attempts.

---

## How long do I have to take the exam?

The current exam-access period is 12 months.

---

## How long do I have access to the training?

The current course and lab access period is four months, or 124 days.

---

## How many lab hours are included?

The current package includes 100 lab hours.

---

## Does BTL1 expire?

The certification is currently issued as a lifetime certification.

---

## Do I need professional SOC experience before taking BTL1?

No.

BTL1 is intended for junior learners.

Some prior knowledge can help, but professional SOC experience is not required.

---

## Is Security Blue Team the same as Centri?

Yes.

Security Blue Team changed its trading name to Centri in June 2026.

The underlying company and existing certifications remained unchanged.

---

# Exam Confidentiality

The BTL1 exam is protected by a Non-Disclosure Agreement.

This guide therefore does **not** contain:

- Real exam questions
- Exam answers
- Flags
- Exact investigation scenarios
- Screenshots from the certification exam
- Confidential exam artifacts
- Information that would reveal the exam solution

The purpose of this guide is to explain the certification, the skills involved, and my experience without compromising the integrity of the assessment.

---

# Final Thoughts

BTL1 was important in my progression from learning cybersecurity concepts to performing structured security investigations.

Security+ gave me a broad cybersecurity foundation.

My early SOC experience at Cyberstone gave me exposure to real security operations.

BTL1 then helped connect many of those concepts and experiences into a more structured blue-team investigation methodology.

The most valuable change for me was moving from thinking about isolated alerts to thinking about incidents as connected timelines of evidence.

Instead of stopping at:

```text
"This event is suspicious."
```

I became more interested in asking:

```text
Why did it happen?

What happened before it?

What happened afterward?

Which systems were involved?

What other evidence supports the finding?

How does everything fit together?
```

That investigation mindset is the main skill I took away from BTL1.

---

# Official Sources

For the most current information, verify details directly from:

- Centri — Blue Team Level 1 certification page
- Centri — Certification and Exam Access policy
- Centri — Is BTL1 Right For Me?
- Centri — BTL1 Exam NDA
- Centri — Security Blue Team to Centri rebrand FAQ

Certification prices, access periods, exam policies, course content, and platform features may change after this guide is published.

---

## Disclaimer

This guide is based on my personal experience completing BTL1 together with publicly available information from the certification provider.
