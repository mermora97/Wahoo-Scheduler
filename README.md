# ScheduleRAG: A Retrieval Augmented Generation Approach to UVA Course Scheduling

## Project Motivation

Course scheduling support is inadequate at large universities and typically falls on students. Diverting attention from maintaining proper marks for current classes can be detrimental to students who may have to extend their enrollment to extra semesters. We look to aid students in this challenging and critical process with a RAG-supplemented LLM scheduler.

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

The two-step RAG model was better suited for this task, providing consistently higher response relevance scores (0.68 and higher).

   
- Figures
   - ![image](https://github.com/user-attachments/assets/7d205d57-5dad-47e0-9923-3fb489ef873b)
   - ![image](https://github.com/user-attachments/assets/9e6a081e-53d2-4b0a-a0b7-4c3a9db920a1)
