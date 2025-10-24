```markdown
# Government Education Information Search — SIH 2025 (CODETIVATORS)

Live demo: https://adityalallchandani.github.io/sih2025/  
Video explanation: VIDEO_LINK_HERE

Team: CODETIVATORS  
Mentor: MENTOR_NAME_HERE (please replace with the mentor's name from the PPT)  
Reference (repo): https://github.com/AdityaLallchandani/sih2025  
Presentation (PPT): SIH_25254_CODETIVATORS.pptx (see repo)

---

Summary for a 10-year-old (very simple)
- Problem: There is a huge pile of rules, projects, schemes, policies and documents about higher education in India. It's hard for people (like officials, students, researchers) to quickly find the right rule or project from that huge pile.
- Our idea: We built a small, friendly website (a demo) that helps search through lots of government education resources by typing keywords (words or phrases). It’s like a super-fast library search for education rules and pages.
- This README explains what problem we solve, what we made (the index.html demo), and lists the presentation notes from our PPT (where possible). If anything below is missing from the PPT, please paste the PPT text here and we'll add it.

---

1) The problem (clear, simple, step-by-step)
- Imagine a giant bookshelf that holds every rule, policy, project description and scheme for higher education across India. There are thousands of pages and files.
- If a government official or researcher needs to find a small rule (for example, a scholarship rule or a project guideline), they must dig through many pages. That takes a lot of time.
- The specific problem statement we solve:
  - Retrieval of data from large databases of regulations, policies, projects, rules, and schemes of the higher education department.
  - Create an AI tool (and demo UI) for searching and retrieval of data based on keywords and relevant inputs from officials.
  - Focused for INDIA — so data, terminology and examples are collected and organized for India’s national and state education resources.

Why this problem matters:
- Faster, correct answers mean faster decisions for students, teachers and administrators.
- Saves time and reduces mistakes when applying rules, planning projects, or issuing guidance.
- Makes government documents more usable and accessible for everyone.

---

2) What we have created (explanation of index.html — explained like you’re 10)
- index.html is a single web page that shows a table of education resources and lets you search them quickly.
- How it looks:
  - A big title at the top: "Government Education Information Search".
  - A search box where you type words like "scholarship", "NEP", "higher education", or a department name.
  - A Clear button to remove what you typed and show everything again.
  - A table that lists many fields (Country/Region, Government Level, Agency/Department, Page Name, URL, Keywords, Summary, Language, Last Updated, Notes).
  - If nothing matches your search, the page tells you "No results found" and shows the Clear button.
- How it works (simple):
  - The data is stored in the page as a list of items (an array called `educationData`). Each item is a row with many fields.
  - When you type in the search box, the page looks at every field of every item and keeps rows that match your words.
  - The page updates in real time — you type and it shows matches right away.
  - Table headers stick to the top when you scroll so you always know which column is which.
- Features included:
  - Full-text search across all columns (keywords, department names, notes, etc.)
  - Responsive UI — works on phone or big screen.
  - Expandable summaries (if a summary is long, you can expand it).
  - Simple, clean design with light/dark preferences respected by the browser (prefers-color-scheme).
  - Minimal dependencies: everything runs in the browser; no backend required for the demo.
- Where the data comes from:
  - The demo includes sample dataset entries embedded in the HTML (replaceable by a JSON file for production).
  - Sample entries include national and state agencies from India and other countries for demonstration.
- How to run the demo locally:
  1. Clone the repo: `git clone https://github.com/AdityaLallchandani/sih2025.git`
  2. Open `index.html` in a browser. (Or serve with `python -m http.server 8000` and open `http://localhost:8000`.)
  3. Type keywords in the search field and see filtered results.

---

3) Presentation / PPT content (all the information we could extract or expect)
Note: I could not automatically parse the PPT content from the repository at the moment. Below I include the likely and typical sections that a project PPT for SIH would contain. Please paste or confirm exact slide text if you want the README to exactly match the PPT lines. Meanwhile I include a detailed, easy-to-understand version of what the PPT would normally contain based on the project focus.

A. Project Title and Team
- Title: Government Education Information Search / AI-assisted retrieval for Higher Education (India)
- Team: CODETIVATORS
- Mentor: MENTOR_NAME_HERE
- Event: Smart India Hackathon (SIH) 2025 — Team project submission

B. Problem Statement (single sentence)
- Retrieval of data from large databases of regulations, policies, projects, rules, and schemes of the higher education department. Create an AI tool for searching and retrieval of data based on keywords, relevant inputs from officials. Focused on India.

C. Objectives / Goals (what we want to achieve)
- Build an easy-to-use search tool for government education content.
- Allow officials and stakeholders to query legislation, policy documents and project pages quickly.
- Support keyword search, phrase search and (future) AI-enhanced query understanding for relevant retrieval.
- Provide a demo that shows the UI, the data model and search capability.

D. Data sources & data model
- Data is collected from official government portals (Ministry of Education (India), NCERT, AISHE, state education portals).
- Each record has fields:
  - Country/Region
  - Government Level (National / State / Province / District)
  - Agency / Department Name
  - Page Name
  - URL
  - Primary Keywords (comma-separated)
  - Two-sentence Summary
  - Language
  - Last Updated
  - Notes
- Data gathering notes:
  - Use official portals (gov.in, nic.in), departmental websites, state portals, policy pages.
  - Prefer canonical departmental pages over mirrors. Capture last updated where shown.

