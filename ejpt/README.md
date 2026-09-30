# eJPT — Junior Penetration Tester

> **Last verified:** September 2026  
> **Exam taken:** August 17, 2026  
> **Provider:** INE Security  
> **Level:** Junior / Entry-Level  
> **Focus:** Penetration Testing / Offensive Security  
> **Delivery:** Online / Remote  
> **Exam format:** Practical, browser-based lab  
> **Focused certification-specific preparation:** Approximately 3 days

## Key Takeaways

- Added an entry-level offensive-security perspective to a primarily Blue Team background.
- Practiced reconnaissance, enumeration, vulnerability identification, exploitation, web testing, and pivoting.
- Learned why thorough enumeration should drive exploitation rather than relying on random exploit attempts.
- Improved my defensive reasoning by understanding how attacker actions can appear in network, authentication, endpoint, and web telemetry.

---

## Overview

The Junior Penetration Tester, commonly known as eJPT, is an entry-level practical penetration-testing certification from INE Security.

INE currently describes eJPT as a hands-on certification that assesses skills across the penetration-testing lifecycle, including:

- Assessment methodologies
- Host and network auditing
- Host and network penetration testing
- Web application penetration testing

The current version was updated in March 2026, with the exam expanding to 45 questions while keeping the 48-hour practical format. INE also expanded the training around reconnaissance, web application testing, and offensive AI workflows.

I completed eJPT on **August 17, 2026**.

Unlike my other INE certifications, eJPT represented a move into offensive security.

However, I did not approach it as someone whose main focus was Red Teaming.

My background was already heavily defensive.

That made eJPT especially useful because it allowed me to look at attacks from the opposite side:

> **Instead of only investigating what an attacker did, I practiced how an attacker discovers, evaluates, exploits, and moves through an environment.**

---

## My Background Before eJPT

By the time I started eJPT, I had already completed:

- CompTIA Security+
- Blue Team Level 1
- eCIR
- eCTHP
- eCDFP
- Approximately seven weeks of SOC internship experience

My main background was therefore:

```text
Security Operations
      +
Incident Response
      +
Threat Hunting
      +
Digital Forensics
```

not penetration testing.

However, that defensive background made many offensive concepts easier to understand.

I was already familiar with concepts such as:

- IP addresses
- Ports
- Protocols
- Services
- Vulnerabilities
- Authentication
- Firewalls
- Logs
- Lateral movement
- Persistence
- Credential access
- MITRE ATT&CK
- Endpoint activity
- Network traffic

The main difference was perspective.

Before eJPT, I often thought:

```text
Attacker Activity
      ↓
Logs / Alerts
      ↓
Investigate
```

eJPT made me think more like:

```text
Target
  ↓
Reconnaissance
  ↓
Enumeration
  ↓
Identify Weakness
  ↓
Exploit
  ↓
Gain Access
  ↓
Expand Access
```

That was the main value of the certification for me.

---

## Why My Blue Team Background Helped

A large part of entry-level offensive security involves technologies I had already encountered from the defensive side.

For example:

| Blue Team Perspective | eJPT Perspective |
|---|---|
| Investigate an open service | Enumerate the service |
| Detect password attacks | Perform controlled password attacks |
| Investigate lateral movement | Understand how lateral movement is performed |
| Analyze suspicious web requests | Generate and test web requests |
| Investigate remote access | Establish remote access |
| Identify exploitation evidence | Perform controlled exploitation |
| Detect reconnaissance | Perform reconnaissance |

Because the underlying technologies were familiar, I mostly needed to learn:

> **How would an attacker actually use them?**

That significantly reduced the learning curve.

---

## My Progression Into Offensive Security

My path into eJPT looked approximately like:

```text
Security+
    ↓
Understand Security Fundamentals
    ↓
BTL1
    ↓
Investigate Attacker Activity
    ↓
SOC Experience
    ↓
See Real Security Telemetry
    ↓
eCIR / eCTHP / eCDFP
    ↓
Understand Incidents, Hunting, and Forensics
    ↓
eJPT
    ↓
Understand the Attacker's Workflow
```

