# Internship Report — Presentation Script

*Speaker: Surendra · Core talk ≈ 10–12 minutes · Deliver at a relaxed pace, pause between the three tasks. The patent list at the end is optional — use it to expand the talk or keep it for questions.*

---

## 1. Opening

Good afternoon, everyone.

My name is Surendra. I'm a final-year law student at IIT Kharagpur, and before law I spent four years working as an AI engineer — so I sit right at the intersection of technology and intellectual property, which is exactly where I've spent the last two months.

Today I'd like to walk you through my internship report — what I worked on over these two months, and what I took away from it.

My work centered on three major tasks. **First, an invention assessment. Second, a patent landscape study on AI-driven cybersecurity. And third, a core IP project built around the Wi-Fi 8 standard.** Let me take each one in turn.

---

## 2. Task One — Invention Assessment

The first task was an invention assessment, and it took me through the complete life cycle of an invention.

It began with sitting down directly with the inventors to understand the idea at its core — not just *what* the invention was, but the problem it set out to solve and what made it different from what already exists. Once I had a clear picture, I carried out **prior-art searches** to map what was already out there and how closely it came to the invention.

On that basis, I **assessed the patentability** of the idea — looking at novelty and inventive step, and identifying which aspects were genuinely protectable. And finally, I **assisted Naveen sir in drafting the claims** — translating the technical concept into the precise legal language that defines the scope of protection.

For me, this was a full journey — from a raw idea, through search and analysis, to a drafted claim — and it gave me a real feel for how an invention travels from the lab to a patent application.

---

## 3. Task Two — AI-Driven Cybersecurity Patent Landscape

The second task was a patent landscape study, requested by **Sharmila, from the AI Security team.**

The objective was to map the landscape of AI-driven cybersecurity patents — to understand the **trends** in the field, the **categories** companies are actively patenting in, **which players** are filing what, and **where the next patentable inventions** are likely to emerge.

I built the entire study from **689 patent records**, covering **22 assignees**, with publications spanning **2023 to 2026**, and then analyzed the trends.

### How I built the categories

Let me first explain how I organized all of this, because the categories are the backbone of the study.

Every patent is stamped with an official technical classification code — but those codes are too broad for strategy work; they lump almost every cybersecurity patent into just one or two giant buckets, which tells you very little. So instead, I **read what each patent actually does** — from its title, abstract and main claim — and sorted it by the *security job it performs.* That gave me **eight clear, industry-standard categories**, and every single patent was counted once, in its main category. Nothing was invented or double-counted — every number traces straight back to the source data.

### The eight categories, in plain terms

Here are the eight, from largest to smallest:

1. **Threat Detection and Response** — the biggest by far, over a third of everything. These catch attacks and decide how to react: spotting suspicious behaviour, scoring alerts, and helping analysts respond.
2. **Network and Cloud Security** — the second biggest. Protecting the network traffic, the cloud, and connected devices.
3. **Vulnerability and Risk Management** — finding weak spots before attackers do, and ranking which ones to fix first.
4. **Identity and Access Management** — making sure only the right people get in: passwords, permissions and privileges.
5. **AI Model Security** — protecting the AI itself, especially large language models, from being tricked or attacked.
6. **Malware and Phishing Defense** — spotting viruses, ransomware, scam emails and malicious links.
7. **Security Automation and Testing** — automating security checks and fixes, especially inside software pipelines.
8. **Data and Privacy Protection** — stopping sensitive data and secrets from leaking.

### What stood out

A few findings jumped out.

First, **the field is highly concentrated.** Just four companies — Microsoft, Cisco, Fortinet and Palo Alto Networks — account for roughly **75%** of the entire dataset, with Microsoft and Cisco alone holding nearly half. In fact, the two most-cited, most-influential patents in the whole set are both Microsoft's.

Second, on categories, **Threat Detection and Response is by far the largest** — over a third of all filings. That tells us it's a crowded, competitive space.