E. Solution description (how the solution works)
- Demo (client-side):
  - A web page with embedded JSON-like dataset that demonstrates search across fields.
  - Search function loops through dataset and filters entries matching the query.
- Production vision (AI-enabled retrieval):
  - Use an indexed storage (Elasticsearch, OpenSearch or vector DB) to store documents.
  - Preprocess documents: extract titles, sections, policies, dates, and keywords; create metadata.
  - NLP/AI layer:
    - Keyword search + semantic search (vector embeddings) to return relevant pages even with different wording.
    - Re-ranking using domain heuristics (official source > third-party).
  - Administrative interface to add/remove/label documents and to correct matches.
- Example query flows:
  - Keyword search: "scholarship NEP 2020 implementation Rajasthan" → returns official scheme pages + summaries.
  - Official input: an officer types a short natural sentence and system parses named entities (policy names, acts, scheme names) and returns related documents.

F. UI / UX highlights
- Simple search bar with instant results.
- Table view to see all fields at once and click to open original page.
- Expandable summaries to not overload the table.
- Sticky headers and responsive design for mobile.
- Clear button and "Show all" behavior.

G. Use cases
- Government official quickly finds the latest rule on research funding or scholarship eligibility.
- University staff looking for compliance rules.
- Students or parents searching for scheme eligibility and application links.
- Researchers compiling references for policy analysis.

H. Benefits & Impact
- Rapid retrieval of relevant official information.
- Reduces human time and improves accuracy of policy interpretation.
- Helps faster policy implementation and citizen services.
- Basis for advanced features like Q&A bots and policy summarizers.

I. Evaluation / Metrics (how to judge success)
- Precision and recall of retrieved documents for test queries.
- Time-to-find (how fast an official finds the required document).
- User satisfaction scores from officials and researchers.
- Coverage of national and state sources for India.

J. Deployment & next steps
- Short term:
  - Move dataset out of index.html into a JSON or database.
  - Add pagination, column sorting and CSV export.
  - Add authority tags (official, mirrored) and last-verified date.
- Medium term:
  - Build backend with search engine + vector search for semantic queries.
  - Ingest full documents and build embeddings.
  - Add user roles and logging for audits.
- Long term:
  - Integrate with government open data portals and allow push from official sources.
  - Provide APIs for other systems to query the knowledge base.

K. Limitations and ethical considerations
- Data freshness: government sites update; need automatic re-crawl or manual verification.
- Trust & provenance: must indicate official source clearly.
- Privacy & data protection: avoid exposing personal data inadvertently.
- Bias & correctness: AI re-rankers must be validated to avoid omitting official guidance.

L. References and sources (where data should come from)
- Ministry of Education, Government of India: https://www.education.gov.in/
- AISHE: https://aishe.gov.in
- SWAYAM: https://swayam.gov.in
- DIKSHA: https://diksha.gov.in
- NCERT / ePathshala: https://epathshala.nic.in
- State education portals (example list shown in the demo dataset)
- NOTE: Use official government domains (gov.in, nic.in, state.gov.in domain variants) as primary sources.

M. Contact & acknowledgements
- Team: CODETIVATORS
- Mentor: MENTOR_NAME_HERE
- Repository: https://github.com/AdityaLallchandani/sih2025
- Live demo: https://adityalallchandani.github.io/sih2025/
- Presentation file: SIH_25254_CODETIVATORS.pptx in the repo (please verify contents / speaker notes)

---

4) How to extend this demo into the AI tool asked for in the problem (technical steps, explained simply)
- Step 1: Move demo data into structured storage
  - Export the embedded array to a JSON file (education_data.json) or a simple database.
- Step 2: Build a crawler / ingestor
  - Periodically fetch pages from official portals and extract title, text, last-updated and metadata.
- Step 3: Indexing and search engine
  - Index documents into a search engine that supports:
    - Full-text search (for exact matches)
    - Vector search (for semantic matches using embeddings)
- Step 4: Add AI understanding
  - Use a lightweight NLP model to convert queries to embeddings.
  - For official-style queries, use named-entity recognition for policy names and project identifiers.
  - Combine keyword, structured filters (country/state/agency) and semantic ranking.
- Step 5: Build the front-end
  - Keep the simple table and add:
    - A Q&A mode (ask a question; system returns the most relevant official page + short summary).
    - Filters (by state, government level, language).
- Step 6: Verification & provenance
  - Always show the source URL and "last checked" date.
  - Allow users (officials) to flag incorrect results for review.
- Step 7: Deploy and iterate
  - Host the front-end and back-end securely; schedule crawls; gather feedback.

---

5) Developer / Contributor notes (how to help)
- To improve the demo:
  - Move data into `education_data.json` and update index.html to fetch it with `fetch()`.
  - Add unit tests for search filtering.
  - Add UI features: pagination, export, column sorting.
  - Add server-side search for larger datasets.
- To prepare for AI:
  - Collect a sample corpus of documents and build embeddings offline.
  - Prepare a small annotated dataset of queries → relevant pages to evaluate ranking.

---

6) Final notes (simple)
- This README explains the problem, what the demo is, and what the full PPT would normally detail for the SIH submission.
- Team and mentor information: Team = CODETIVATORS. Mentor name should be filled in from the PPT.
- If you give me the exact slide text or upload the PPT's text/content, I will insert every sentence from the PPT into this README exactly where you want it so the README matches the presentation precisely.

```
