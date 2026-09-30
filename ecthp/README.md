# eCTHP — Certified Threat Hunting Professional

> **Last verified:** September 2026  
> **Exam taken:** August 12, 2026  
> **Provider:** INE Security  
> **Level:** Professional  
> **Focus:** Threat Hunting / Blue Team / Behavioral Analysis  
> **Delivery:** Online / Remote  
> **Focused certification-specific preparation:** Approximately 3 days

## Key Takeaways

- Added a proactive threat-hunting mindset to my previous alert-driven SOC and incident-response experience.
- Practiced hypothesis-driven hunting, behavioral analysis, endpoint hunting, network hunting, and MITRE ATT&CK mapping.
- Learned to identify the telemetry required to test a hunting hypothesis before searching the environment.
- Better understood how successful hunts can reveal detection gaps and improve future detections.

---

## Overview

The Certified Threat Hunting Professional, commonly known as eCTHP, is a professional-level defensive cybersecurity certification from INE Security focused on proactive threat hunting.

INE currently describes eCTHP as a professional certification for defensive-security practitioners who want to specialize in proactively identifying threats inside enterprise environments.

The biggest difference between threat hunting and traditional alert-driven investigation is the starting point.

A SOC investigation often begins with:

```text
Alert
  ↓
Investigate
```

Threat hunting may instead begin with:

```text
Hypothesis
    ↓
Identify Required Data
    ↓
Search Environment
    ↓
Look for Suspicious Behavior
    ↓
Validate or Reject Hypothesis
```

That shift from **reactive investigation** to **proactive searching** was the main thing eCTHP added to my Blue Team knowledge.

I completed eCTHP on **August 12, 2026** while I was still completing my SOC internship at Cyberstone.

---

## My Background Before eCTHP

By the time I started eCTHP, I already had:

- CompTIA Security+
- Blue Team Level 1
- eCIR
- Approximately six to seven weeks of SOC internship experience

This background mattered significantly.

I was already familiar with:

- SIEM monitoring
- Alert triage
- Log analysis
- Incident investigation
- Network traffic analysis
- Threat intelligence
- Digital forensics
- MITRE ATT&CK
- Evidence correlation
- Incident timelines

Because of that, eCTHP did not need to teach me how security investigations work from the beginning.

Instead, it introduced a different question:

> **What if no alert exists yet?**

That is where threat hunting became distinct from the incident-response mindset I had developed through BTL1 and eCIR.

---

## My Progression Before eCTHP

My progression looked roughly like:

```text
Security+
    ↓
Understand Cybersecurity Concepts
    ↓
BTL1
    ↓
Learn Structured Blue Team Investigation
    ↓
SOC Internship
    ↓
Work With Real Alerts and Logs
    ↓
eCIR
    ↓
Go Deeper Into Incident Response
    ↓
eCTHP
    ↓
Search Proactively for Threats
```

This sequence made eCTHP much easier for me to understand.

Instead of learning threat hunting as an isolated subject, I could see how it connects to SOC monitoring and incident response.

---

## Incident Response vs. Threat Hunting

This distinction was probably the most important conceptual takeaway for me.

### Incident Response

Incident response often starts because something has already been detected.

For example:

```text
Alert
  ↓
Suspicious Activity
  ↓
Investigation
  ↓
Scope
  ↓
Containment / Response
```

The analyst already has a reason to investigate.

---

### Threat Hunting

Threat hunting can begin without a specific alert.

For example:

```text
Threat Intelligence
        +
Known Attacker Behavior
        +
Environment Knowledge
        ↓
Hypothesis
        ↓
Search Available Telemetry
        ↓
Identify Anomalies
        ↓
Validate Findings
```

The hunter asks:

> **Could this behavior already exist in the environment without having triggered a detection?**

That proactive mindset was the main difference I took from eCTHP.

---

## Hypothesis-Driven Threat Hunting

One of the most useful ideas in threat hunting is starting from a hypothesis.

A hypothesis should describe suspicious behavior that may exist in the environment.

For example:

```text
An attacker may be using PowerShell
for malicious execution on Windows endpoints.
```

From there, the investigation becomes more structured.

---

### Step 1 — Define the Behavior

Instead of searching randomly for:

```text
powershell.exe
```

the real question is:

> **What would suspicious PowerShell activity look like?**

Potential characteristics might include:

- Unusual parent processes
- Encoded commands
- Suspicious command-line arguments
- Network connections
- Downloads
- Unexpected child processes
- Execution by unusual users
- Execution at unusual times

---

### Step 2 — Identify the Required Data