Third, and most interesting strategically — **AI Model Security**, meaning patents that protect language models and generative-AI systems from threats like prompt attacks, is still a relatively small category, but it is clearly the **fastest-emerging** one. The window to stake foundational IP there is open right now.

### White space — where the real opportunities are, and why

This was the part the team cared about most: where is it actually easier to invent something protectable?

The **crowded zones** are the big three — Threat Detection and Response, Network and Cloud Security, and Vulnerability and Risk Management. So much has already been patented there that any new filing has to be very tightly differentiated to stand out.

The **white spaces** are the smaller categories — **Data and Privacy Protection, Security Automation and Testing, and Malware and Phishing Defense** — together with **AI Model Security**, which is small but growing fastest.

**Why these count as white space** is simple: far fewer patents exist there, which means there's less prior art standing in the way of a new filing. So a focused, well-differentiated invention has a much clearer path to protection — especially when it's combined with a cloud, identity, or AI-model angle.

And **where the inventions can actually go** — I highlighted a few concrete directions:
- An **LLM security control plane** — inspecting prompts, verifying AI tool-calls, and validating AI outputs, with an audit trail.
- **Explainable, automated SOC triage** — ranking incidents using evidence graphs and auto-suggesting responses, so analysts aren't drowning in alerts.
- **Exposure-aware vulnerability prioritization** — fusing how critical an asset is, whether an exploit actually exists, and fresh threat intelligence into one score.
- **Automatic least-privilege fixes for the cloud** — recommending and verifying the minimum permissions a workload really needs.
- **Privacy-preserving threat-intelligence sharing** — letting organizations learn from each other's attack data without exposing their raw logs.

The pattern that works for a strong patent is always the same: combine **a specific data source, an AI model, a security decision, and a feedback loop** — rather than just claiming "AI for cybersecurity" in general.

To keep everything auditable, I also identified the **most influential patents** in each category — ranked by how often later patents cite them — and I delivered the study as a full presentation alongside a graph-ready workbook, so the team can trace every number back to the source and recreate any chart themselves.

---

## 4. Task Three — Core IP: Wi-Fi 8 Beacon Management

The third task was a core IP project — and this one was hands-on invention work against the upcoming **Wi-Fi 8 standard.**

Let me set up the problem first. In Wi-Fi, an access point — the AP — periodically broadcasts a small message called a **beacon frame.** This beacon carries the capability and configuration information that a device, or station, needs in order to discover the network and connect to it.

Here's the challenge. Across the generations — Wi-Fi 5, 6 and 7 — the amount of capability information packed into that beacon has kept growing. It has swelled to **around 500 bytes.** And because beacons are broadcast very frequently, repeating this large payload over and over consumes a significant amount of airtime — which actually **slows the connection down.**

Our invention, aimed at Wi-Fi 8 — which is built around **Ultra High Reliability, or UHR** — solves exactly this. Instead of carrying all that heavy information in the beacon, the patent introduces a compact **"UHR operation element"**: a very short indicator, placed inside the beacon frame, that simply signals *the AP supports UHR capabilities.* A station can detect UHR support from this lightweight flag — without the beacon having to carry the full payload. So we keep the channel efficient and connections fast, while still advertising the new capability.

Beyond the invention itself, I also **mapped the patent's claims against the Wi-Fi 8 standard** — lining up each element of our claims with the relevant part of the standard, which is how you build the case that the patent reads onto real-world, standard-compliant products.

This project let me work at the level of a live technical standard, and see how a small, well-placed idea can translate into a valuable, protectable invention.

---

## 5. Closing

So, to sum up — over these two months I worked across three different modes of IP practice: **assessing and drafting a single invention, mapping an entire technology landscape, and contributing to core IP against a live standard.**

What tied them together, for me, was the combination of my engineering background and my legal training — being able to understand the technology deeply, and then think clearly about how to protect it. That has been the most rewarding part of this internship.

Thank you all for your time. I'd be glad to take any questions.