For me, eJPT did not replace the Blue Team path.

It complemented it.

---

## The Penetration Testing Mindset

The biggest difference I noticed was that penetration testing is not:

```text
Run Exploit
    ↓
Get Shell
```

A large amount of the work happens before exploitation.

A more realistic simplified workflow is:

```text
Understand Scope
      ↓
Reconnaissance
      ↓
Host Discovery
      ↓
Port Scanning
      ↓
Service Enumeration
      ↓
Vulnerability Identification
      ↓
Validate Potential Attack Path
      ↓
Exploitation
      ↓
Post-Exploitation
      ↓
Further Enumeration
```

The important lesson was:

> **Enumeration drives exploitation.**

If you do not understand the target, you do not know what to attack.

---

## Reconnaissance

Reconnaissance is about collecting information that can guide later testing.

Depending on the target, this may include:

- Hosts
- IP addresses
- Domains
- Subdomains
- Technologies
- Network structure
- Exposed services
- Web applications

A simplified process is:

```text
Target
   ↓
Collect Information
   ↓
Identify Attack Surface
   ↓
Prioritize Testing
```

The goal is not collecting information for its own sake.

The goal is identifying useful attack paths.

---

## Host Discovery

Before testing services, you need to know which systems are alive.

This can involve identifying:

- Active hosts
- Reachable systems
- Network ranges
- Potential gateways
- Other reachable subnets

From a Blue Team perspective, this also helped me better understand why reconnaissance activity can produce recognizable network patterns.

---

## Port Scanning

Port scanning answers an important question:

> **What is exposed?**

For example:

```text
Target Host
    ↓
Open Port 22
Open Port 80
Open Port 445
    ↓
SSH
HTTP
SMB
```

But finding an open port is only the beginning.

The next step is enumeration.

---

## Service Enumeration

This was one of the most important ideas reinforced by eJPT.

Knowing that a port is open does not automatically tell you what to do next.

For example:

```text
Port 445 Open
      ↓
SMB
      ↓
What Version?
What Shares?
What Users?
What Permissions?
What Authentication Is Allowed?
```

Or:

```text
Port 80 Open
      ↓
Web Application
      ↓
What Technology?
What Directories?
What Inputs?
What Authentication?
What Functionality?
```

This is where enumeration becomes much more important than simply scanning.

---

## Nmap and Network Enumeration

Nmap was one of the important tools in the learning path.

For me, the value was not memorizing every Nmap flag.

It was understanding the questions scanning can answer.

For example:

```text
Which hosts are reachable?
        ↓
Which ports are open?
        ↓
Which services are running?
        ↓
Which versions are exposed?
        ↓
What should I investigate next?
```

That workflow is much more important than memorizing isolated commands.

---

## Vulnerability Identification

After identifying services and applications, the next question becomes:

> **Is there a weakness I can realistically exploit?**

That may involve:

- Outdated services
- Weak credentials
- Misconfiguration
- Exposed administrative interfaces
- Vulnerable web functionality
- Known vulnerabilities

One important lesson is:

```text
Service Version
      +
Configuration
      +
Environment
      ≠
Guaranteed Exploitability
```

Finding a CVE associated with a product does not automatically mean exploitation will succeed.

The weakness needs to be validated in context.

---

## Exploitation

Exploitation is where a confirmed weakness is used to gain additional access.

In a controlled penetration-testing environment, this may involve:

- Exploiting a vulnerable service
- Using weak credentials
- Exploiting web functionality
- Establishing a shell
- Gaining remote access

The important lesson for me was that exploitation is only one stage of the overall process.

```text
Reconnaissance
      ↓
Enumeration
      ↓
Identify Weakness
      ↓
Exploit
```

Without the earlier stages, exploitation becomes guesswork.

---

## Metasploit

