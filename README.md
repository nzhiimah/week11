# week 11 : Phishing - Phishmas Greetings

### Flag 1 : Spoofed Invoice Alert

Flag : ``` THM{yougotnumber1-keep-it-going} ```

---
#### Indicators Identified
- Spoofing: The sender appears legitimate but the underlying email address does not match the claimed identity
- Sense of Urgency: Classic “Pay immediately” or “Invoice overdue” pressure tactic.
- Fake Invoice: Attachments or links pretending to be invoices ; common phishing vector.

#### Explanation
- The first email sets the tone: an urgent invoice request designed to panic the user. 
- These attacks attempt to trick accounting teams into immediate payment.
- Always verify sender domains and cross-check invoice legitimacy.

#### Email Content
<img width="1910" height="1021" alt="Screenshot 2026-06-01 225547" src="https://github.com/user-attachments/assets/15e36cca-c798-4044-a6f0-0519278017ab" />
<br>

#### Suspicious Sender Address
<img width="848" height="558" alt="Screenshot 2026-06-01 225645" src="https://github.com/user-attachments/assets/5ec6b112-1a44-44dc-b8f4-0d95d2841174" />

<br>

#### Classification & Flag
<img width="844" height="801" alt="Screenshot 2026-06-01 225753" src="https://github.com/user-attachments/assets/7fd64fc1-d905-4d17-826e-6e56d1844f23" />

---