---

## The highlighted patents, in plain English

*Keep this handy. These are the two most-cited patents I flagged in each category. You can weave the top one or two into Task Two, or use the whole list to answer questions.*

**Threat Detection and Response**
- **US11647034 (Microsoft)** — Turns raw network access logs into a map of who is connecting, from where, to which service; learns what "normal" looks like and flags anything far from normal — cutting false alarms. *This is the single most-cited patent in the whole set (109 citations).*
- **US20230259632 (Microsoft)** — Pools security data from many organizations to measure how well security products actually cover different attack techniques, then recommends fixes for the gaps.

**Network and Cloud Security**
- **US20230370452 (Microsoft)** — Builds a map of every device and facility and how critical each one is, discovers devices automatically, and gives each a security score with advice.
- **US20250317739 (Cisco)** — Learns what normal Wi-Fi traffic looks like, generates fake traffic to teach an AI the difference, and then catches both known and brand-new wireless attacks with fewer false alarms.

**Vulnerability and Risk Management**
- **US20240403437 (Cisco)** — Notices when an app relies on an outside third-party service (an API), checks that service for known weaknesses, and acts on them — catching supply-chain risk.
- **US20250047701 (Palo Alto Networks)** — Automatically draws a picture of all your network assets and groups them, so you can see your risk at a glance.

**Identity and Access Management**
- **US12003541 (Palo Alto Networks)** — Checks whether a cloud function has more permissions than it actually needs, and flags it if it's over-privileged.
- **US20250080561 (CyberArk)** — Watches high-privilege sessions and works out whether an action was taken by a real human or by an automated script — catching sneaky automation.

**AI Model Security**
- **US20250181836 (Robust Intelligence)** — An AI that automatically tries to "jailbreak" another AI, holding conversations that slip past its safety rules — a testing tool to find weaknesses before attackers do.
- **US20250335795 (Palo Alto Networks)** — Uses language models to read messy, unstructured documents and answer questions about them, getting better from user feedback.

**Malware and Phishing Defense**
- **US12003535 (Microsoft)** — Reads a web link and its details (its certificate, IP, and where it came from) through a transformer AI to decide if it's a phishing link — and even trains itself on fake, tricky links.
- **US11687652 (Trend Micro)** — Creates a "fingerprint" of a suspicious file that works no matter what chip it runs on, compares it to known malware fingerprints, and names the malware family if it matches.

**Security Automation and Testing**
- **US11620379 (Google)** — Watches commands before the computer runs them, uses AI to spot hidden or disguised malicious commands, and blocks them.
- **US11550911 (Palo Alto Networks)** — Uses AI to analyze source code in several ways at once to decide if it's malicious, then acts on it — security built right into the software pipeline.

**Data and Privacy Protection**
- **US11783062 (Microsoft)** — Treats "secrets" like passwords, tokens and certificates specially, tagging each with risk information — how exposed it is, how much damage a leak would cause — and controls access accordingly. *This is the second most-cited patent in the set (70 citations).*
- **US11921820 (Fortinet)** — A smarter way to train security AI using far fewer hand-labeled examples, by grouping similar data and labeling just one example per group.

---

### Delivery tips
- **Timing:** the core talk (sections 1–5) runs about 10–12 minutes. The patent list is a bonus — mention two or three, and keep the rest for Q&A.
- **Signposting:** the *"First… Second… Third…"* in your opening frames the whole talk — lean on it so the audience always knows where you are.
- **Task Two:** the strongest new part is the white-space story — say *what's* crowded, *what's* open, and *why* (fewer patents = less prior art in the way). That's the insight the team will remember.
- **Task Three:** build up the problem ("500 bytes, broadcast very frequently, slows the connection") before revealing the fix — that contrast is what lands.
- **Numbers:** swap in any exact figures you have (precise category percentages, beacon rate) into the bolded spots.
- **Credit:** naming Naveen sir and Sharmila is good — it shows you worked within a team.