Metasploit was one of the frameworks I practiced with.

From my Blue Team background, I was already familiar with the name and with the idea that exploitation frameworks can generate recognizable attacker activity.

Using it from the offensive side helped me better understand the workflow.

For example:

```text
Identify Vulnerability
      ↓
Find Relevant Module
      ↓
Configure Target
      ↓
Configure Payload
      ↓
Execute
      ↓
Evaluate Result
```

The important part was not:

> "Metasploit automatically hacks systems."

It was understanding what information is required before an exploit can be used successfully.

---

## Password Attacks

Another area involved authentication attacks.

Tools such as Hydra can be used in authorized environments to test weak credentials.

The important defensive takeaway for me was seeing how credential attacks are actually structured.

For example:

```text
Identify Authentication Service
        ↓
Identify Possible Usernames
        ↓
Test Credentials
        ↓
Successful Authentication
```

That made defensive concepts such as:

- Account lockout
- MFA
- Strong passwords
- Rate limiting
- Authentication monitoring

more concrete.

---

## Web Application Testing

The current eJPT emphasizes web application penetration testing more heavily than older versions. INE's 2026 update specifically expanded this area.

The general workflow involves understanding:

- Application structure
- Inputs
- Authentication
- Directories and files
- Requests and responses
- Potential vulnerabilities

A simplified workflow is:

```text
Web Application
      ↓
Map Functionality
      ↓
Identify Inputs
      ↓
Inspect Requests
      ↓
Test Behavior
      ↓
Validate Weakness
```

This reinforced that web testing is not simply running an automated scanner.

You need to understand how the application behaves.

---

## Burp Suite

Burp Suite helps make web traffic visible and controllable.

A simplified workflow is:

```text
Browser Request
      ↓
Burp Proxy
      ↓
Inspect Request
      ↓
Modify Parameters
      ↓
Forward Request
      ↓
Observe Response
```

This was useful from a Blue Team perspective too.

Web attacks that appear as:

```text
Suspicious HTTP Request
```

inside security logs become easier to understand after manually creating and modifying requests yourself.

---

## Directory and Content Discovery

Web applications can expose content that is not directly linked from the main interface.

Enumeration can therefore include searching for:

- Hidden directories
- Administrative panels
- Backup files
- API paths
- Configuration files
- Other exposed resources

The lesson was similar to network enumeration:

> **Do not assume the visible surface is the complete attack surface.**

---

## Pivoting and Network Movement

One of the most interesting concepts for me was pivoting.

A compromised host may provide access to systems that were not directly reachable from the original attacker position.

A simplified example:

```text
Attacker
   ↓
Target A
   ↓
Internal Network
   ↓
Target B
```

From a Blue Team perspective, this made lateral movement much easier to visualize.

Previously, I mostly investigated:

```text
Source
  ↓
Destination
```

After practicing offensive networking concepts, I had a clearer understanding of why one compromised system can become a stepping stone into another part of the network.

---

## Post-Exploitation

Gaining access is not necessarily the end of an attack.

After initial compromise, an attacker may:

- Enumerate the system
- Identify users
- Examine network configuration
- Search for credentials
- Identify other hosts
- Establish persistence
- Move laterally
- Access sensitive information

This made the attack lifecycle more concrete to me.

For example:

```text
Initial Access
      ↓
System Enumeration
      ↓
Privilege / Credential Discovery
      ↓
Persistence
      ↓
Lateral Movement
```

These are exactly the kinds of behaviors defenders later try to detect.

---

## How eJPT Changed My Defensive Thinking

This was the most important part of eJPT for me.

Before eJPT, I might investigate an event such as:

```text
Repeated Connections to Multiple Ports
```

and recognize it as possible scanning.

After practicing scanning myself, I had a better understanding of:

- Why the attacker scans
- What information they want
- What they may do with the result
- Which step likely follows

Similarly:

```text
Repeated Authentication Failures
```

became easier to connect with how password attacks are performed.

And:

