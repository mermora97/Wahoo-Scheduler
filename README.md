# ScheduleRAG: A Retrieval Augmented Generation Approach to UVA Course Scheduling
![image](https://github.com/user-attachments/assets/c2a0a08a-f214-4b1f-be68-3e4979191440)
![image](https://github.com/user-attachments/assets/7d205d57-5dad-47e0-9923-3fb489ef873b)

## Project Motivation

At large universities, course scheduling support is often inadequate and falls heavily on students.  
The time-consuming task of independently navigating course catalogs and major requirements can divert attention from current coursework and even delay graduation.  

**ScheduleRAG** aims to simplify and optimize the scheduling process using a Retrieval-Augmented Generation (RAG) pipeline powered by a Large Language Model (LLM), helping students plan their academic paths more efficiently and confidently.

## Project Features
- Web scraped data from Lou’s List and UVA majors pages
- Embedded and stored data into ChromaDB vector collections
- RAG pipeline using an LLM to answer scheduling queries
- Intelligent course recommendations based on major requirements, schedule constraints, and personal preferences

## Tech Stack
- **Python** (web scraping, backend)
- **BeautifulSoup / Requests** (scraping)
- **ChromaDB** (vector database)
- **LangChain / LlamaIndex** (RAG framework)
- **LLM Model** (e.g., OpenAI GPT, HuggingFace models)

## Results
![image](https://github.com/user-attachments/assets/12dc6c1f-dd65-4583-a922-3227c82e1aaf)

The two-step RAG model was better suited for this task, providing consistently higher response relevance scores (0.68 and higher).
