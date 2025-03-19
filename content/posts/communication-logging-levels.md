---
title: "Regular Communication needs Logging Levels"
date: 2025-03-19T22:19:25+05:30
draft: false
---
# **Debugging Communication: Why Regular Communication needs Logging Levels**  

Over my career span, I have seen many engineers miss out on well-deserved recognition. And this is not because their work wasn’t great, but because they didn’t represent it appropriately. 
Whether it’s providing status updates or showcasing completed work, how you communicate matters just as much as what you communicate.  

In any business, an engineer (or any professional, really) interacts with at least three to four different personas:  
1. **Peers & Colleagues** – Those working alongside you.  
1. **Immediate Superiors** – Your team lead or project manager.  
1. **Senior Managers** – The higher-ups who oversee multiple teams.  

🔹 Understanding your audience is key to adjusting the verbosity of your updates/communication. 
I recently used the analogy of application logging levels == your verbosity of updates while mentoring a few interns, and it seemed to click well so here it is  

### **Your Communication is Like Application Logging Levels**  
Just as application logs provide different levels of detail based on the situation, your communication should vary depending on the audience. Logs help debug issues when things go wrong and provide just enough information during normal operations. The same applies to work updates as well.  

Let’s say you, an engineer, is asked for a status update on the task that they are working on. The engineer is developing an API, and there’s a bug causing unexpected null values in the response. Here’s how the responses should be in my opinion:  

---

#### **1️⃣ Debug Logs (Highest Verbosity) → Peers (Troubleshooting Together)**  
👥 **Audience:** Another engineer working closely with you on the same issue.  

💬 **Response:**  
> *"I checked the API call, and the payload has an unexpected null value. The issue seems to be at the deserialization step in `processRequest()`, where it's not handling missing attributes properly. The root cause is that the JSON parser isn't enforcing required fields. I’m testing a fix by adding a default value and implementing stricter validation."*  

✅ **Key Takeaway:**  
- Highly detailed technical explanation.  
- Mentions specific function names, root cause, and next steps.
- Perfect for collaborative debugging with a peer and this level of detail is absolutely needed here.  

---

#### **2️⃣ Info Logs (Moderate Verbosity) → Team Lead (Project Status Update)**  
👥 **Audience:** Your team lead or project manager who oversees the work. 

> *"The API fix is implemented and currently under testing. The issue was due to missing attribute handling in deserialization, which has now been addressed. All unit tests are passing, and I’ll deploy it to the staging environment by EOD for further validation."*  

✅ **Key Takeaway:**  
- Explains the problem and the status of it at a higher level.   
- Focuses on progress and next steps.  

---

#### **3️⃣ Warning/Error Logs (Filtered but Significant) → Manager (Broader Impact & Risk Assessment)**  
👥 **Audience:** A senior manager who oversees multiple teams and cares about risks, timelines, and impact.  

💬 **Response:**  
> *"We discovered an issue where certain API responses contained null values due to improper attribute handling. A fix has been applied and is being tested. We expect it to be deployed by tomorrow. No customer impact has been observed so far."*  

✅ **Key Takeaway:**  
- Focuses on business impact, resolution status, and timeline.  
- Addresses risk ("no customer impact observed") to reassure leadership.  

---

#### **4️⃣ Critical / health check (Minimal Verbosity) → Leadership & Executives (Strategic Update)**  
👥 **Audience:** VPs, CTOs, Business Leaders who care about the bigger picture.  

💬 **Response:**  
> *"All API services are functioning normally. We continue to optimize reliability and are addressing minor issues as they arise. No disruptions are reported."*  

✅ **Key Takeaway:**  
- No mention of debugging or implementation details.  
- Focuses on stability & reliability.  
- Reassures leadership without raising unnecessary concerns.  

---

**Communication is about providing the right level of detail to the right audience.**  
- Too much detail?  **The audience gets bored.**  
- Too little detail? **It causes anxiety since loss of confidence creeps in if troubleshooting is being done effectively.**  

By metering verbosity based on the recipient’s role it ensures all necessary stakeholders are at peace including you ;)
