# FUTURE_CS_02

# Phishing Detection & Awareness System

**Cyber Security Task 2 (2026) — Future Interns**

A hands-on security-analyst exercise: analyzing phishing email samples, documenting the indicators that expose them, classifying risk, and producing an awareness training deliverable a real business could use.

> This is a defensive, educational project. No malicious content was created, sent, or executed. All email samples in this repo are illustrative reconstructions used for analysis and training only.

## Repository contents

| File | Description |
|---|---|
| [`Phishing_Detection_Awareness_Report.docx`](./Phishing_Detection_Awareness_Report_FI-2.docx) | Full analyst report: methodology, four analyzed email exhibits (indicators + risk rating for each), the risk classification framework, a plain-language explanation of how phishing attacks work, and prevention/Do's-and-Don'ts guidance. |
| [`phishing-training-module.html`](./phishing-training-module.html) | Interactive, self-contained web training module for end users — annotated email/URL exhibits, social engineering tactics, case studies, and a scored quiz. Open directly in a browser. |
| `README.md` | This file. |

## Objective

Work through phishing samples the way a security analyst would:

1. Analyze phishing email samples
2. Identify common phishing indicators
3. Classify each email's risk level
4. Explain the attack in simple, non-technical language
5. Turn the findings into an awareness deliverable others can actually use

## Tools used

| Tool | Purpose |
|---|---|
| [Google Admin Toolbox — Message Header](https://toolbox.googleapps.com/apps/messageheader/) | Parses raw email headers to reveal the true originating server and SPF/DKIM/DMARC authentication results. |
| [MxToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx) | Cross-checks authentication results and mail routing against known infrastructure. |
| Browser address-bar / hover inspection | Manually reveals a hyperlink's true destination and checks domain structure before clicking. |
| Google Docs / MS Word | Report drafting and formatting into a client-ready `.docx`. |

## Analysis approach

1. **Read as a user would** — note first impressions: tone, urgency, requests.
2. **Check the sender** — the full email address, not just the display name.
3. **Review headers** — SPF/DKIM/DMARC authentication results and originating domain.
4. **Inspect links** — hover (never click) to reveal the real destination URL and check for domain look-alikes.
5. **Check formatting details** — generic greetings, spelling/grammar irregularities, mismatched branding.
6. **Classify risk** — apply the Safe / Suspicious / Phishing framework and document the reasoning.

### Risk classification framework

| Rating | Criteria |
|---|---|
| 🟢 **Safe** | Sender domain matches exactly; SPF/DKIM/DMARC all pass; no urgency, payment, or credential request; links resolve to the expected domain. |
| 🟡 **Suspicious** | One or two irregularities present without conclusive evidence of malicious intent — verify before acting. |
| 🔴 **Phishing** | Multiple indicators together: failed authentication, look-alike/mismatched domain, urgency/fear tactic, and a request for credentials, payment, or sensitive data. |

## What's in the report

- 4 analyzed email exhibits (3 phishing/suspicious, 1 legitimate for contrast), each with headers, indicators table, risk badge, and plain-language explanation
- The full risk classification framework
- A plain-language breakdown of how phishing attacks work (disguise → trigger → capture → exploitation)
- Prevention guidelines and a Do's / Don'ts table for employees

## Study references

These public repositories were reviewed for context on real-world phishing email structure and datasets — **study only, not reused or reproduced here**:

- [phishing_pot](https://github.com/rf-peixoto/phishing_pot) — collected real phishing samples
- [phishing-mail-examples](https://github.com/autinerd/phishing-mail-examples) — header + body text samples
- [Phishing_Email](https://github.com/sadat1971/Phishing_Email) — labeled phishing/non-phishing dataset
- [Phishing.Database](https://github.com/Phishing-Database/Phishing.Database) — phishing domain/URL dataset


## Usage

- **Report**: open `Phishing_Detection_Awareness_Report.docx` in Word, Google Docs, or LibreOffice.
- **Training module**: download `phishing-training-module.html` and open it in any browser, or host it via GitHub Pages (Settings → Pages) for a shareable link.

## Author

[Your Name] — Cyber Security Track, Future Interns
