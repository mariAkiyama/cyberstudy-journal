---
title: "Phishing"
draft: false
bookCollapseSection: true
weight: 10
---

`# content/en/glossary/test.md` 
## What is Phishing?

Phishing is a type of cyber attack where attackers trick users into revealing sensitive information.

### How to recognize a phishing email:
* **Urgent or threatening language:** The email often demands immediate action.
* **Suspicious links:** Hover over links to check if they lead to an unexpected address.
* **Look-a-like domain:** Fake email domain might be used.
* **Grammatical errors:** Poor spelling and grammar can be a red flag.

### Technical red flags:
>Do not share sensitive information to the public tools.
* **Spoofed Sender Address:** The "From" address may look legitimate, but the email header reveals a different origin.
    * **Tool:** Use **Email Header Analyzers** (e.g., from Google Admin Toolbox or MXToolbox) to parse the full header and verify the true source.
* **Mismatching "Reply-To" Address:** The "Reply-To" address is different from the "From" address, a common tactic to bypass filters.
    * **Tool:** **Email Header Analyzers** can highlight this mismatch and show the true reply-to address.
* **Suspicious File Types:** The email contains attachments with unusual or executable file extensions like `.exe`, `.zip`, `.js`, or `.scr`.
    * **Tool:** Calculate the MD5 hash of the suspicious attachment and check it on **VirusTotal** before opening it. This helps detemine if the file is known malware without uploading potentially legitimatem, but sensitive, content.
* **Embedded Macros:** Attachments (e.g., Office files) prompt you to "Enable Content."
    * **Tool:** Upload the file to **VirusTotal**. It can often detect malicious macros within documents.
* **URL Mismatches:** The displayed link text is legitimate, but the actual URL points to a different, malicious site.
    * **Tool:** Use **VirusTotal** or **PhishTank** to check the actual URL. You can also use browser extensions that provide link previews.
* **Typosquatting/Homoglyph Attacks:** The domain name has a subtle variation of a legitimate one.
    * **Tool:** **URL scanners** like VirusTotal can identify if the domain is known to be malicious. Additionally, browser extensions can help by highlighting suspicious characters.
* **Redirects:** The link uses a shortened URL or multiple redirects to hide its true destination.
    * **Tool:** **URL expander services** (e.g., `checkshorturl.com`) can reveal the final destination of a shortened link without you having to click on it.
* **Use of IP Addresses:** The link points directly to an IP address instead of a domain name.
    * **Tool:** Use **VirusTotal** to check the reputation of the IP address and see if it's associated with known malicious activity
