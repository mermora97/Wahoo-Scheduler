# ScheduleRAG: Recommendation for UVA Course Scheduling

## Motivation

Course scheduling support is inadequate at large universities and typically falls on students. Diverting attention from maintaining proper marks for current classes can be detrimental to students who may have to extend their enrollment to extra semesters. We look to aid students in this challenging and critical process with a RAG-supplemented LLM scheduler.

## Models

One and two-step RAG methods were developed to provide personalized schedules. Vectorized course and degree requirements databases provided context for the model generation.

## Results

The two-step RAG model was better suited for this task, providing consistently higher response relevance scores (0.68 and higher).

## To Do: 4/9/25
Powerpoint
- SiS
- Lou's List
- us vs Chat GPT
- Keep it engaging (video and NOT live coding)
- Memes later on for added flare

Paper
- Continue working on this (Courtney & Hannah)
- Rachel's RAG Model Implimentation
  - "Biology undergrad 2nd year 2025"
  - Uses the input above to query the course description DB using vector imbedding matching
  - The output is text for the first LLM pass: 1) user query, 2)  text from database - major descriptions/ requirements, 3) system prompt #1 - tells the LLM it's purpose, the output it should provide, instructions to not hallucinate. The output of this is input as a new query to be embedded in another vector look up to do a look-up into the courses database (Lou's List). The output of this, along with the outputs from the original database lookups from the major descriptions, as well as the OG user query AND system prompt #2 - table format, no class overlap, 12-15 credits per semester, first year students shouldn't have upper level courses, times should be included, other format specifications & specifics for courses.
  - The output of this is our final product!
- Mercedes' RAG Model Implimentation
  - "Biology undergrad 2nd year 2025"
  - Uses input to query the course description database (UVA SIS) using vector imbedding matching
  - Uses the exact same input to also query the course database (Lou's List) using vector imbedding matching
  - Whatever output comes from both databases after both querries, we then feed to the LLM to provide a course description for the user
  - Feeds the user query to both major and courses DB collection. The major should get the requirements and courses should retrieve the times, schedule, etc. and EVERYTHING is combined and fed to the LLM to merge both features. 
- Goal:
  - what's the best way to produce better results?
     - Tuning variables? reducing tokens: 20k to fewer (Rachel)
   
- Figures
   - ![image](https://github.com/user-attachments/assets/7d205d57-5dad-47e0-9923-3fb489ef873b)
   - ![image](https://github.com/user-attachments/assets/9e6a081e-53d2-4b0a-a0b7-4c3a9db920a1)



Research
- Looking into a better LLM model that considers GPUs vs CPUs to increase computation speed.

---
## To Do: 3/31/25
Paper: (Hannah)
- Introduction & Related Works
- Methodology
- Literature review

Lou's List Data into SQL Database for querying: (Courtney)
- Ask Prof if an SQL database will work the best to store and query our Database using our LLM

Rag model & LLM:
- Vectorized database

