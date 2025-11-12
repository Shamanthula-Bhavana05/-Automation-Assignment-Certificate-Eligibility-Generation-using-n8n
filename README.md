# 🏆 Certificate Eligibility Generation using n8n

## 📘 Project Overview
This project automates the **Certificate Eligibility Generation** process for students at **Innomatics Research Labs** using **n8n**, a workflow automation tool.  

It collects student performance details via **Google Forms**, stores them in **Google Sheets**, and uses **n8n workflows** to automatically determine which certificate each student qualifies for — **Gold 🥇, Silver 🥈, Bronze 🥉, or Not Eligible ❌**.  

Once eligibility is decided, personalized emails are automatically sent to each student with their certificate status.

---

## 🎯 Objectives
- Automate the evaluation of student performance  
- Determine certificate eligibility based on predefined conditions  
- Send personalized certificate emails automatically  
- Reduce manual effort and human error  

---

## ⚙️ Workflow Components
### 1. **Google Form**
Collects student performance data including:
- Name  
- Email ID  
- Batch Number  
- Monthly Assessment Marks  
- Total Tasks Completed  
- Quiz Marks  
- Total Assignments Completed  
- Project Presentation (Yes/No)

### 2. **Google Sheets**
Stores form responses automatically and serves as input data for the n8n workflow.

### 3. **n8n Workflow**
- **Google Sheet Node** → Reads data  
- **If / Switch Node** → Applies eligibility logic  
- **Code Node (optional)** → Adds custom formatting or logic  
- **Email Node** → Sends personalized result emails  

---

## 🧮 Eligibility Criteria
| Certificate Type | Conditions |
|------------------|------------|
| 🥇 **Gold** | Marks > 80, Tasks = 10, Assignments = 10, Quiz > 80, Project = Yes |
| 🥈 **Silver** | Marks 60–80, Tasks = 10, Assignments = 10, Quiz 60–80, Project = Yes |
| 🥉 **Bronze** | Marks 40–60, Tasks = 10, Assignments = 10, Quiz 40–60, Project = Yes |
| ❌ **Not Eligible** | Does not meet any criteria |

---

## ✉️ Email Templates

### 🥇 Gold Certificate
**Subject:** 🎉 Congratulations! You’re Eligible for the Gold Certificate  
**Body:**  
Hello {{Name}},  
Congratulations! Based on your outstanding performance, you are eligible for the **Gold Certificate**.  
Keep up the great work and continue shining! ✨  

---

### 🥈 Silver Certificate  
**Subject:** Good Job! You’ve Earned the Silver Certificate  
**Body:**  
Hello {{Name}},  
Great effort! Based on your results, you are eligible for the **Silver Certificate**.  
Keep pushing forward — Gold is just one step away! 🏅  

---

### 🥉 Bronze Certificate  
**Subject:** You’re Eligible for the Bronze Certificate  
**Body:**  
Hello {{Name}},  
Well done! You’ve qualified for the **Bronze Certificate**.  
Keep practicing and improving to reach Silver or Gold next time! 💪  

---

### ❌ Not Eligible  
**Subject:** Update on Your Certificate Eligibility  
**Body:**  
Hello {{Name}},  
Thank you for your participation. Currently, you are **not eligible** for a certificate.  
Complete all tasks, assignments, and quizzes, and improve your marks based on the given criteria.  
You’ve got this — keep trying! 💫  

---

## 🧩 Tech Stack
- **n8n** – Workflow Automation  
- **Google Forms** – Data Collection  
- **Google Sheets** – Data Storage  
- **Gmail Node** – Automated Email Sending  

---

## 📊 Workflow Diagram
```text
Google Form → Google Sheet → n8n Workflow → Eligibility Logic → Send Email
````
<img width="1920" height="905" alt="Certificate Eligibility Generation using n8n(Interface)" src="https://github.com/user-attachments/assets/e1ee96f5-1aac-4e0b-b391-50910b9984dc" />


---

## 🎥 Project Demo
🎥 **Watch the full project demo here:**  
🔗 [YouTube Video](https://youtu.be/hesajiGYEnE?si=pgESyifG72_XPLMD)

📂 **GitHub Repository:**  
🔗 [Certificate Eligibility Generation using n8n](https://github.com/Shamanthula-Bhavana05/-Automation-Assignment-Certificate-Eligibility-Generation-using-n8n)

---

## 🌐 Connect with Me

💼 **LinkedIn:** [Shamanthula Bhavana](https://www.linkedin.com/in/shamanthula-bhavana-7343bb331)
📂 **GitHub Repository:** [Shamanthula Bhavana](https://github.com/Shamanthula-Bhavana05)
---

## 🏁 Conclusion

This automation project efficiently evaluates student performance and sends certificate eligibility emails in real-time. It eliminates manual effort, ensures accuracy, and demonstrates strong workflow automation skills using **n8n**.

---


