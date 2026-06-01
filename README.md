# week 11 : Phishing - Phishmas Greetings

### Flag 1 : Spoofed Invoice Alert

Flag : ``` THM{yougotnumber1-keep-it-going} ```

---
#### Indicators Identified
- Spoofing: The sender appears legitimate but the underlying email address does not match the claimed identity
- Sense of Urgency: Classic “Pay immediately” or “Invoice overdue” pressure tactic.
- Fake Invoice: Attachments or links pretending to be invoices ; common phishing vector.

#### Email Content
<img width="1910" height="1021" alt="Screenshot 2026-06-01 225547" src="https://github.com/user-attachments/assets/15e36cca-c798-4044-a6f0-0519278017ab" />
<br>

#### Suspicious Sender Address
<img width="848" height="558" alt="Screenshot 2026-06-01 225645" src="https://github.com/user-attachments/assets/5ec6b112-1a44-44dc-b8f4-0d95d2841174" />

<br>

#### Classification & Flag
<img width="844" height="801" alt="Screenshot 2026-06-01 225753" src="https://github.com/user-attachments/assets/7fd64fc1-d905-4d17-826e-6e56d1844f23" />

#### Explanation
- The first email sets the tone: an urgent invoice request designed to panic the user. 
- These attacks attempt to trick accounting teams into immediate payment.
- Always verify sender domains and cross-check invoice legitimacy.

---

### Flag 2 : Suspicious Attachment From a Spoofed Sender
Flag : ``` THM{nmumber2-was-not-tha-thard!} ```

---
#### Indicators Identified
- Impersonation: Attacker pretends to be a known internal staff member.
- Spoofing: Email headers, reply-to, or display name mismatch.
- Malicious Attachment: Risky .zip, .exe, or macro-enabled documents.

#### Email Content
<img width="1914" height="795" alt="Screenshot 2026-06-01 225931" src="https://github.com/user-attachments/assets/ba064a07-8108-4f42-85b0-682ff5c87cdb" />
<br>

#### Suspicious Attachment
<img width="1208" height="227" alt="Screenshot 2026-06-01 225953" src="https://github.com/user-attachments/assets/795d5936-777e-4b7a-bc64-beb2e5c552e9" />
<br>

#### Classification & Flag
<img width="833" height="789" alt="Screenshot 2026-06-01 230036" src="https://github.com/user-attachments/assets/019064b5-457c-4c7d-84de-9f5b7239cfab" />

#### Explanation
- The second phishing email includes a dangerous attachment.
- These are often used to deploy malware such as keyloggers or RATs.
- File extension and email origin clearly show tampering.

---

### Flag 3 : High-Pressure Social Engineering Attempt
Flag : ``` THM{Impersonation-is-areal-thing-keepIt} ```

---
#### Indicators Identified
- Impersonation: Identity forged to gain trust.
- Social Engineering Text: Emotional manipulation, friendly tone, or authority tone.
- Sense of Urgency: “Do this now,” “We’re running out of time,” etc.

#### Email Content
<img width="886" height="842" alt="Screenshot 2026-06-01 230205" src="https://github.com/user-attachments/assets/27dea066-47b1-49ab-b839-30c59910f146" />
<br>

#### Suspicious Sender Address
<img width="848" height="565" alt="Screenshot 2026-06-01 230222" src="https://github.com/user-attachments/assets/3c9a172d-0a94-4a5a-bfe8-b35b2cfa3a57" />
<br>

#### Classification & Flag
<img width="839" height="800" alt="Screenshot 2026-06-01 230308" src="https://github.com/user-attachments/assets/db83af7e-671b-4dc8-a08e-53d135dc619d" />


#### Explanation
- This one tries to override critical thinking using urgency.
- Social engineering relies heavily on psychological manipulation rather than technical exploits.


---

### Flag 4 : External Domain Red Flags

Flag : ``` THM{Get-back-SOC-mas!!} ```

---
#### Indicators Identified
- Impersonation: Pretending to be a trusted service.
- External Sender Domain: Domain looks similar but is not legitimate.
- Social Engineering Text: Attempts to lure the victim into reacting fast.

#### Email Content
<img width="1289" height="900" alt="Screenshot 2026-06-01 230426" src="https://github.com/user-attachments/assets/a055b0c5-8ba8-4269-a2b4-e7e76676296c" />
<br>

#### Email Header Investigation
<img width="833" height="565" alt="Screenshot 2026-06-01 230446" src="https://github.com/user-attachments/assets/d21221cc-68af-4731-800e-d10eef4d87fa" />
<br>

#### Classification & Flag
<img width="831" height="812" alt="Screenshot 2026-06-01 230522" src="https://github.com/user-attachments/assets/bcbcf286-9c65-4f79-9a6c-5aa5ba29e4e0" />

#### Explanation
- Attackers commonly use external look-alike domains to bypass casual inspection.
- SOC teams often catch these by analyzing MX records, SPF failure, DMARC anomalies and domain registration metadata.

---

### Flag 5 : Classic Spam Message

Flag : ```THM{It-was-just-a-sp4m!!}  ```

---
#### Indicators Identified
- Spam Content: Promotional, irrelevant, mass-mailed messages.

#### Email Content
<img width="1297" height="936" alt="Screenshot 2026-06-01 230604" src="https://github.com/user-attachments/assets/bc1ab8d2-8621-4a66-869e-62e340aa5d03" />
<br>

#### Email Header Investigation
<img width="836" height="553" alt="Screenshot 2026-06-01 230641" src="https://github.com/user-attachments/assets/8e13c6b8-2cc4-49f8-8937-9eaa17c8176c" />

<br>

#### Classification & Flag
<img width="845" height="247" alt="Screenshot 2026-06-01 230700" src="https://github.com/user-attachments/assets/f9930939-fe97-4737-b436-16af0f56dd99" />

#### Explanation
- Not every suspicious email is a phishing attack, sometimes it’s just spam.
- However, spam often hides phishing links or malware, so identifying patterns like poor grammar, random ads or mass-mail headers helps differentiate.

---

### Flag 6 : Typosquatting & Impersonation Trap

Flag : ```THM{number6-is-the-last-one!-DX!}```

---
#### Indicators Identified
- Impersonation: Fake identity crafted to gain trust.
- Typosquatting / Punycode: Domains with subtle spelling variations or Unicode characters.
- Social Engineering Text: Friendly request or emotional hook.

#### Email Content
<img width="1275" height="944" alt="Screenshot 2026-06-01 230746" src="https://github.com/user-attachments/assets/2038278e-144f-4553-9b3f-0572c7d7131a" />
<br>

#### Email Header Investigation
<img width="836" height="557" alt="Screenshot 2026-06-01 230804" src="https://github.com/user-attachments/assets/e8a6c959-0939-431a-8513-2ca715c25b05" />

<br>
<img width="600" height="103" alt="Screenshot 2026-06-01 230831" src="https://github.com/user-attachments/assets/3371988f-4279-4ce4-8e35-0a3f68aca311" />
<br>

#### Suspicious URL Comparison
<img width="587" height="157" alt="Screenshot 2026-06-01 230857" src="https://github.com/user-attachments/assets/16594cc1-1e30-4125-94bb-4b6a9604a41c" />
<br>

#### Classification & Flag
<img width="833" height="789" alt="Screenshot 2026-06-01 230922" src="https://github.com/user-attachments/assets/ed7c4ccc-f1b8-40a4-9368-efb07c868be4" />

#### Explanation
- Typosquatting is especially dangerous because visually similar domains trick users easily — punycode (xn-- variants) can mask non-ASCII lookalike characters, making phishing URLs appear legitimate.

---