A hunt is only possible if the environment collects the necessary telemetry.

For this example, useful sources might include:

- Process-creation telemetry
- Sysmon
- PowerShell logging
- Windows Event Logs
- Network connections
- DNS logs
- EDR telemetry
- SIEM data

This taught me an important lesson:

> **A good hunting idea is useless if the required telemetry does not exist.**

---

### Step 3 — Search for the Behavior

The hunt could then look for:

```text
powershell.exe
      ↓
Parent Process
      ↓
Command Line
      ↓
User
      ↓
Destination IP / Domain
      ↓
Child Processes
      ↓
Timestamp
```

Instead of only identifying PowerShell execution, the goal is to determine whether the surrounding behavior is suspicious.

---

### Step 4 — Validate the Finding

A suspicious result is not automatically malicious.

It should be compared against:

- User context
- Host role
- Administrative activity
- Normal environment behavior
- Related process activity
- Network connections
- Other security telemetry

This was directly relevant to what I was already learning in my SOC internship:

> **Suspicious does not automatically mean malicious.**

Context matters.

---

## Indicators of Compromise vs. Indicators of Attack

Another useful distinction in threat hunting is between **Indicators of Compromise** and broader behavioral indicators.

### Indicators of Compromise

IoCs may include:

- IP addresses
- Domains
- URLs
- File hashes
- Email addresses

They can be extremely useful, but they often describe artifacts that are already known.

For example:

```text
Known Malicious Hash
        ↓
Search Environment
        ↓
Find Matching File
```

This can be effective, but attackers can change infrastructure or payloads.

---

### Behavioral Indicators

Behavior-based hunting focuses more on **what the attacker is doing**.

For example:

```text
Credential Dumping
        ↓
Suspicious LSASS Access
        ↓
Unexpected Process
        ↓
Correlated Endpoint Activity
```

or:

```text
Persistence
    ↓
Scheduled Task Created
    ↓
Unusual Executable
    ↓
Suspicious User Context
```

This made MITRE ATT&CK particularly useful.

Instead of only searching for known bad artifacts, you can hunt for attacker techniques.

---

## MITRE ATT&CK in Threat Hunting

BTL1 and eCIR had already introduced MITRE ATT&CK to me.

eCTHP helped reinforce how ATT&CK can support hunting.

For example:

```text
Threat Intelligence
        ↓
Known Attacker Technique
        ↓
MITRE ATT&CK
        ↓
Identify Required Telemetry
        ↓
Build Hunting Hypothesis
        ↓
Search Environment
```

Suppose the hypothesis relates to malicious PowerShell usage.

That can be mapped to:

```text
T1059.001 — PowerShell
```

The technique itself does not prove malicious activity.

Instead, it provides a structured way to think about:

- Attacker behavior
- Relevant telemetry
- Detection opportunities
- Hunting queries

---

## Behavioral Analysis

Threat hunting taught me to think less about individual alerts and more about **patterns of behavior**.

For example, these events separately may not be enough:

```text
PowerShell Execution

DNS Query

Outbound Connection

New Scheduled Task
```

But when they occur together:

```text
PowerShell Execution
        ↓
Suspicious DNS Query
        ↓
Outbound Connection
        ↓
Persistence Created
```

the combined behavior becomes much more interesting.

That is similar to correlation in incident response, but the difference is that a hunter may be actively searching for the pattern before an alert exists.

---

## Endpoint Hunting

Endpoint telemetry can provide visibility into:

- Process execution
- Parent-child process relationships
- Command lines
- User activity
- Persistence
- Credential access
- File creation
- Registry modifications
- Scheduled tasks
- Service creation
- Network connections

A useful hunting workflow might be:

```text
Hypothesis
    ↓
Identify Relevant Endpoint Events
    ↓
Search Across Hosts
    ↓
Identify Outliers
    ↓
Inspect Process Tree
    ↓
Correlate User / Network Activity
    ↓
Determine Whether Behavior Is Expected
```

One thing I learned is that process context matters.

For example:

```text
powershell.exe
```

alone tells you very little.

But:

```text
winword.exe
    ↓
powershell.exe
    ↓
External Connection
```

is significantly more interesting.

Again, the exact conclusion depends on context.

---

## Network Hunting

Network telemetry can reveal behaviors that endpoint evidence may not fully explain.

Useful data may include:

- Source and destination IPs
- Ports
- Protocols
- DNS queries
- Connection frequency
- Data volume
- Authentication activity
- External connections
- Beaconing patterns

A network hunt may look like:

```text
Environment Baseline
        ↓
Identify Unusual Communication
        ↓
Determine Source Host
        ↓
Identify Destination
        ↓
Analyze Frequency / Protocol
        ↓
Correlate With Endpoint Evidence
```

For me, the most valuable part was again **correlation**.

A suspicious network connection becomes much more meaningful when I can determine:

- Which endpoint generated it
- Which user was active
- Which process initiated it
- What happened immediately before it

---

## Baselines and Anomalies

Threat hunting often depends on understanding what is normal.

Without a baseline, it is difficult to know whether something is unusual.

For example:

```text
User logs in at 2 AM
```

may appear suspicious.

But:

- Is that user's job shift overnight?
- Is the system a server accessed automatically?
- Is the authentication coming from a known administrative system?

The activity only becomes meaningful when compared with expected behavior.

A useful way to think about it is:

```text
Observed Activity
        ↓
Compare With Baseline
        ↓
Expected?
   ↙         ↘
 Yes         No
  ↓           ↓
Move On   Investigate Further
```

This is one of the reasons threat hunting requires environment knowledge in addition to technical knowledge.

---

## Threat Intelligence in Hunting

Threat intelligence can provide the initial direction for a hunt.

For example:

```text
Threat Intelligence Report
        ↓
Attacker Uses Technique X
        ↓
Could Technique X Exist Here?
        ↓
Identify Relevant Telemetry
        ↓
Build Hunt
```

This is different from simply searching for a known malicious IP or hash.

Threat intelligence can also describe:

- Tactics
- Techniques
- Procedures
- Malware behavior
- Common persistence mechanisms
- Credential-access methods
- Command-and-control techniques

These behavioral details can be converted into hunting ideas.

---

## From Hunt to Detection

One of the most useful relationships I learned is that successful threat hunts can improve future detection.

For example:

```text
Hunting Hypothesis
       ↓
Search Environment
       ↓
Find Suspicious Pattern
       ↓
Validate Behavior
       ↓
Understand Detectable Characteristics
       ↓
Create / Improve Detection
```

This means threat hunting does not only discover existing threats.

It can also identify **detection gaps**.

That connection is particularly relevant to SOC and detection-engineering work.

---

## My SOC Internship and Threat Hunting

My Cyberstone internship complemented eCTHP because I was already working with SIEM platforms and different log sources.

During the internship, I worked with telemetry from areas such as:

- Firewalls
- Endpoints
- Cloud platforms
- Database audit logs
- SaaS platforms
- Web-security systems

Most of my work was alert-driven investigation and triage.

However, I also gained experience searching through telemetry and investigating activity beyond a single alert.

eCTHP helped me understand that similar searching can be performed proactively.

Instead of:

```text
Alert Exists
    ↓
Search Logs
```

the process can become:

```text
Suspicious Behavior Hypothesis
            ↓
Search Logs
            ↓
Determine Whether Behavior Exists
```

That was an important change in perspective for me.

---

## How I Prepared

My focused preparation for eCTHP was approximately **three days**.

Like my other INE certifications, most of my preparation came from:

- INE learning material
- INE labs
- Hands-on use of the tools
- Previous Blue Team knowledge

By this point I already had:

- Security+
- BTL1
- eCIR
- Several weeks of SOC experience

So the three days should not be interpreted as the amount of time required to learn threat hunting from zero.

A more accurate representation is:

```text
Security+
    ↓
BTL1
    ↓
SOC Experience
    ↓
eCIR
    ↓
3 Days of Focused eCTHP Preparation
    ↓
Exam
```

The short certification-specific preparation period was possible because a large part of the underlying Blue Team foundation already existed.

---

## Why BTL1 Helped

BTL1 had already taught me:

- SIEM investigation
- Threat intelligence
- Log analysis
- Network analysis
- Endpoint evidence
- MITRE ATT&CK
- Evidence correlation

That meant eCTHP could focus more on changing **how those tools and data sources are used**.

For example:

```text
BTL1
Alert → Evidence → Investigation

eCTHP
Hypothesis → Evidence Search → Hunt
```

The same telemetry may be involved.

The mindset is different.

---

## Why eCIR Helped

eCIR immediately preceded eCTHP in my learning path.

eCIR strengthened my ability to:

- Investigate incidents
- Analyze endpoint evidence
- Analyze network evidence
- Correlate events
- Reconstruct attack activity

eCTHP then changed the starting point.

Instead of asking:

> **What happened in this incident?**

I started thinking more about:

> **What attacker behavior could exist here without having generated an alert yet?**

