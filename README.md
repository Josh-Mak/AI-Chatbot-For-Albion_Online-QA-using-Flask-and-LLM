# AI-Chatbot-For-QA-Albion_Online
This is an AI chatbot powered by a large langauge model that answers questions about the video game Albion Online.

Intro: I made this program when I was creating YouTube content for Albion Online, using Flask, google-gemini (LLM), and requests. As a creator that put out lots of educational content about the game, I got endless questions about it, and so thought a chatbot would be extremely helpful to not only me, but my viewers. This project taught me a lot about using LLM's in production code, how frontends like Flask work, and webscraping/data analysis. I also learned about more traditional chatbot methods, such as embeddings and vectorestores, as the initial version of this bot used these.

Technical Overview: Big Lips McBot uses Flask for a simple frontend that allows users to ask questions about the video game Albion Online. Heres how it works:
  1. Users ask a question about the Albion Online.
  2. The LLM extracts the 'subject' of the question.
  3. The subject is searched for in the albion online wiki, and the best matching wiki page is scraped.
  4. Data is translated into readable text, and fed back into the LLM as context with the original question.
  5. The LLM uses the original question and context to provide an answer to the question.

Purpose/Benefits:
  - Big Lips McBot makes finding information about Albion Online much easier. While in some sense, it is simply the information found on the wiki in a different format, it makes searching for the information you need extremely easy. For example, finding what abilities are available on the broadsword may be just as easy to find with a google search, but finding out the most recent balance change to the broadsword would be a much harder task without Big Lips McBot.

Current State of the Project: Functional but far from complete. 
  - After extensive tests with the LLM (google-gemini), I determined it was not quite at the level needed to make this project work, and I did not want to commit money for a better model (such as GPT 3.5), or server space for a local model.

Challenges & Future Improvements:
  - Google-Gemini is not at the level needed to make this bot work well.
  - Currently has some very crude solutions to things like context limits size for the LLM.
  - Needs a method for reading html tables.
  - Increased knowledge base with custom documents, using embeddings/vectorstores for pulling context could increase the scope of questions able to be answered.
  - Currently the bot is setup for ask 1 question, get 1 answer, with no actualy conversation or memory. However, I have set it up to be able to easily include memory in the future.
  - Integrating voice-to-text and text-to-speach for real time Q&A while the user is playing the game.
