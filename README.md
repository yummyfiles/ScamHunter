# ScamHunter

**Finding, documenting, and reporting harmful websites and online activity.**

ScamHunter isn't just about scams. It's a free, open-source project for researching websites and online services that can harm people, expose their information, spread malware, or trick them into doing something risky. The goal is to keep useful evidence and sources in one place so people can understand what's going on and report it responsibly.

> **quick reminder:** a weird domain, an unfamiliar site, or an accusation online doesn't automatically prove anything. We need evidence, not just vibes.

## What this project covers

- **Scams and phishing:** fake stores, fraudulent giveaways, impersonation, phishing pages, deceptive ads, and redirect tricks.
- **Non-consensual image sharing and exploitation:** sites that distribute people's images without permission or profit from that abuse. We don't repost the images themselves.
- **Doxxing and personal-data exposure:** data-broker sites, exposed personal information, and databases or dumps that put people at risk. We don't mirror private data dumps or publish unnecessary personal details.
- **Malware and malicious infrastructure:** harmful downloads, malware-distribution URLs, botnet indicators, and other threats documented by public threat-intelligence sources.
- **Dark-web and other high-risk services:** publicly documented services associated with stolen data, exploitation, illegal marketplaces, or other harmful activity. Research stays within safe and lawful boundaries.
- **Other harmful sites and online activity:** anything else with credible evidence of harm, even if it doesn't fit neatly into one category.

These are research categories, not automatic labels. A site should not be called harmful just because its name looks suspicious or someone made an accusation about it.

## How we document things

We try to separate what a source reports from what ScamHunter has actually checked. A useful record should include the source, date checked, evidence or reference, known limitations, and confidence level.

- **Confirmed / corroborated:** credible evidence supports the specific claim, ideally from multiple independent sources or a reliable authoritative source.
- **Unverified lead:** worth checking, but not independently confirmed yet.
- **Resolved / inactive:** the reported activity appears to have stopped or the indicator is no longer active. That doesn't erase historical risk.

A listing in a public feed is evidence that the feed reported something; it isn't automatically proof of every claim about a site. We don't promise that a website is safe just because we haven't found reports about it.

## Research rules

- Don't break into accounts, bypass access controls, exploit systems, or disrupt sites.
- Don't download suspicious files, submit personal information, interact with criminal services, or open harmful content just to investigate it.
- Don't publish victims' private information, credentials, private messages, or copies of non-consensual images.
- For sensitive cases, document only what's necessary: public source references, dates, relevant domains or indicators, and a clear description of the risk.
- Don't harass people, encourage retaliation, or make claims you can't support.
- If you're not sure, say you're not sure.
- Use the tools in [sources/](sources/README.md) responsibly. If a task genuinely needs a VM, configure it carefully: disable shared folders and clipboard, avoid unnecessary USB access, and isolate networking. A VM is an extra layer, not a guarantee of containment.

## Current status

ScamHunter is still getting set up. Right now, it's focused on research guidelines, lead tracking, report templates, and useful sources. Automated scanning might come later, once there's a safe and sensible way to do it.

## Want to help?

1. Read [CONTRIBUTING.md](CONTRIBUTING.md) and [SECURITY.md](SECURITY.md) first.
2. Stick to evidence you can collect safely and lawfully.
3. Use the [report template](reports/REPORT_TEMPLATE.md) to write down what you found.
4. Keep unverified leads clearly marked, and include sources and dates.
5. Protect the people who may be affected by the site you're documenting.

## Where to report a site or incident

These are useful starting points, depending on what you found:

- [Google Safe Browsing — report phishing](https://safebrowsing.google.com/safebrowsing/report_phish/)
- [Microsoft — report an unsafe site](https://www.microsoft.com/en-us/wdsi/support/report-unsafe-site)
- [FTC ReportFraud](https://reportfraud.ftc.gov/) — fraud in the US
- [FBI IC3](https://www.ic3.gov/) — internet crime reports in the US
- [CISA](https://www.cisa.gov/report) — cybersecurity incidents and issues

For non-consensual intimate images or exposed personal information, use the platform's reporting/removal process and appropriate official support channels. Avoid resharing the material as evidence. Check each organization's current instructions before submitting anything. ScamHunter is independent and isn't officially connected to any of these organizations.

## Disclaimer

Read [DISCLAIMER.md](DISCLAIMER.md) before using this project or relying on its findings. ScamHunter provides information for general educational and informational purposes only; it does not guarantee that a website is safe or harmful, and it is not legal, financial, or cybersecurity professional advice.

## Repo map

- `research/` — leads we're checking and notes on what we actually know
- `reports/` — report templates and notes
- `sources/` — threat-checking tools, privacy tools, virtualization options, and reporting links
- `CONTRIBUTING.md` — how to contribute without making a mess
- `SECURITY.md` — keeping research safe
- `DISCLAIMER.md` — the project's formal disclaimer

## The basics

- **Evidence first.** Suspicious doesn't automatically mean guilty.
- **Stay safe.** Don't download random files, enter your info, or turn off security protections.
- **Don't cross the line.** No unauthorized access, exploiting stuff, or disrupting sites.
- **Protect people.** Keep private and sensitive info out of reports.
- **Be honest.** Include sources, dates, limitations, and how confident you actually are.

## License

No license has been picked yet. Until one is added, don't assume this repo gives permission to reuse, modify, or redistribute its contents.