That made the progression from eCIR to eCTHP feel very natural.

---

## My Most Important Preparation Advice: Use the Tools

As with eCIR, my strongest recommendation is to use the tools yourself.

Do not only watch:

```text
Instructor
   ↓
Open Tool
   ↓
Run Query
   ↓
Find Result
```

Practice doing it yourself:

```text
Question
   ↓
Choose Data Source
   ↓
Open Tool
   ↓
Create Search / Filter
   ↓
Review Results
   ↓
Pivot
   ↓
Correlate Evidence
```

Threat hunting involves exploration.

If basic tool navigation consumes too much attention, it becomes harder to focus on the behavior you are hunting.

---

## Do Not Hunt Randomly

Threat hunting is not simply searching through logs until something looks strange.

A better approach is:

```text
Hypothesis
    ↓
Required Data
    ↓
Search Strategy
    ↓
Results
    ↓
Analysis
    ↓
Conclusion
```

For example:

```text
Hypothesis:
Attackers may be using scheduled tasks for persistence.

        ↓

Required Data:
Scheduled-task creation telemetry

        ↓

Search:
Look for task creation across endpoints

        ↓

Analysis:
User
Command
Executable
Parent process
Timestamp
Frequency

        ↓

Conclusion:
Expected administration or suspicious persistence?
```

This structure keeps the hunt focused and reproducible.

---

## My Exam Experience

I completed eCTHP remotely on **August 12, 2026**.

Like the other INE exams I completed during this period, the assessment required me to use technical tools and work with information from the provided environment.

My previous BTL1, eCIR, and SOC experience significantly reduced the learning curve.

The exam reinforced that understanding the methodology alone is not enough.

You also need to be comfortable:

- Navigating tools
- Searching available data
- Identifying relevant evidence
- Recognizing suspicious patterns
- Connecting related findings

I do not include real questions, answers, exact scenarios, machine details, or confidential exam content in this repository.

---

## What eCTHP Added to My Skills

The biggest thing eCTHP added was a **proactive security mindset**.

Before eCTHP, much of my practical experience followed:

```text
Alert
  ↓
Investigate
```

After studying threat hunting, I understood another workflow:

```text
Hypothesis
    ↓
Search
    ↓
Identify
    ↓
Validate
```

The certification reinforced my ability to:

- Build threat-hunting hypotheses
- Identify which telemetry is required for a hunt
- Search proactively for attacker behavior
- Use MITRE ATT&CK to structure hunting ideas
- Analyze endpoint behavior
- Analyze network behavior
- Identify behavioral anomalies
- Correlate events across multiple data sources
- Distinguish IoC-based searching from behavior-based hunting
- Use threat intelligence to generate hunting ideas
- Identify potential detection gaps
- Turn hunting findings into possible detection improvements

---

## Skills I Could Demonstrate More Confidently After eCTHP

After completing eCTHP, I was more comfortable with:

- Starting from attacker behavior rather than an existing alert
- Translating a threat hypothesis into required telemetry
- Searching SIEM data for suspicious behavior
- Investigating unusual process relationships
- Examining command-line activity
- Looking for persistence techniques
- Looking for suspicious authentication behavior
- Correlating endpoint and network telemetry
- Using environmental baselines to identify anomalies
- Mapping observed behavior to MITRE ATT&CK
- Using threat intelligence to inform hunts
- Validating whether unusual activity is malicious or legitimate
- Thinking about how successful hunts could become detections

I would not describe completing eCTHP as making me an experienced professional threat hunter.

For me, it provided a structured practical foundation in threat-hunting methodology and expanded the way I approached Blue Team telemetry.

---

## eCTHP Compared With eCIR

The two certifications were closely related in my learning path but emphasized different mindsets.

| eCIR | eCTHP |
|---|---|
| Incident response | Threat hunting |
| Primarily reactive | Proactive |
| Begin with an incident or suspicious activity | Begin with a hypothesis |
| Determine what happened | Search for behavior that may be undetected |
| Scope attacker activity | Discover hidden activity |
| Respond to confirmed findings | Generate and validate hunting findings |

For me:

```text
eCIR
"What happened?"

        ↓

eCTHP
"What could be happening that we have not detected yet?"
```

That is probably the clearest way I would describe the difference.

---

## eCTHP Compared With BTL1

BTL1 built the broad Blue Team foundation.

eCTHP specialized one area of that foundation.

```text
BTL1
    ↓
SIEM
Threat Intelligence
Endpoint Analysis
Network Analysis
Incident Response
MITRE ATT&CK

        ↓

eCTHP
        ↓
Use Those Capabilities
to Hunt Proactively
```