```text
Internal Host Connecting to Another Internal Host
```

became easier to interpret in the context of possible lateral movement.

The offensive perspective gave additional meaning to defensive telemetry.

---

## Attacker Action → Defender Visibility

One of the most valuable mental models I took from eJPT was:

| Attacker Action | Possible Defensive Evidence |
|---|---|
| Host discovery | Network telemetry |
| Port scanning | Firewall / NDR logs |
| Service enumeration | Repeated service requests |
| Password attacks | Authentication failures |
| Exploitation | Endpoint / network alerts |
| Command execution | Process telemetry |
| Remote access | Authentication and remote-session logs |
| Pivoting | Internal network connections |
| Persistence | Endpoint artifacts |
| Web testing | Web / WAF logs |

This does not mean every attack automatically generates perfect evidence.

But understanding the attacker's workflow helped me ask better defensive questions.

---

## How I Prepared

My focused preparation for eJPT was approximately **three days**.

My main preparation resource was INE.

I focused on:

- The official learning path
- Practical labs
- Tool navigation
- Enumeration methodology
- Network scanning
- Exploitation workflow
- Web application testing
- Pivoting concepts
- Authentication attacks

However, the three days should not be misunderstood.

I was not learning networking, attacks, and security concepts from zero.

My actual background looked more like:

```text
Security+
    ↓
BTL1
    ↓
SOC Internship
    ↓
eCIR
    ↓
eCTHP
    ↓
eCDFP
    ↓
3 Days of Focused eJPT Preparation
    ↓
Exam
```

My previous Blue Team depth made many of the introductory offensive concepts familiar.

The main challenge was learning to apply them from the attacker's side.

---

## Why My Preparation Was Short

My preparation time should **not** be interpreted as:

> **eJPT only takes three days to learn.**

That is not what happened.

Before eJPT, I already understood:

- Networking
- Common protocols
- Ports
- Vulnerabilities
- Authentication
- Security controls
- Attacker techniques
- Lateral movement
- Persistence
- Network analysis

The defensive certifications had taught me:

```text
"What does this attack look like?"
```

eJPT mainly added:

```text
"How is this attack actually performed?"
```

That difference made the learning curve much shorter for me.

---

## My Most Important Preparation Advice: Enumerate Everything

If I had to choose one lesson from eJPT, it would be:

> **Do not rush exploitation. Enumerate first.**

A weak approach is:

```text
Find Host
   ↓
Try Random Exploits
```

A stronger approach is:

```text
Find Host
   ↓
Scan Ports
   ↓
Identify Services
   ↓
Enumerate Services
   ↓
Understand Versions / Configuration
   ↓
Identify Potential Weakness
   ↓
Validate
   ↓
Exploit
```

The quality of the exploitation phase depends heavily on the quality of enumeration.

---

## Take Notes

Another important habit is keeping organized notes.

Useful information may include:

- IP addresses
- Hosts
- Open ports
- Services
- Versions
- Credentials
- Interesting directories
- Potential vulnerabilities
- Successful commands
- Failed attempts
- Pivot routes

A simple structure can prevent repeatedly rediscovering the same information.

This is particularly important because the exam environment can be reset, and INE's eJPT lab guidelines warn that resetting deletes data stored on the provided Kali system. INE recommends saving useful scan results and notes locally.

---

## Tool Familiarity Matters

The eJPT exam environment I used provided a preconfigured Kali Linux system with the required tools, scripts, wordlists, Metasploit, and a local Exploit-DB/SearchSploit installation.

The Kali system itself was not connected to the Internet, while the host system could be used for research and note-taking.

Because the required tooling is available, preparation should focus less on installation and more on actually knowing how to use the tools.

I recommend practicing:

- Navigation
- Scanning
- Search and filtering
- Editing command options
- Reading tool output
- Saving results
- Pivoting between findings

---

## Tools I Practiced

My eJPT preparation included practical exposure to tools and techniques such as:

### Network Enumeration

