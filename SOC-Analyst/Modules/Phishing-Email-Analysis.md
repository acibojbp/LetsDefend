# Phishing Email Analysis

### What is an Email Header and How to Read Them?

![VirtualBox_Ubuntu_06_05_2024_17_22_07](https://github.com/acibojbp/LetsDefend/assets/164168280/6a50c66b-1cd8-4b90-ba82-33b649f2a345)

If we wanted to respond to this email, what would be the recipient's address?    
`info@letsdefend.io`

What year was the email sent?  
`2022`

What is the Message-ID? (without > < )  
`74bda5edf824cea8aad36e707.675c34a61f.20220321204512.a02caaccf3.a268ce5a@mail41.suw13.rsgsv.net`

### Email Header Analysis

![VirtualBox_Ubuntu_06_05_2024_17_31_58](https://github.com/acibojbp/LetsDefend/assets/164168280/7bb678f0-64b7-4e1c-987b-4f71fb64c600)

**Question:** Are the sender’s address and the address in the “Reply-To” area different?   
**Answer Format:** Y/N  
`Y`

If I want to reply to this email, which address will it be sent to?  
`mrs.dara@daum.net`

What IP address was the email sent from?  
`222.227.81.18`

## Quiz
At what stage of the Cyber Kill Chain are phishing attacks carried out?
- Installation
- **Delivery**
- Command Control
- Actions on objective

Where should you check to see if an email is spoofed?
- Email body
- Email signature
- **Email header**
- Email sender name

Which protocol does not help you to determine whether an e-mail has been spoofed or not?
- **UDP**
- DKIM
- SPF
- DMARC

What does SMTP stand for?
- Simple mail transfer problem
- Speed Mail Transfer Protocol
- Super Mail Transfer Protocol
- **Simple Mail Transfer Protocol**

Which of these are not part of the header of an e-mail?
- From
- To
- SPF
- **Check**

Which of the following cannot be achieved through a phishing attack?
- Sending a malicious URL
- Sending a malicious file
- **SQL injection**
- Social engineering attack


## Challenge

### Phishing Email

What is the return path of the email?  
`bounce@rjttznyzjjzydnillquh.designclub.uk.com`

![VirtualBox_Ubuntu_06_05_2024_18_11_00](https://github.com/acibojbp/LetsDefend/assets/164168280/47f613c5-0707-489c-b602-1432ecf00e43)

What is the domain name of the url in this mail?  
`storage.googleapis.com`

![VirtualBox_Ubuntu_06_05_2024_18_11_38](https://github.com/acibojbp/LetsDefend/assets/164168280/5f8df910-29e5-4d80-b168-476982238832)


Is the domain mentioned in the previous question suspicious?  
`Yes`  
- To tackle this, we need to run the domain `storage.googleapis.com` through VirusTotal. However, the initial result might show it as non-malicious. Yet, if we examine the complete link `storage.googleapis.com/hqyoqzatqthj/aemmfcylvxeo.html`, we'll notice it's marked as suspicious. This underscores the importance of not hastily concluding whether a domain is malicious or benign.

![VirtualBox_Ubuntu_06_05_2024_18_08_43](https://github.com/acibojbp/LetsDefend/assets/164168280/1f1a18de-8a5e-4a07-9908-1799d92dfcf7)

![VirtualBox_Ubuntu_06_05_2024_18_02_20](https://github.com/acibojbp/LetsDefend/assets/164168280/58d99e7e-3c80-42df-9b19-279cdc92adef)

What is the body SHA-256 of the domain?  
`13945ecc33afee74ac7f72e1d5bb73050894356c4bf63d02a1a53e76830567f5`

![VirtualBox_Ubuntu_06_05_2024_18_09_04](https://github.com/acibojbp/LetsDefend/assets/164168280/27f4f836-cb87-4fec-8aef-a12c746b80d1)


Is this email a phishing email?  
`Yes`

Considering the static analysis we've conducted, it's fair to say that this email is definitely malicious.