BTL1 taught me how different defensive disciplines connect.

eCTHP showed me how many of those same sources can be used proactively to search for threats.

---

## My Blue Team Progression

At this point, my learning path had become:

```text
Security+
    ↓
Cybersecurity Foundation
    ↓
BTL1
    ↓
Practical Blue Team Foundation
    ↓
SOC Internship
    ↓
Real Operational Exposure
    ↓
eCIR
    ↓
Incident Investigation & Response
    ↓
eCTHP
    ↓
Proactive Threat Hunting
```

The next step for me was eCDFP, where I went deeper into digital forensics.

---

## Frequently Asked Questions

#### When did I take eCTHP?

August 12, 2026.

#### How long did I prepare specifically for it?

Approximately three days.

That was focused certification-specific preparation after Security+, BTL1, eCIR, and several weeks of SOC experience.

#### Is eCTHP a beginner certification?

INE currently describes it as a **professional-level** certification aimed at defensive-security professionals specializing in proactive threat hunting.

#### Is eCTHP focused on Blue Team work?

Yes.

INE places eCTHP within its defensive-security and threat-hunting certification path.

#### Did BTL1 help?

Significantly.

BTL1 gave me much of the practical foundation in SIEM, threat intelligence, network analysis, endpoint investigation, and MITRE ATT&CK.

#### Did eCIR help?

Yes.

eCIR strengthened my incident-investigation skills immediately before I moved into proactive hunting.

#### Did my SOC internship help?

Yes.

My internship gave me practical exposure to SIEMs, log sources, alerts, investigation, and basic threat-hunting searches.

#### What was the biggest difference from eCIR?

The starting point.

eCIR generally reinforced:

```text
Something happened → investigate it.
```

eCTHP reinforced:

```text
Something may be happening → go search for it.
```

#### What is my biggest preparation recommendation?

Practice the tools and learn how to convert a hypothesis into a search strategy.

---

## Exam Confidentiality

This guide does **not** contain:

- Real exam questions
- Exam answers
- Exact hunting scenarios
- Exact machines or lab configurations
- Confidential datasets
- Flags
- Brain dumps
- Information revealing exam solutions

The purpose is to document:

- My learning process
- My threat-hunting methodology
- What I gained from the certification
- How it connected with my SOC experience
- How it fit into my Blue Team progression

without compromising exam integrity.

---

## Final Thoughts

eCTHP changed the way I thought about security monitoring.

Before it, most of my practical experience followed a reactive model:

```text
Alert
  ↓
Investigate
  ↓
Determine What Happened
```

Threat hunting introduced another model:

```text
Understand Attacker Behavior
        ↓
Create Hypothesis
        ↓
Identify Required Telemetry
        ↓
Search Environment
        ↓
Identify Anomalies
        ↓
Correlate Evidence
        ↓
Validate or Reject Hypothesis
```

The certification showed me that defenders should not always wait for existing detections to tell them where to look.

Sometimes the analyst has to ask:

> **What would an attacker do here?**  
> **What evidence would that behavior produce?**  
> **Do we collect that evidence?**  
> **Can I search for it across the environment?**  
> **Is what I found expected or malicious?**

That proactive investigation mindset was the main skill eCTHP added to my learning path.

It complemented BTL1 and eCIR well:

```text
BTL1
Learn How to Investigate

        ↓

eCIR
Investigate and Respond to Incidents

        ↓

eCTHP
Search Proactively for Threats
```

---

## Official Sources

For current information, verify details directly through:

- [INE Security — Certified Threat Hunting Professional](https://ine.com/security/certifications/ecthp-certification)
- [INE Security — Certifications](https://ine.com/security/certifications)
- [INE Security — Cybersecurity Learning Paths](https://my.ine.com/CyberSecurity/learning-paths)

INE currently positions eCTHP as a professional-level certification for defensive-security practitioners specializing in proactively identifying threats in enterprise environments.

Exam format, pricing, voucher policies, training access, and certification requirements may change after this guide is published.

---

## Disclaimer

This guide combines my personal experience completing eCTHP on August 12, 2026 with publicly available information from INE.

My approximately three days of preparation represent **focused eCTHP-specific preparation**, not the total time required to develop the underlying Blue Team and threat-hunting skills.

My preparation time, previous experience, difficulty perception, and exam experience should not be interpreted as a guarantee of another candidate's experience.

This repository does not contain confidential exam material, brain dumps, memorized questions, or exact exam scenarios.
