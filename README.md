<img width="1914" height="795" alt="Screenshot 2026-06-01 225931" src="https://github.com/user-attachments/assets/d9418d31-93f8-4491-8d0b-1670343d6c64" /># week 11 : Phishing - Phishmas Greetings

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

