- Nmap
- Linux networking utilities

### Exploitation

- Metasploit Framework
- SearchSploit / Exploit-DB

### Web Application Testing

- Burp Suite
- Content and directory discovery tools

### Authentication Testing

- Hydra

### Remote Access and Networking

- Netcat
- Remote-service clients
- Kali Linux networking tools

The important part was not memorizing tool names.

It was understanding the role each one plays in the penetration-testing process.

---

## My Exam Experience

I completed eJPT remotely on August 17, 2026.

The version I took was the updated 2026 exam.

INE announced in March 2026 that the revised exam contains **45 questions** and keeps the **48-hour hands-on practical format**.

My exam experience included:

- Practical interaction with the provided lab
- Questions based on information retrieved from machines
- Theoretical multiple-choice questions
- Fill-in-the-blank style answers

For many questions, understanding the answer required me to actually enumerate or interact with the environment first.

That reinforced why practical tool familiarity matters.

I do not include real exam questions, answers, exact targets, flags, or confidential lab details in this repository.

---

## What eJPT Added to My Skills

eJPT helped me become more comfortable with:

- Thinking through the penetration-testing lifecycle
- Performing host discovery
- Scanning ports and services
- Enumerating exposed services
- Identifying possible weaknesses
- Validating vulnerabilities
- Using exploitation frameworks
- Performing basic web application testing
- Understanding password attacks
- Establishing remote access in controlled labs
- Understanding post-exploitation
- Understanding pivoting and lateral movement
- Connecting attacker actions with defensive telemetry

The most important value for me was not becoming a Red Team specialist.

It was developing **attacker perspective**.

---

## Skills I Could Demonstrate More Confidently After eJPT

After completing eJPT, I was more comfortable with:

- Mapping an attack surface
- Moving from host discovery to service enumeration
- Reading scan results and deciding what to investigate next
- Using Nmap as part of a structured enumeration process
- Identifying potential attack paths
- Using Metasploit in a controlled lab
- Interacting with web requests through Burp Suite
- Understanding basic password-attack workflows
- Understanding the role of remote services in attacks
- Thinking through post-exploitation steps
- Understanding basic pivoting
- Explaining how common offensive actions may appear to defenders

I would not describe myself as a professional penetration tester based on eJPT alone.

For me, eJPT gave me a practical entry-level offensive-security foundation that complements my primary Blue Team focus.

---

## eJPT Compared With Security+

The difference between Security+ and eJPT was very clear.

| Security+ | eJPT |
|---|---|
| Broad cybersecurity foundation | Offensive-security fundamentals |
| Understand attacks conceptually | Perform controlled attacks |
| Learn what vulnerabilities are | Identify and validate weaknesses |
| Learn network-security concepts | Enumerate network services |
| Understand web attacks | Test web applications |
| Understand authentication attacks | Perform controlled credential testing |

For me:

```text
Security+
"What is this attack?"

        ↓

eJPT
"How would an attacker actually perform it?"
```

---

## eJPT Compared With BTL1

BTL1 and eJPT examine security from opposite perspectives.

```text
eJPT
Attacker
  ↓
Reconnaissance
  ↓
Enumeration
  ↓
Exploitation

BTL1
Defender
  ↓
Alert
  ↓
Evidence
  ↓
Investigation
```

Studying both made the relationship between offensive and defensive security clearer.

---

## How eJPT Complements My Blue Team Path

My primary focus remains defensive security.

That is why eJPT is valuable in my certification path.

For example:

```text
eJPT
Understand the Attack

        ↓

BTL1 / eCIR
Investigate the Attack

        ↓

eCTHP
Hunt for the Attack

        ↓

eCDFP
Analyze the Evidence Left by the Attack
```

This gives me a more complete view of the security lifecycle.

---

## Current Certification Information

INE currently describes eJPT as a browser-based, hands-on certification covering:

- Assessment methodologies
- Web application penetration testing
- Host and network penetration testing
- Host and network auditing


