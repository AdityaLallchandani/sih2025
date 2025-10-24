# 🧠 Government Education Information Search — SIH 2025 (CODETIVATORS)

**Live Demo:** [https://adityalallchandani.github.io/sih2025/](https://adityalallchandani.github.io/sih2025/)

**Video Explanation:** [https://www.youtube.com/your_project_video](https://www.youtube.com/your_project_video)

**Repository:** [https://github.com/AdityaLallchandani/sih2025](https://github.com/AdityaLallchandani/sih2025)

**Team Name:** CODETIVATORS
**Mentor:** Dr. Akash Mecwan (Electronics and Communication Engineering Department)

---

## 🧩 The Problem — Explained Simply

Imagine there’s a *giant library* full of thousands of books and files — all containing India’s education rules, policies, projects, regulations, and government schemes.

Now, suppose an education officer, student, or teacher wants to find one small piece of information, like:

* “What is the latest rule for scholarship eligibility?”
* “Which scheme helps students with low income?”
* “What are the policies under NEP 2020?”

Right now, they must search across many websites and PDFs. That takes **a lot of time** and often leads to confusion.

### 🧠 Our official problem statement:

> **Retrieval of data from large databases of regulations, policies, projects, rules, and schemes of the higher education department. Create an AI tool for searching and retrieval of data based on keywords and relevant inputs from officials.**

### 🎯 Why this problem matters

* Saves hours of searching and confusion.
* Helps government officials make **faster and smarter decisions**.
* Makes education rules and policies **transparent and easy to find**.
* Ensures that correct and updated information reaches students, universities, and the public.

---

## 💡 What We Created — The Demo (index.html)

We built a **demo website** that shows how the main idea will work.
You can see it live here: [https://adityalallchandani.github.io/sih2025/](https://adityalallchandani.github.io/sih2025/)

### 🔍 How it works

* When you open the website, you’ll see a **search box** and a big **table** of government education information.
* You can type words like “scholarship”, “AICTE”, or “higher education”.
* As you type, the table automatically filters and shows only the matching items.
* Each row includes:

  * **Country/Region**
  * **Government Level (Central or State)**
  * **Agency/Department Name**
  * **Page Name**
  * **URL** (direct link to that page)
  * **Keywords**
  * **Summary**
  * **Language**, **Last Updated**, and **Notes**

If you type something and there’s no result, the website politely says “No results found”.

### ⚙️ What happens behind the scenes

* The page stores all data in a simple **JavaScript array** (like a digital spreadsheet).
* Every time you type, the program checks every entry to find matches.
* It’s **fast**, runs **entirely in the browser**, and doesn’t need a backend server for the demo.
* It’s built with **HTML, CSS, and JavaScript** only.

### 🧰 Features in the demo

* Instant keyword filtering
* Mobile-friendly design
* Sticky table headers
* Expandable summaries
* Dark/light mode support

This demo is like a **tiny example** of the full AI-powered system we plan to build.

---

## 🤖 Our AI Solution — “INSIGHT AI”

Our main proposed solution is called **Insight AI** — a secure, intelligent portal designed to give **instant, accurate policy answers**.

### ✨ What Insight AI does

* **Multilingual Support:** You can ask and get answers in regional languages.
* **Cross-Document Comparison:** It can compare “Policy A vs. Policy B”.
* **Automated Summarization:** Gives you a quick summary (“TL;DR”) of long policy documents.
* **Policy Relationship Graph:** Shows how different acts, schemes, and rules are connected.
* **Smart Financial Advisory:** Suggests cost-saving options using available government schemes.

### 🧩 How it solves the problem

* Brings all education data to one place.
* Finds and shows answers directly from *official documents*.
* Links to exact paragraphs so you can trust the information.

---

## 🌟 Innovation & Uniqueness

| Feature                | Description                                      |
| ---------------------- | ------------------------------------------------ |
| **Understands Intent** | Knows what you *mean*, not just what you *type*. |
| **Direct Answers**     | Gives short summaries, not just links.           |
| **100% Verifiable**    | Every answer links to the real source section.   |

---

## 🧱 Technical Approach

| Layer                 | Tools & Technology                        |
| --------------------- | ----------------------------------------- |
| **Frontend**          | HTML, CSS, JavaScript (for responsive UI) |
| **Backend**           | Python (Flask or FastAPI)                 |
| **Database**          | Vector Database (e.g., ChromaDB)          |
| **Methodology (RAG)** | Retrieval-Augmented Generation            |

### ⚙️ How RAG Works (Simplified)

1. **Ingest:** Feed all official documents (MoE, UGC, AICTE).
2. **Index:** Create a searchable “knowledge index”.
3. **Retrieve:** When someone asks something, find matching sections.
4. **Generate:** Summarize the results into a clear, short answer.

---

## 📊 Feasibility and Viability

* **Technical Feasibility:** ✅ High (RAG is well-documented and stable).
* **Data Feasibility:** ✅ High (documents from MoE, UGC, AICTE are public).

### Difference from Chatbots

Ordinary chatbots answer simple public FAQs.
**Insight AI** is a *smart internal tool* for officials, designed to handle **complex policy questions**.

### Extra Capabilities

* **Timeline Analysis:** See how policies changed over time.
* **Proactive Alerts:** Get notified when new documents are uploaded.
* **Role-Based Access:** Secure logins for different user types.

---

## 🌍 Environmental & Social Impact

* **Paperless queries** → saves trees every year.
* **Reduces travel** → no need to visit offices for verification.
* Promotes **Green Initiative** and supports a **digital India** vision.

---

## 💪 Impact & Benefits

| Group                       | Benefits                                               |
| --------------------------- | ------------------------------------------------------ |
| **Officials**               | Saves time, improves confidence and decision accuracy. |
| **Students & Universities** | Simplifies scholarship and approval processes.         |
| **Public**                  | Improves transparency and access to education schemes. |

---

## ⚠️ Challenges & Our Solutions

| Challenge                            | Solution                                                             |
| ------------------------------------ | -------------------------------------------------------------------- |
| Complex document formats (PDF scans) | Use **OCR** for text extraction.                                     |
| Keeping data current                 | Use **automated web crawlers**.                                      |
| Wrong AI answers                     | Add **human-in-the-loop verification** and **confidence scores**.    |
| Multilingual accuracy                | **Fine-tune** models using translated Indian education data.         |
| User adoption                        | **Training sessions + Gamification** (leaderboard for most queries). |

---

## 📚 Research and References

### 🔗 Primary Data Sources

* [Ministry of Education, Government of India](https://www.education.gov.in)
* [University Grants Commission (UGC)](https://www.ugc.ac.in)
* [All India Council for Technical Education (AICTE)](https://www.aicte-india.org)

### 📘 Key Reference Documents

* **National Education Policy 2020** — Ministry of Education, Govt. of India
* **AICTE Approval Process Handbook** (Latest Edition)
* **RUSA (Rashtriya Uchchatar Shiksha Abhiyan)** — Master Guidelines
* **Julija, D. (2021).** *What is Retrieval-Augmented Generation (RAG)?* [Medium Article](https://medium.com/@drjulija/what-is-retrieval-augmented-generation-rag-938e4f6e03d1)

---

## 👥 Team & Mentor

| Role             | Name                                                       |
| ---------------- | ---------------------------------------------------------- |
| **Team Name**    | CODETIVATORS                                               |
| **Project Name** | Insight AI                                                 |
| **Mentor**       | Dr. Akash Mecwan (Electronics & Communication Engg. Dept.) |
| **Hackathon**    | Smart India Hackathon 2025                                 |

---

## 🎬 Project Files

* **Presentation:** `SIH_25254_CODETIVATORS.pptx`
* **Project Documentation and Prototype Video:** [YouTube Link](https://www.youtube.com/your_project_video)
* **GitHub Repository:** [https://github.com/AdityaLallchandani/sih2025](https://github.com/AdityaLallchandani/sih2025)
* **Live Demo:** [https://adityalallchandani.github.io/sih2025/](https://adityalallchandani.github.io/sih2025/)

---

## 🧭 In Summary

We made a smart helper called **Insight AI** that helps people find the right rule or policy about education in India — just by typing a few words.
It reads big government documents, understands what you mean, and gives short, verified answers.
Our demo website shows the idea in action, and our next step is to make it fully AI-powered for real officials to use.

