# AI_agent Intensive - Capstone Project 
# Topic : AI Multi-Agent Research Assistant 
   A modular multi-agent system powered by Gemini that turns any natural-language request into an automated research workflow.

🔥 What It Does:
  * Researches topics with reliable sources
  * Finds academic papers & metadata
  * Summarizes concepts & papers in Markdown
  * Discovers & downloads datasets
  * Verifies output quality
  * Runs tasks asynchronously for speed
All coordinated by a central Orchestrator Agent.

🧩 Architecture (Simple Overview):
  * Planner → Breaks goal into subtasks.
  * Web Researcher → Gathers sources.
  * Paper Finder → Retrieves relevant papers.
  * Summarizer → Builds structured explanations.
  * Dataset Finder/Downloader → Locates & fetches datasets.
  * Verifier → Checks consistency, links & JSON.
  * Controller → Executes tasks + aggregates results.

⚡Setup:

 *install:
  pip install google-generativeai python-dotenv aiohttp tqdm requests bs4 huggingface_hub

 *Configure Gemini key:
  import os, google.generativeai as genai
  os.environ["GEMINI_API_KEY"] = "YOUR_KEY"
  genai.configure(api_key=os.environ["GEMINI_API_KEY"])

 ▶️ Run:
  controller = Controller()
  goal = input("Enter your goal: ")
  tasks = controller.plan(goal)
  result = await controller.execute(tasks)

 📄 Output:
   Clean Markdown report
   Structured lists, tables, summaries
   Downloaded dataset (ZIP) if requested
   Trace log for reproducibility

🛠️Tech Stack
   Python
   Gemini API
   AsyncIO
   Jupyter Notebook

🚧Future Enhancements
   Gradio-based UI
   Local model fallback
   Stronger verification
   Automatic dataset-to-downloader linking


######################### AI_agent Intensive - Capstone Project ############################################################











 