Regular exam vouchers currently expire after **180 days**. One free retake is included after an unsuccessful attempt and must be completed within **14 days**, with both attempts occurring before voucher expiration. Passing eJPT credentials are currently valid for **three years**.

---

## Frequently Asked Questions

#### When did I take eJPT?

August 17, 2026.

#### Was eJPT my first offensive-security certification?

Yes.

#### How long did I prepare specifically for it?

Approximately three days.

That was focused certification-specific preparation after extensive prior defensive-security learning.

#### Is eJPT practical?

Yes.

INE describes it as a browser-based, hands-on penetration-testing exam.

#### How long is the current exam?

INE's March 2026 update states that the exam keeps a **48-hour practical format**.

#### How many questions are on the current exam?

The 2026 update increased the exam from 35 to **45 questions**.

#### Did my Blue Team background help?

Significantly.

I was already familiar with many attacker techniques from investigating them defensively.

#### What was new for me?

Performing the actions from the offensive side:

- Enumeration
- Exploitation
- Web testing
- Password attacks
- Post-exploitation
- Pivoting

#### What is my biggest preparation recommendation?

Do not rush exploitation.

Enumerate thoroughly first.

---

## Exam Confidentiality

This guide does **not** contain:

- Real exam questions
- Exam answers
- Exact target IPs
- Exact vulnerabilities from the exam
- Flags
- Credentials
- Machine configurations
- Confidential lab data
- Brain dumps

The purpose of this guide is to document:

- What I learned
- How I prepared
- How my defensive background helped
- Which offensive skills I developed
- How eJPT fits into my Blue Team path

without compromising exam integrity.

---

## Final Thoughts

eJPT was useful to me because it gave me the attacker's perspective.

Before eJPT, I had already spent significant time studying how defenders:

- Detect
- Investigate
- Hunt
- Analyze evidence

eJPT helped complete the picture by teaching me to think through:

```text
How does the attacker find the target?

How do they discover exposed services?

How do they decide what to attack?

How do they exploit a weakness?

What do they do after gaining access?

How might they move further?
```

That changed the way I interpreted defensive telemetry.

Instead of only recognizing:

> **"This looks like scanning."**

I understood more clearly:

> **"The attacker is probably trying to map the attack surface and decide what to enumerate next."**

Instead of only seeing:

> **"Repeated authentication failures."**

I had a clearer understanding of how credential attacks generate that activity.

And instead of only investigating lateral movement, I had practiced the basic concepts behind how an attacker reaches another system.

That is the role eJPT plays in my certification path:

```text
Security+
Understand Security

        ↓

BTL1
Investigate Security Events

        ↓

eCIR
Respond to Incidents

        ↓

eCTHP
Hunt for Threats

        ↓

eCDFP
Analyze Forensic Evidence

        ↓

eJPT
Understand the Attacker
```

My goal with eJPT was not to present myself as an experienced penetration tester.

It was to build enough practical offensive-security understanding to become a better defender.

---

## Official Sources

For current information, verify details directly through:

- [INE — eJPT Certification](https://ine.com/security/certifications/ejpt-certification)
- [INE Security — Cybersecurity Learning Paths](https://my.ine.com/CyberSecurity/learning-paths)

INE updated eJPT in March 2026 with expanded reconnaissance and web-application content, an updated exam, and 45 questions while retaining the 48-hour practical format.

Exam content, policies, pricing, and training may change after this guide is published.

---

## Disclaimer

This guide combines my personal experience completing eJPT on August 17, 2026 with publicly available information from INE.

My approximately three days of preparation represent **focused eJPT-specific preparation**, not the total time required to develop the networking, cybersecurity, and attacker-methodology knowledge behind the certification.

My preparation time, prior knowledge, exam experience, and perceived difficulty should not be interpreted as a guarantee of another candidate's experience.

This repository does not contain confidential exam material, brain dumps, memorized questions, or exact exam scenarios.
