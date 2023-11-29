# AI-Chatbot-For-QA-Albion_Online
This is an AI chatbot powered by a large langauge model that answers questions about the video game Albion Online.

General: Big Lips McBot uses Flask as a simple frontend that allows users to ask questions about the video game Albion Online. Using a LLM, it get's the appropriate topic of the question, and then, using websearching/scraping uses data from the wiki to inform the LLM in answering the question.

Purpose/Benefits:
  - Big Lips McBot makes finding information about Albion Online much easier. While in some sense, it is simply the information found on the wiki in a different format, it makes searching for the information you need extremely easy. For example, finding what abilities are available on the broadsword may be just as easy to find with a google search, but finding out the most recent balance change to the broadsword would be a much harder task without Big Lips McBot.

Current State of the Project: Functional but far from complete. 
  - After extensive tests with the LLM (google-gemini), I determined it was not quite at the level needed to make this project work, and I did not want to commit money for a better model (such as GPT 3.5), or server space for a local model.

Potential Improvements:
  - Google-Gemini is not at the level needed to make this bot work well.
  - Currently has some very crude solutions to things like context limits size for the LLM.
  - Needs a method for reading html tables.
  - Increased knowledge base with custom documents, using vectorstores for pulling context could increase the scope of questions able to be answered.
